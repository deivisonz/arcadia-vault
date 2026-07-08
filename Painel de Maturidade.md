---
tags: [MOCs, sistema]
tipo: painel
---
# 🌡️ Painel de Maturidade do Cânone

Pipeline de status das fichas: **esboço → rascunho → revisão → cânone**. O símbolo **✦** (dentro das notas) marca conteúdo inventado a confirmar.

## Panorama (snapshot · 2E · 2026-07-07)
| Status | Fichas |
|---|---|
| esboço | 0 |
| rascunho | 375 |
| revisão | 35 |
| cânone | 2 |
| **Total (fichas de lore)** | **412** |

## 🔵 Em revisão (35)
- [[A Guerra Civil das Mercantilhas]]
- [[A Guerra Civil de Draukar]]
- [[A Guerra de Contenção]]
- [[A Invasão Uriana]]
- [[A Primeira Maré de Nihiloth]]
- [[A Queda de Draknovir]]
- [[A Revoada Draconiana]]
- [[Análise do Mapa]]
- [[Aquilonia - Continente Oeste]]
- [[Arquipélago de Hamada]]
- [[As Cadeiras]]
- [[Auroria - Continente Leste]]
- [[Borealis - Continente Norte]]
- [[Caçadores de Dragões]]
- [[Conselho das Brumas]]
- [[Culto aos Dragões]]
- [[Drakavir -  Abismo Draconiano]]
- [[Guilda dos Assassinos]]
- [[Guilda dos Ladrões]]
- [[Guilda dos Mercadores]]
- [[Igreja de Vohzro]]
- [[Nihiloth]]
- [[O Colapso de Taurin]]
- [[O Conflito dos Credos]]
- [[O Presente de Arcádia]]
- [[Ordem dos Silenciados]]
- [[Panteão Elfico]]
- [[Panteão Nordico]]
- [[Panteão Tiberico]]
- [[Sistema de Magia]]
- [[Sociedade dos Desbravadores]]
- [[Sultaria - Continente Sul]]
- [[Sylvanismo]]
- [[Terras Selvagens]]
- [[Vandria]]

## 🟢 Cânone — maduro (2)
- [[A Natureza do Divino]]
- [[Os Três Dragões]]

## 🟡 Em esboço — precisam virar rascunho (0)
- *(nenhuma)*

> [!tip] Como promover uma ficha
> Abra a ficha e mude o campo `status:` no topo (ex.: `rascunho` → `revisão` → `cânone`). Depois regenere este painel para atualizar o snapshot.

## Visão dinâmica (opcional — requer o plugin Dataview)
Com o plugin **Dataview** instalado, este bloco lista tudo automaticamente:

```dataview
TABLE status, tipo
WHERE status AND status != "cânone"
SORT status ASC, file.name ASC
```
