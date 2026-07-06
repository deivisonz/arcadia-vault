---
tags: [MOCs, sistema]
tipo: índice-mestre
---
# 🗺️ Cânone de Arcádia

Fonte da verdade do mundo. Este arquivo define **como trabalhamos**, o **estado atual** do vault e os **fios centrais** que tudo o mais deve respeitar.

---

## Como trabalhamos (fluxo acordado)

1. **Propor antes de escrever.** Para qualquer lore nova, eu apresento um esboço ou opções primeiro; só escrevo no arquivo depois do seu OK.
2. **Referências em wikilink.** Toda menção a uma entidade que tem (ou terá) ficha vira `[[link]]`, para alimentar o grafo do Obsidian.
3. **Revisão por diff + changelog.** O vault é versionado em git. Toda sessão eu registro o que mexi em [[Registro de Alterações]], e você confere pelo diff.
4. **Pipeline de status** em cada ficha (campo `status` no frontmatter):
   `esboço` → `rascunho` → `revisão` → `cânone`
   - **esboço**: arquivo vazio ou só estrutura.
   - **rascunho**: conteúdo bruto meu, ainda não lido por você.
   - **revisão**: pronto para você aprovar/corrigir.
   - **cânone**: aprovado por você. Vira lei do mundo.
5. **Só o que está em `cânone` é imutável.** O resto é maleável e pode ser reescrito livremente.

---

## Convenções de escrita

- **Idioma:** português (PT-BR), tom de fantasia sombria, registro "in-world" quando fizer sentido (como se escrito por um cronista de Arcádia).
- **Nomenclatura de arquivos:** nome próprio da entidade (`Draukar.md`), sem prefixos. Templates começam com `_Template - `.
- **Datas:** sempre no sistema de eras — `EH` (Era dos Heróis), `ET` (Era das Trevas), `1E`, `2E`. Presente narrativo ≈ **2E 718–720**.
- **Frontmatter:** todo arquivo de conteúdo recebe `tipo`, `status` e `tags`. Campos de relação (`região`, `capital`, `afiliação`…) usam `"[[link]]"`.
- **Ganchos de expansão:** cada ficha termina com uma seção `#### Ganchos de expansão` — perguntas em aberto que eu posso desenvolver depois.

---

## Princípio das referências (regra de ouro)

**Tudo em Arcádia tem uma âncora no mundo real ou em outras obras de fantasia — com um toque único que a distingue.** Esta é a bússola criativa do mundo. Ao criar ou expandir qualquer coisa, eu parto da referência declarada e depois acrescento o "twist arcadiano".

Cada ficha carrega um campo `referência` no frontmatter, nomeando sua(s) inspiração(ões).

Referências já estabelecidas:

| Elemento | Referência-base | Toque único |
|---|---|---|
| [[Panteão Tiberico]] | Deuses greco-romanos | Divindade incognoscível (ver [[A Natureza do Divino]]) |
| [[Panteão Nordico]] | Mitologia nórdica | Ligado às três luas e ao inverno de eras |
| Terras dos Skalds / Clãs | Reinos nórdicos / vikings | Divididos em Clãs do Lobo e do Urso |
| [[Bruvia]] | Inglaterra medieval + Norte de *Game of Thrones* | — |
| [[Uria]] | Roma imperial / teocracia | Culto ao Imperador, xenofobia extrema |
| [[Tarov]] / [[Astarov]] | Roma (Império dividido) + minotauros | Cisma escravista vs. cosmopolita |
| [[Saewan]] | Japão feudal | Samurais e ninjas em arquipélago |
| [[Tapesh]], [[Habajj]] | Pérsia / mundo árabe | Mar de areia navegável |
| [[Os Três Dragões]] | Mitos de dragões primordiais | Fundam minotauros, elfos silvestres e a magia humana |

> [!note] Ao expandir, sempre declarar a referência
> Se a referência de um elemento ainda não estiver definida, eu proponho uma antes de escrever.

## Templates disponíveis

Em [[Templates]]: Reino & Império · Cultura & Povo · Divindade · Personalidade · Localização · Organização & Ordem · Ancestralidade · Cosmologia.

---

## Estado atual do vault (linha de base)

Total de fichas de conteúdo: **~236** — a grande maioria ainda em **esboço**. O conteúdo real hoje está concentrado nos rascunhos ([[Rascunho Geral]], [[Rascunho reinos]], [[Rascunho Regiões]]), no [[Resumão]], na [[Linha do Tempo]] e nos 4 arquivos de continentes.

| Categoria | Total | Esboços | Com conteúdo |
|---|---:|---:|---:|
| Ancestralidades | 10 | 10 | 0 |
| Culturas | 22 | 22 | 0 |
| Divindades | 27 | 27 | 0 |
| Ordens Religiosas | 4 | 4 | 0 |
| Reinos & Impérios | 84 | 77 | 7 |
| Personalidades | 27 | 27 | 0 |
| Localizações | 4 | 3 | 1 |
| Organizações | 2 | 2 | 0 |
| Cosmologia (Planos) | 4 | 3 | 1 |
| Astrologia (Corpos) | 5 | 4 | 1 |

> [!warning] Dívida de organização
> O melhor conteúdo vive em **rascunhos soltos**, não nas fichas oficiais, e quase não há wikilinks. As duas primeiras frentes de trabalho deveriam ser: (1) migrar rascunho → ficha oficial; (2) converter menções em **negrito** para `[[wikilinks]]`.

---

## Fios centrais do mundo (pilares do cânone)

Tudo que eu escrever deve ser coerente com estes pilares:

- **As cinco eras.** [[I - A Era das Lendas|Lendas]] → [[II - A Era dos Heróis|Heróis]] → [[III - A Era das Trevas|Trevas]] → [[IV - 1º Era|Primeira Era]] → [[V - 2º Era|Segunda Era]] (presente).
- **O Cataclisma** (EH 4475) partiu o mundo e derrubou os impérios antigos (Azurian, Korvandrin, Tarkisium).
- **Três luas.** [[Luna]] (benévola), [[Selene]] (rubra, vampiros), [[Mortemnis]] (presságios; seu retorno anuncia catástrofe). Plot atual: Mortemnis em rota de colisão, só atinge o mundo se ele for fragilizado.
- **Os Três Dragões** (vermelho/montanhas, verde/florestas, azul/magia) como mito fundador — ver [[Os Três Dragões]].
- **A imortalidade élfica perdida** com a morte da Árvore Mãe (Draknovir, EH 0).
- **Cinco continentes.** [[Aquilonia - Continente Oeste|Aquilonia]] · [[Auroria - Continente Leste|Auroria]] · [[Borealis - Continente Norte|Borealis]] · [[Sultaria - Continente Sul|Sultaria]] · [[Drakavir -  Abismo Draconiano|Drakavir]].
- **Grandes potências atuais:** [[Uria]] (expansionista/xenófoba), o **Conselho das Mercantilhas** (império comercial anônimo), [[Tarov]] vs [[Astarov]] (herdeiros de Taurin).

---

## Próximos passos propostos

1. ✅ Templates e sistema de status criados.
2. ⬜ Definir o **glossário canônico de nomes** (grafias oficiais: ex. *Arcádia* vs *Arcadia*, *Astarov* vs *Auristania*).
3. ⬜ Migrar rascunhos → fichas oficiais (categoria por categoria).
4. ⬜ Passe de wikilinks nas fichas que já têm conteúdo.
5. ⬜ Preencher esboços por prioridade combinada.
