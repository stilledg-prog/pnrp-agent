# Protocol (PNRP) — conteúdo normativo-operacional

Este diretório contém os artefatos do protocolo:

- `rules.json` — repositório canônico das diretrizes e regras
- `indexes/generated/rules_ref_index.json` — índice de rastreabilidade (por regra e por asset)

## Convenções

- Cada regra deve possuir um `rule_id` estável (ex.: `PR-024`, `IA-001`) para rastreabilidade.
- Quando possível, assets devem referenciar regras via campos `rules_ref` (ex.: forms/checklists).
- Guides em Markdown podem manter rastreabilidade manual no índice caso não embutam `rule_id` no texto.

## Manutenção do índice

- O índice pode ser mantido manualmente (curadoria) ou gerado por varredura (best-effort):
```bash
python tools/build_rules_ref_index.py --repo-root .
```

Se o seu guia Markdown não contém `PR-xxx` no texto, a geração automática não terá como inferir o mapeamento.
