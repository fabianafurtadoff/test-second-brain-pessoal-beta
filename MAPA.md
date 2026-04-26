# MAPA — Cérebro Pessoal de Fabiana Furtado

## Função

Ponto de entrada pra navegar este cérebro pessoal.

## Contexto

Este é o cérebro pessoal/individual de **Fabiana Furtado** — um por diretor (ou por cargo). É o workspace canônico do **OpenClaw pessoal** (Aria).

## Relação com os outros 2 cérebros

Se você é diretor da Aria Systems, tem acesso a 3 cérebros simultâneos:

| cérebro | propósito | branches | captura |
|---|---|---|---|
| `ariasystems-second-brain` | operacional do time (coletivo) | staging + main | via `/save` + `/team-sync` |
| `ariasystems-diretoria` | sensível da diretoria (coletivo) | staging + main (PR sempre) | via `/save` + `/team-sync` |
| **este** (pessoal) | só de Fabiana Furtado | só main | via `/save` (direto) + daily notes do agente |

## Estrutura

- `agentes/aria/` — agente pessoal (Aria) com config + daily notes em `memory/`
- `empresa/contexto/` — o que Fabiana Furtado sabe/lembra sobre a Aria Systems e contexto pro trabalho dele
- `empresa/skills/` — skills próprias do cérebro pessoal (inicializar-cerebro, save, team-sync)
- `empresa/rotinas/` — automações pessoais (se houver)

## Regras operacionais

- **Só Markdown e HTML.** Outros formatos ficam no Drive, referenciados com URL.
- **Captura explícita via `/save`** — nada sobe em tempo real.
- **`/team-sync`** distribui pros 2 cérebros coletivos com quiz.
- **Branch única: `main`.** Sem staging, sem PRs, sem consolidação noturna.
- **Pull + push periódicos** pelo OpenClaw pessoal (cron 15 min) — mantém sincronizado entre VPS e laptop.

---

*Cérebro pessoal — só o dono escreve. O que é coletivo vai pros outros 2 cérebros via `/team-sync`.*
