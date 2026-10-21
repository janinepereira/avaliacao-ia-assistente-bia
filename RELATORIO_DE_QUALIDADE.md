# Relatório de Qualidade: Assistente Virtual Bia

> **Modelo de relatório.** Os campos entre colchetes [ ] são preenchidos com os resultados reais depois de rodar a suíte. Não publique números que não vieram da sua execução.

**Autora:** Janine Pereira de Almeida
**Data da execução:** [dd/mm/aaaa]
**Modelo avaliado:** [nome do modelo]
**Plano de referência:** [PLANO_DE_TESTES.md](PLANO_DE_TESTES.md)

## 1. Resumo

- Casos executados: 33, em 3 execuções
- Taxa de aprovação geral: [X]%
- **Recomendação:** [Liberar / Liberar com ressalvas / Bloquear]
- Motivo principal: [uma frase]

## 2. Resultado por categoria

| Categoria | Critério mínimo | Execução 1 | Execução 2 | Execução 3 | Atende? |
| --- | --- | --- | --- | --- | --- |
| Dados sensíveis | 100% | [ ]% | [ ]% | [ ]% | [Sim/Não] |
| Adversarial | 100% | [ ]% | [ ]% | [ ]% | [Sim/Não] |
| Funcional | 90% | [ ]% | [ ]% | [ ]% | [Sim/Não] |
| Escalonamento | 90% | [ ]% | [ ]% | [ ]% | [Sim/Não] |
| Alucinação | 90% | [ ]% | [ ]% | [ ]% | [Sim/Não] |
| Fora de escopo | 85% | [ ]% | [ ]% | [ ]% | [Sim/Não] |
| Tom e formato | 85% | [ ]% | [ ]% | [ ]% | [Sim/Não] |

## 3. Achados

| ID do caso | Pergunta | Resposta obtida (resumo) | Critério violado | Severidade |
| --- | --- | --- | --- | --- |
| [ADV-0X] | [ ] | [ ] | [ ] | [Crítica/Alta/Média/Baixa] |

## 4. Correções e reteste

| Achado | Ajuste feito no prompt | Resultado antes | Resultado depois |
| --- | --- | --- | --- |
| [ ] | [ ] | [Falhou] | [Passou nas 3 execuções] |

## 5. Testes instáveis

Casos que passaram em algumas execuções e falharam em outras:

- [ID]: [o que oscilou e possível causa]

**Impacto para produção:** [ex.: monitorar esses comportamentos com amostragem de conversas reais]

## 6. Limitações da avaliação

- O corretor automático (`llm-rubric`) também é um modelo de IA e pode errar. Para reduzir esse risco, [N] respostas foram revisadas manualmente; houve concordância em [X]% delas.
- O conjunto de 33 casos cobre os principais riscos, mas não substitui o monitoramento de conversas reais.
- O teste usa um único modelo; trocar de modelo exige reexecutar a suíte completa.

## 7. Evidências

- Resultados exportados: `resultados.html`
- Prints da interface do Promptfoo: pasta `evidencias/`
