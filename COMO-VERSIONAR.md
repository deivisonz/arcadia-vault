---
tags: [sistema]
tipo: guia
---
# 🔧 Como versionar o Arcadia no Git

> Rode estes comandos **na sua máquina** (Git Bash ou PowerShell), dentro da pasta do vault.
> Motivo: o ambiente do Claude não tem `git-lfs`, não pode apagar arquivos da pasta e não tem suas credenciais do GitHub.

O repositório está bem: histórico e arquivos intactos. Só o cache de índice (`.git/index`) ficou corrompido e precisa ser reconstruído.

---

## Passo 1 — Consertar o índice

**Git Bash:**
```bash
cd "/d/Documents/Obsidian Vault/Arcadia"
rm -f .git/index.lock .git/index
git reset
git status        # deve voltar ao normal e listar os arquivos novos
```

**PowerShell:**
```powershell
cd "D:\Documents\Obsidian Vault\Arcadia"
Remove-Item -Force .git\index.lock, .git\index -ErrorAction SilentlyContinue
git reset
git status
```

---

## Passo 2 — Corrigir o LFS para o mapa atual

A regra antiga aponta para `Atlas/Arcadia Map.jpg`, que não existe mais. O mapa atual é `Atlas/arcadia.webp` (21 MB) e não estava sendo rastreado.

```bash
git lfs install
git lfs track "*.webp" "*.jpg" "*.png"
```

---

## Passo 3 — Ignorar a config do Obsidian, commitar e enviar

```bash
printf '.obsidian/\n.DS_Store\nThumbs.db\n.trash/\n' > .gitignore
git rm -r --cached .obsidian
git add -A
git commit -m "Estrutura de worldbuilding + piloto Panteão Tibérico; LFS no mapa atual; ignora .obsidian/"
git push
```

---

## Depois disso

- Os próximos commits podem ser feitos direto pelo plugin **Obsidian Git**, sem terminal.
- Limpeza opcional (sem urgência): o mapa antigo de ~194 MB ainda ocupa espaço no histórico do LFS. Quando tiver certeza que não precisa dele, rode `git lfs prune`.

---

## Se der erro

Copie a mensagem e me mande — eu ajudo a destravar.
