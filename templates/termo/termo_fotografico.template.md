# AUTO DE RECONHECIMENTO FOTOGRÁFICO

**Procedimento:** ${case.procedure_ref.type} ${case.procedure_ref.number}  
**Órgão/Unidade:** ${case.agency.name} — ${case.agency.unit}  
**Case ID:** ${case.case_id}  

**Data/Hora (início):** ${procedure.date_time.started_at}  
**Data/Hora (término):** ${procedure.date_time.ended_at}  
**Local:** ${procedure.location.type} — ${procedure.location.description}  
**Modo:** ${procedure.lineup_mode}  

---

## 1. JUSTIFICATIVA DA MODALIDADE FOTOGRÁFICA
**Justificativa formal (impossibilidade do presencial):**  
${procedure.justification.photo_modality_reason}

---

## 2. QUALIFICAÇÃO DOS PARTICIPANTES (uso interno)
**Reconhecedor:** ${participants.recognizer.identity.display_name}  
**Reconhecido:** ${participants.subject.identity.display_name}  
**Condutor do ato:** ${participants.conductor.identity.display_name}  
**Defesa/Advogado (se presente):** ${participants.defense.identity.display_name}  

---

## 3. ENTREVISTA PRÉVIA (registro essencial)
**Entrevista prévia realizada:** ${pre_interview.was_conducted}  

**Descrição livre/espontânea:**  
${pre_interview.free_description.narrative}

---

## 4. INSTRUÇÕES FORMAIS AO RECONHECEDOR
Declara-se que o reconhecedor foi previamente informado de que:  
- o autor pode ou não estar entre as imagens;  
- não há obrigação de reconhecer;  
- a investigação prosseguirá;  
- o grau de certeza será registrado em suas palavras.

**Instruções prestadas:** ${instructions.delivered}

---

## 5. COMPOSIÇÃO DO ALINHAMENTO FOTOGRÁFICO
**Total de imagens no alinhamento:** ${lineup.count_total}  
**Total de fillers:** ${lineup.count_fillers}  
**Show-up (imagem isolada):** ${lineup.showup}

**Isonomia técnica/visual (declaração):**  
- Iluminação: ${lineup.photographic.iso_visual.lighting}  
- Fundo: ${lineup.photographic.iso_visual.background}  
- Resolução/qualidade: ${lineup.photographic.iso_visual.resolution}  
- Enquadramento (rosto+busto): ${lineup.photographic.iso_visual.crop}  
- Ausência de identificadores (texto/uniforme/logomarca/número): ${lineup.photographic.iso_visual.no_identifiers}

**Notas de semelhança/isonomia:**  
${lineup.composition_notes}

---

## 6. USO DE IA (quando aplicável)
**Uso de IA:** ${lineup.photographic.ai.used}  
**Ferramenta:** ${lineup.photographic.ai.tool}  
**Justificativa:** ${lineup.photographic.ai.justification}  
**Foto do reconhecido padronizada:** ${lineup.photographic.ai.subject_photo_standardized}  
**Lote/Referência interna de geração:** ${lineup.photographic.ai.generated_assets_ref}

---

## 7. RESULTADO
**Resultado:** ${result.outcome}  
**Imagem reconhecida (ID, se aplicável):** ${result.recognized_item_id}  
**Grau de certeza (declaração literal):**  
${result.certainty_statement}

---

## 8. REGISTRO AUDIOVISUAL E CADEIA DE CUSTÓDIA
**Registro audiovisual integral:** ${evidence.video.exists}  
**Referência interna do vídeo:** ${evidence.video.storage_ref}  
**Hash (se disponível):** ${evidence.video.hash_sha256}

**Pacote do alinhamento (imagens + metadados):** ${evidence.lineup_package.storage_ref}  
**Hash (se disponível):** ${evidence.lineup_package.hash_sha256}

---

## 9. ENCERRAMENTO
Por ser verdade, lavra-se o presente termo para fins de documentação do ato.

**Assinaturas (conforme rotina interna):**  
- Condutor: __________________________  
- Reconhecedor: _______________________  
- Defesa/Advogado (se presente): ________

---
${audit.software.agent_name} ${audit.software.agent_version} — ${audit.created_at}
