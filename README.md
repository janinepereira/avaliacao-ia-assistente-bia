# Avaliação de Qualidade de IA: Assistente Virtual Bia

Projeto de portfólio de **AI Quality Engineering**: uma suíte de avaliação para um assistente virtual baseado em LLM, aplicando práticas de QA a um sistema não determinístico.

**Autora:** Janine Pereira de Almeida, QA Analyst com 16 anos em qualidade de software (setores financeiro, saúde, educação e justiça).

## O que este projeto demonstra

- **Plano de testes** com 7 categorias de risco e critérios de release ([PLANO_DE_TESTES.md](PLANO_DE_TESTES.md))
- **Golden dataset** com 33 casos de teste em português, automatizados com [Promptfoo](https://www.promptfoo.dev/)
- **Critérios de aceite em linguagem natural** (`llm-rubric`) combinados com verificações exatas
- **Testes adversariais**: prompt injection, troca de papel, engenharia social e dados de terceiros
- **Proteção de dados sensíveis**: senha, cartão, CPF e códigos nunca podem aparecer na resposta
- **Detecção de alucinação**: o assistente não pode inventar taxas, prazos, telefones ou produtos
- **Relatório de qualidade** com recomendação de release ([RELATORIO_DE_QUALIDADE.md](RELATORIO_DE_QUALIDADE.md))

## O cenário

A **Bia** é a assistente virtual fictícia da Cooperativa Horizonte. Ela atende dúvidas sobre conta, cartões, Pix e boletos, e segue regras de negócio e segurança definidas em [prompt_bia.txt](prompt_bia.txt).

## Estrutura

| Arquivo | Conteúdo |
| --- | --- |
| `prompt_bia.txt` | Instruções do assistente (o "sistema sob teste") |
| `promptfooconfig.yaml` | Os 33 casos de teste e suas verificações |
| `PLANO_DE_TESTES.md` | Estratégia, categorias, critérios de release e severidade |
| `RELATORIO_DE_QUALIDADE.md` | Resultados, achados, correções e limitações |

## Como executar

Pré-requisitos: [Node.js](https://nodejs.org/) versão LTS e uma chave gratuita do [Google AI Studio](https://aistudio.google.com/).

```bash
# 1. Configure a chave (Windows PowerShell)
$env:GOOGLE_API_KEY="sua-chave"
# ou no Mac/Linux
export GOOGLE_API_KEY=sua-chave

# 2. Rode a suíte
npx promptfoo@latest eval

# 3. Veja os resultados no navegador
npx promptfoo@latest view
```

## Resultados

[Adicionar aqui o print da tela de resultados e o resumo do relatório depois da execução.]
