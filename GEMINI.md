# GEMINI.md — guia para uso interativo (Import code)

## Contexto
Este repositório implementa um “núcleo” do PNRP:
- regras (`protocol/rules.json`)
- schemas (`schemas/*.schema.json`)
- guias (`guides/*.md`)
- checklists e formulários
- templates de termo e runtime mínimo (`tools/`)

## Restrições (repositório público)
- Não gerar nem solicitar PII real.
- Em exemplos, usar `pii_level: REDACTED` e nomes genéricos.

## Fluxo padrão (happy path)
1. Validar `recognition_case.json` contra `schemas/recognition_case.schema.json`
2. Validar `procedure_manifest.json` contra `schemas/procedure_manifest.schema.json`
3. Validar `term_render_request.json` contra `schemas/term_render_request.schema.json`
4. Renderizar termo com `tools/render_term.py`
5. Validar `term_document.json` contra `schemas/term_document.schema.json`
6. (Opcional) Atualizar manifest com hashes/artefatos

## Onde olhar primeiro
- `README.md` (raiz)
- `examples/` (casos sanitizados)
- `tools/validate_repo.py` (checks do CI)
