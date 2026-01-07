# Manual Técnico — Uso de IA na Composição de Imagens (Reconhecimento Fotográfico)
Base: Portaria MJSP nº 1080/2025 — Capítulo de IA + Anexo IV (Manual Técnico Simplificado).

## 1) Escopo e finalidade do uso de IA
É admitido o uso de IA para gerar imagens destinadas à composição de alinhamentos fotográficos, observadas as diretrizes do Protocolo.:contentReference[oaicite:52]{index=52}
Finalidades típicas:
- garantir uniformidade estética e técnica;
- evitar exposição indevida de terceiros;
- ampliar variedade de perfis sem recorrer a bancos sensíveis;
- padronizar o procedimento e reduzir risco de indução;
- reduzir influência de vieses cognitivos do reconhecedor.:contentReference[oaicite:53]{index=53}

## 2) Requisitos para utilização
- O uso de IA deve ser **formalmente justificado** (carência de meios e/ou padronização, segurança e proteção de terceiros, entre outros).:contentReference[oaicite:54]{index=54}
- A ferramenta deve permitir **customização paramétrica** de elementos faciais e fenotípicos.:contentReference[oaicite:55]{index=55}
- As imagens geradas devem simular fotografias reais de pessoas fictícias semelhantes, com uniformidade de qualidade.:contentReference[oaicite:56]{index=56}

## 3) Parâmetros técnicos obrigatórios (padrão mínimo)
As imagens por IA devem observar padrões homogêneos de:
- resolução, enquadramento, iluminação, fundo neutro e posição frontal; e
- variações de fenótipo coerentes com a descrição prévia, para diversidade e redução de sugestões involuntárias.:contentReference[oaicite:57]{index=57}

Conforme Anexo IV (padrões de geração):
- enquadramento: rosto e busto (altura dos ombros), posição frontal;
- fundo: neutro, claro, sem texturas/elementos de destaque;
- iluminação: difusa, sem sombras marcadas/reflexos irregulares;
- expressão: neutra, olhos abertos voltados à câmera (se possível);
- vestuário: preferir o possivelmente usado no fato; se inviável, camiseta/camisa lisa sem caracteres;
- escala facial harmonizada entre todas as imagens;
- diversidade fenotípica dentro dos parâmetros descritos pelo reconhecedor.:contentReference[oaicite:58]{index=58}

## 4) Procedimento recomendado (pipeline operacional)
### 4.1 Preparação da foto do reconhecido (quando for usada junto com IA)
A fotografia real do reconhecido pode ser previamente ajustada para equiparação:
- corrigir iluminação, nitidez, contraste, enquadramento e fundo;
- padronizar escala facial, posição do olhar e plano de corte (ombros/busto);
- eliminar elementos distintivos (vestuário incomum, fundo institucional, objetos).:contentReference[oaicite:59]{index=59}

### 4.2 Geração e controle de qualidade
Boas práticas e etapas técnicas:
- configurar uniformidade de enquadramento, iluminação, fundo e resolução;
- eliminar imagens com distorções/artefatos/inconsistências e repetir geração se necessário;
- salvar em formato sem compressão (ex.: PNG/TIFF) para rastreabilidade;
- evitar repetições de padrões faciais idênticos;
- garantir diversidade (tons de pele/traços) sem criar destaque para o reconhecido;
- realizar testes prévios do alinhamento para verificar homogeneidade.:contentReference[oaicite:60]{index=60}:contentReference[oaicite:61]{index=61}

### 4.3 Registro e rastreabilidade (obrigatório)
A autoridade responsável deve:
- registrar formalmente o uso de IA (ferramentas, parâmetros, justificativa);
- manter arquivada a base de imagens e todos os arquivos gerados, para controle/defesa;
- juntar ao procedimento investigatório as imagens utilizadas, garantindo acesso integral e possibilidade de perícia/auditoria técnica.:contentReference[oaicite:62]{index=62}:contentReference[oaicite:63]{index=63}

## 5) Vedações específicas (IA)
- É vedada inserção de elementos gráficos, símbolos ou objetos nas imagens.:contentReference[oaicite:64]{index=64}
- Não se admite uso de imagens extraídas de redes sociais, bancos de suspeitos ou registros pessoais sem consentimento ou controle legal da fonte.:contentReference[oaicite:65]{index=65}
- O conjunto não pode conter diferenças visuais que realcem/singularizem o retrato do reconhecido (sem “destaque involuntário”).:contentReference[oaicite:66]{index=66}

## 6) Regras protetivas — Crianças e adolescentes
- Em reconhecimento fotográfico de adolescentes como supostos autores de ato infracional, **somente** são admitidas imagens geradas por IA, sendo **vedada** a utilização de fotografias reais de crianças/adolescentes.:contentReference[oaicite:67]{index=67}
- O ato deve evitar indução/pressão e ser integralmente gravado; aplicar regras específicas quando envolver criança/adolescente como vítima/testemunha (Lei 13.431/2017).:contentReference[oaicite:68]{index=68}

## 7) Segurança da informação e governança tecnológica
- Soluções de TI e ferramentas de reconhecimento automatizado devem observar diretrizes de Portaria MJSP nº 961/2025; instituições devem garantir mecanismos de segurança, rastreabilidade, auditabilidade, integridade e confidencialidade, conforme legislação de proteção de dados e normas do MJSP.:contentReference[oaicite:69]{index=69}

## 8) Entregáveis mínimos (para o repositório e para auditoria)
Para cada alinhamento com IA, manter (fora do GitHub público; referenciar no manifest):
- parâmetros/prompt/configuração;
- ferramenta/modelo e versão;
- data, responsável, unidade;
- lote de imagens geradas + seleção final (sem compressão);
- pacote do alinhamento (imagens + metadados) e referência de armazenamento;
- termo circunstanciado e registro audiovisual do ato;
- checklist preenchido (Anexo V).:contentReference[oaicite:70]{index=70}:contentReference[oaicite:71]{index=71}
