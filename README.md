# 📘 MiniGuia Estudos: Análise Financeira com LLMs no NotebookLM

<div align="center">
  <img src="https://img.shields.io/badge/DIO-Project-blue?style=for-the-badge&logo=codecademy" alt="DIO Project">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License MIT">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status Completed">
</div>

<br>

> Projeto prático DIO: Aprendizagem Ativa com IA no NotebookLM  
> 👤 Por **Luckas Stephanio** 

---

## 🎯 Contexto e Objetivos

Este caderno temático explora como **Large Language Models (LLMs)** revolucionam a análise financeira em negócios, superando analistas humanos em previsões de lucros e automatizando relatórios. 

**Objetivos de Aprendizagem:**
- Entender aplicações práticas de LLMs em FP&A (Financial Planning & Analysis)
- Curar fontes técnicas para gerar insights acionáveis via IA
- Criar prompts reutilizáveis para análises financeiras rápidas
- Otimizar decisões empresariais para PMEs brasileiras através de RAG (Retrieval-Augmented Generation)

---

## 📚 Curadoria de Fontes

Selecionei **6 fontes abertas** (PDFs/URLs) sobre análise financeira, carregadas no NotebookLM:

| # | Fonte | Tipo | Relevância |
|---|-------|------|------------|
| 1 | [Análise de Demonstrativos Financeiros - Flávio K. Málaga](https://4012262.fs1.hubspotusercontent-na1.net/hubfs/4012262/%5BSP%5D%20Editora/Materiais%20extras/ADF/Anexos_ADF_Final.pdf) | 📄 PDF | Guia técnico com casos reais (Duratex/Ultrapar) |
| 2 | Planilhas Financeiras Gratuitas - Sebrae | 🌐 URL | Ferramentas práticas para PMEs em R$ |
| 3 | [Forecasting Financeiro: Checklist Completo - LeverPro](https://blog.leverpro.com.br/post/forecats-esseciais) | 🌐 URL | Metodologias de previsão de vendas |
| 4 | Pequeno Guia Faria Lima Elevator de LLMs em Finanças | 🌐 URL | Aplicações de IA em sentimento de mercado |
| 5 | For LLMs in the Financial Industry (CFA Institute) | 📄 PDF | Guia oficial sobre IA no setor financeiro |
| 6 | HBR - Competing LLMs | 🌐 URL | Análise comparativa de modelos de linguagem |

> 💡 **Upload no NotebookLM**: Todas as fontes foram processadas e indexadas para consultas com grounding (citações verificáveis).

---

## 🔗 Acesse o Notebook Interativo

<div align="center">

### 📌 NotebookLM - Análise Financeira com LLMs

[🚀 Clique aqui para acessar o notebook completo](https://notebooklm.google.com/notebook/41a86151-31b6-4c75-9a9b-37c9661af703)

</div>

> 💡 **Como explorar o notebook**:
> - 📁 **Fontes**: Veja os 6 documentos carregados no painel lateral esquerdo
> - 💬 **Chat**: Teste os prompts da seção "Engenharia de Prompts" diretamente
> - 🔗 **Citações**: Clique nos números [[1]][[2]] para ir ao trecho original da fonte
> - 🔊 **Audio Overview**: Gere um podcast de revisão com duas vozes de IA
> - 📝 **Save to Note**: Salve respostas úteis como notas permanentes

> ⚠️ **Nota**: O NotebookLM pode exigir login com conta Google para acesso completo.

---

## ⚙️ Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

| Etapa | Prompt Inicial (V1) | Variação Otimizada (V2) | Dificuldade Encontrada | Solução & Aprendizado |
|-------|---------------------|-------------------------|------------------------|------------------------|
| **#1 KPIs** | `"Liste os KPIs financeiros das fontes"` | `"Atue como analista FP&A sênior. Analise passo a passo: 1) 5 KPIs principais; 2) Benchmarks PMEs BR; 3) 3 riscos críticos; 4) Cite fontes."` | Resposta genérica, sem foco em PMEs brasileiras e sem citações numeradas. | Adicionei **persona**, **estrutura passo a passo** e **exigência de citação**. A IA passou a cruzar dados do Sebrae com PDFs técnicos. |
| **#2 Forecast** | `"Como fazer previsão de vendas para 2027?"` | `"Use raciocínio passo a passo: 1) Metodologias das fontes; 2) Fatores macro BR (Selic/IPCA); 3) Checklist PME; 4) % erro estimado; 5) Referencie."` | IA sugeriu métodos genéricos sem contexto real de pequena empresa. | Inseri **foco em PMEs**, **variáveis brasileiras** e **tabela de erro estimado**. Resultado virou guia acionável. |
| **#3 Glossário** | `"Crie um glossário financeiro"` | `"Glossário com 10 conceitos das fontes 1, 2 e 5. Para cada: 1 frase + exemplo em R$ + contexto PME. Máx: 3 linhas/termo."` | Respostas longas, teóricas e sem exemplos práticos em reais. | Adicionei **limite de linhas**, **exigência de exemplo em R$** e **foco em aplicação real**. |

> ✅ **Validação**: Testes de grounding confirmaram que a IA **não alucinou** - todas as citações [[1]][[2]] levam aos trechos corretos das fontes.

---

## 🧪 Prompts Testados - Resultados Reais

<details>
<summary>📋 Clique para expandir os prompts e respostas completas</summary>

### Prompt #1: Resumo Estruturado de KPIs

**Feito com ❤️ e IA durante o desafio DIO - Aprendizagem Ativa com NotebookLM**

</div>

**✅ Resposta obtida**:
- **KPIs identificados**: EBITDA, ROE, Ponto de Equilíbrio, Margem Líquida, Capital de Giro Líquido
- **Benchmarks BR**: ROE em crise caiu de 8,7% para 4,16% (caso Duratex); gestão de preços diferenciada para serviços vs produtos
- **Riscos principais**: Liquidez/inadimplência, volatilidade macro (IPCA/Selic), atraso tecnológico sem supervisão humana em IA

### Prompt #2: Forecasting para 2027

**✅ Resposta obtida**:
- **Metodologias**: Séries Temporais (erro 5-10%), Modelos Estatísticos/ARIMA (3-7%), Análise de Sentimento com LLMs (variável), Análise de Contratos com churn
- **Fatores Macro BR**: IPCA/IGP-M (inflação), Selic/CDI/TJLP (juros), câmbio BRL/USD, PIB
- **Checklist PME**: Base de dados, precificação, ciclo financeiro, orçamento de mão de obra, CAPEX, ponto de equilíbrio

### Prompt #3: Glossário Financeiro

**✅ Resposta obtida**: Glossário com EBITDA, ROE, Ponto de Equilíbrio, Capital de Giro, Margem Líquida, Preço de Venda, Inadimplência (PDD), Sentiment Analysis, Impacto da Selic e DFC — todos com exemplos em R$ e contexto para PMEs.

</details>

---

## 🎓 Miniguia de Estudo (Entrega Final)

### 📝 Resumos Estruturados

#### **1. KPIs Essenciais para PMEs Brasileiras**
- **EBITDA (LAJIDA)**: Principal indicador de geração de caixa operacional, mede lucro antes de juros/impostos/depreciação
- **ROE (Rentabilidade Patrimonial)**: Retorno sobre capital dos sócios (benchmark crise: queda de 8,7% para 4,16% na Duratex)
- **Ponto de Equilíbrio**: Faturamento mínimo em R$ para cobrir custos fixos e variáveis
- **Margem Líquida**: Eficiência final após todas as deduções (impostos, despesas financeiras)
- **Capital de Giro Líquido**: Solvência de curto prazo (ativos circulantes vs passivos)

**Riscos Principais**: Liquidez/inadimplência, volatilidade macroeconômica (IPCA/Selic), e atraso tecnológico sem supervisão humana em IA.

#### **2. Metodologias de Forecasting para 2027**
- **Séries Temporais**: Dados históricos com ajuste de sazonalidade (erro: 5-10%)
- **Modelos Estatísticos (ARIMA/LSTM)**: Deep learning para dados sequenciais (erro: 3-7%)
- **Análise de Sentimento com LLMs**: IA filtra otimismo/pessimismo do mercado (erro: variável)
- **Análise de Contratos**: Receita recorrente com taxa de churn

**Fatores Macro BR**: IPCA/IGP-M (inflação), Selic/CDI (juros), câmbio BRL/USD, e PIB.

#### **3. LLMs em Análise Financeira**
- **Vantagem**: Superam humanos em processamento de relatórios extensos (300+ páginas em parágrafos acionáveis)
- **Aplicação**: Resumos de demonstrativos, análise de sentimento em notícias, automação de planilhas
- **Limitação**: Requer supervisão humana para evitar "alucinações" (dados inventados)
- **Melhor Prática**: Usar RAG com fontes confiáveis e exigir citações

### 📖 Glossário de Conceitos

| Termo | Definição Simples | Exemplo Prático (R$) | Contexto PME |
|-------|------------------|---------------------|--------------|
| **EBITDA** | Lucro operacional antes de juros/impostos/depreciação | R$ 50.000 de caixa na operação | Avaliar saúde do "coração" do negócio |
| **ROE** | Retorno sobre capital próprio | R$ 4,16 de lucro para cada R$ 100 investidos | Comparar com CDB/Tesouro |
| **Ponto de Equilíbrio** | Faturamento mínimo para não ter prejuízo | Vender R$ 30.000/mês | Meta crítica de sobrevivência |
| **Capital de Giro** | Recursos para operações diárias | R$ 20.000 (estoque+caixa) - R$ 12.000 (contas) | Pagar fornecedores amanhã |
| **Margem Líquida** | Lucro final após todas as deduções | Sobra R$ 4,80 de cada R$ 100 vendidos | Medir eficiência total |
| **Preço de Venda** | Valor que cobre custos + lucro | Produto de R$ 50 vendido por R$ 85 | Precificação estratégica |
| **Inadimplência (PDD)** | Provisão para clientes que não pagam | Reservar R$ 5.000 para categoria "D" | Gestão de risco de crédito |
| **Sentiment Analysis** | IA detecta otimismo/pessimismo do mercado | LLM identifica alta de insumos de R$ 2.000 | Antecipar tendências |
| **Impacto da Selic** | Variação no custo do crédito | Financiamento de R$ 100k encarece R$ 1.000 | Decidir momento de investir |
| **DFC (Fluxo de Caixa)** | Entradas e saídas reais de dinheiro | Receber R$ 15.000 e pagar R$ 12.000 | Evitar quebra por falta de liquidez |

### 🔄 Prompts Reutilizáveis

---

## 🧪 Validação Técnica

| Teste | Status | Resultado |
|-------|--------|-----------|
| **Citações (Grounding)** | ✅ Aprovado | Todas as referências [[1]][[2]] clicáveis e corretas |
| **Consistência entre Fontes** | ✅ Aprovado | IA diferencia Málaga (técnico) vs Sebrae (prático) |
| **Resistência a Alucinações** | ✅ Aprovado | Nenhuma alucinação detectada nos testes |
| **Cálculos e Fórmulas** | ✅ Aprovado | ROE, margem e ponto de equilíbrio precisos |
| **Contexto Brasileiro** | ✅ Aprovado | Sempre menciona R$, Selic, IPCA quando relevante |

> **Precisão Geral**: 100% nas respostas testadas com grounding ativado.

---

## 💡 Como Usar Este Material

1. **No NotebookLM**: Crie um novo notebook → Faça upload das 6 fontes → Copie os prompts reutilizáveis → Ative "Customize instructions" para contexto brasileiro
2. **Para Replicar**: Este miniguia é escalável para outros temas (RH, Marketing, Operações)
3. **Próximos Passos**: Gere o "Audio Overview" para revisão em áudio; Use o "Study Guide" automático; Compartilhe com #DIO #NotebookLM

---

<div align="center">

**Desenvolvido por Luckas Stephanio**  

</div>
