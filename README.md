# DepFixAgent: Correção Automatizada de APIs Depreciadas com LLMs e Agentes Inteligentes

## Visão Geral

Este projeto investiga e propõe melhorias no uso de **Modelos de Linguagem de Grande Escala (LLMs)** para lidar com **APIs depreciadas** em código gerado automaticamente. Ele é inspirado e baseado no artigo _"LLMs Meet Library Evolution: Evaluating Deprecated API Usage in LLM-based Code Completion"_.

Nosso foco é explorar o uso de **agentes inteligentes** aliados a LLMs de última geração (como GPT-4o, Claude 3.5, etc.) para detectar e corrigir automaticamente APIs obsoletas, mantendo a funcionalidade do código e incorporando conhecimento atualizado de bibliotecas externas.

## Escopo

O projeto propõe:

- Utilizar **LLMs recentes** para gerar código mais preciso e resiliente a mudanças em bibliotecas;
- Implementar agentes que **consultam fontes externas** (como documentação oficial) para auxiliar na correção;
- Comparar os resultados com abordagens conhecidas, como `REPLACEAPI` e `INSERTPROMPT`;
- Automatizar a **validação semântica e sintática** das correções via ferramentas como `mypy`, `pyright` ou `pytest`.

## Experimentos

Os experimentos avaliam:

- Taxa de uso de APIs depreciadas por diferentes LLMs;
- Taxa de correções bem-sucedidas;
- Similaridade semântica entre o código original e o corrigido;
- ⚠Introdução (ou não) de novos erros.

Comparações serão feitas entre:
- **Método A**: LLM + código bruto gerado;
- **Método B**: LLM + reparo com REPLACEAPI/INSERTPROMPT;
- **Método C**: LLM + Agente Autônomo com consulta externa.

## 🛠Requisitos

- Python 3.10+
- Transformers (HuggingFace)
- LangChain ou AutoGen (para agentes)
- OpenAI API / Anthropic API
- Ferramentas de análise: `black`, `flake8`, `mypy`, `pyright`

## Equipe

- João Pedro Felix da Silva (jpfs2)
- Gabriel Henrique Vasconcelos (ghv)
- Almir Alves (aasc)
- Erbert Bernardino Gadelha Rocha (ebgr)

---

> Este projeto faz parte da disciplina de TAES, com o objetivo de investigar contribuições práticas da IA generativa para atividades do ciclo de vida do software.

