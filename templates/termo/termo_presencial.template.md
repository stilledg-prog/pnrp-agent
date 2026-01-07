# AUTO DE RECONHECIMENTO PESSOAL - PRESENCIAL

**Procedimento:** ${case.procedure_ref.type} ${case.procedure_ref.number}  
**Órgão/Unidade:** ${case.agency.name} — ${case.agency.unit}  
**Case ID:** ${case.case_id}  

**Data/Hora (início):** ${procedure.date_time.started_at}  
**Data/Hora (término):** ${procedure.date_time.ended_at}  
**Local:** ${procedure.location.type} — ${procedure.location.description}  
**Modo:** ${procedure.lineup_mode}  

---

## 1. QUALIFICAÇÃO DOS PARTICIPANTES (uso interno)
**Reconhecedor:** ${participants.recognizer.identity.display_name}  
**Reconhecido:** ${participants.subject.identity.display_name}  
**Condutor do ato:** ${participants.conductor.identity.display_name}  
**Defesa/Advogado (se presente):** ${participants.defense.identity.display_name}  

---

## 2. ENTREVISTA PRÉVIA (registro essencial)
**Entrevista prévia realizada:** ${pre_interview.was_conducted}  

**Descrição livre/espontânea:**  
${pre_interview.free_description.narrative}

**Condições de percepção:**  
- Tempo (s): ${pre_interview.visibility_conditions.time_seen_seconds}  
- Distância (m): ${pre_interview.visibility_conditions.distance_meters}  
- Iluminação: ${pre_interview.visibility_conditions.lighting}  
- Ângulo: ${pre_interview.visibility_conditions.angle}  
- Horário estimado: ${pre_interview.visibility_conditions.time_of_day}  

**Conhecimento prévio/exposição anterior:**  
- Já conhecia: ${pre_interview.prior_knowledge.knew_before}  
- Exposição anterior a imagens/informações: ${pre_interview.prior_knowledge.prior_image_exposure}  
- Detalhes: ${pre_interview.prior_knowledge.exposure_details}

---

## 3. INSTRUÇÕES FORMAIS AO RECONHECEDOR
Declara-se que o reconhecedor foi previamente informado de que:  
- o autor pode ou não estar presente;  
- não há obrigação de reconhecer;  
- a investigação prosseguirá;  
- o grau de certeza será registrado em suas palavras.

**Instruções prestadas:** ${instructions.delivered}

---

## 4. ALINHAMENTO E EXECUÇÃO
**Total de pessoas no alinhamento:** ${lineup.count_total}  
**Total de fillers:** ${lineup.count_fillers}  
**Show-up (apresentação isolada):** ${lineup.showup}  
**Variação de posicionamento:** ${lineup.positioning_varied}  

**Notas de semelhança/isonomia:**  
${lineup.composition_notes}

---

## 5. RESULTADO
**Resultado:** ${result.outcome}  
**Grau de certeza (declaração literal):**  
${result.certainty_statement}

**Posição reconhecida (se aplicável):** ${result.recognized_position}  
**Ausência de feedback sugestivo:** ${result.no_feedback_provided}

---

## 6. REGISTRO AUDIOVISUAL E CADEIA DE CUSTÓDIA
**Registro audiovisual integral:** ${evidence.video.exists}  
**Referência interna do vídeo:** ${evidence.video.storage_ref}  
**Hash (se disponível):** ${evidence.video.hash_sha256}

**Referência do pacote de alinhamento:** ${evidence.lineup_package.storage_ref}  
**Hash (se disponível):** ${evidence.lineup_package.hash_sha256}

---

## 7. ENCERRAMENTO
Por ser verdade, lavra-se o presente termo para fins de documentação do ato.

**Assinaturas (conforme rotina interna):**  
- Condutor: __________________________  
- Reconhecedor: _______________________  
- Defesa/Advogado (se presente): ________

---
${audit.software.agent_name} ${audit.software.agent_version} — ${audit.created_at}
