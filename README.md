# PNRP Agent (repositório público)

## Base normativa

Este repositório implementa, em nível conceitual e operacional, o **Protocolo Nacional de Reconhecimento de Pessoas**, instituído pela **Portaria do Ministério da Justiça e Segurança Pública nº 1122/2026**, incluindo suas diretrizes gerais, regras procedimentais e mecanismos de governança.

As disposições relativas ao uso de **Inteligência Artificial** observam, adicionalmente, a **Portaria MJSP nº 1080/2025**, especialmente o Capítulo de IA e o Anexo IV (Manual Técnico Simplificado).


## Objetivos

- Manter o **conteúdo do protocolo** (regras, guias, checklists e templates) consistente e rastreável
- Permitir validação automática via **schemas JSON**
- Facilitar revisão e uso interativo em chats que importem código (ex.: Gemini “Import code”)

## Estrutura

- `protocol/` — regras canônicas e índices de rastreabilidade
- `schemas/` — JSON Schemas (case, manifest, checklist_result, term_document, term_render_request, guide_bundle)
- `guides/` — guias operacionais (presencial, fotográfico, manual de IA)
- `checklists/` — checklist de avaliação
- `templates/` — formulários (`templates/forms`) e templates de termo (`templates/termo`)
- `tools/` — scripts (validate, render_term, build_rules_ref_index, validate_repo)
- `examples/` — casos de exemplo (sem PII)

## Segurança e PII (repositório público)

- **Nunca** coloque PII real no repositório (nome completo, CPF/RG, endereços, imagens/vídeos reais).
- Para documentos reais, utilize referências por `storage_ref` (cofre interno) e hashes quando aplicável.

## Uso rápido (runtime mínimo)

### 1) Instalar dependências
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### 2) Validar um JSON contra um schema
```bash
python tools/validate.py --schema schemas/recognition_case.schema.json examples/presencial/recognition_case.json
```

### 3) Renderizar termo a partir de `term_render_request.json`
```bash
python tools/render_term.py --request examples/presencial/term_render_request.json --out-dir artifacts/termo
```

## CI (GitHub Actions)

O workflow em `.github/workflows/ci.yml` executa `python tools/validate_repo.py` em push/PR para:
- impedir JSON inválido
- validar exemplos contra schemas
- bloquear lixo de macOS
- checar sintaxe dos scripts

## Licença

MIT (ver `LICENSE`). Ajuste conforme a política institucional antes de uso oficial.
