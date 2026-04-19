# 📘 MiniGuia Estudos: Análise Financeira com LLMs no NotebookLM
<div align="center">
  <img src="https://img.shields.io/badge/DIO-Project-blue?style=for-the-badge&logo=codecademy" alt="DIO Project">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License MIT">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status Completed">
</div>

<br>
> Projeto prático DIO: Aprendizagem Ativa com IA no NotebookLM  
> 👤 Por **Luckas Stephanio** | 
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
| 5 | For LLMs in the Financial Industry | 📄 PDF | Guia CFA Institute sobre IA no setor financeiro |
| 6 | HBR - Competing LLMs | 🌐 URL | Análise comparativa de modelos de linguagem |

> 💡 **Upload no NotebookLM**: Todas as fontes foram processadas e indexadas para consultas com grounding (citações verificáveis).

---

## ⚙️ Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Testei prompts no NotebookLM, refinando iterativamente para precisão. Registro das dificuldades e soluções:

| Etapa | Prompt Inicial (V1) | Variação Otimizada (V2) | Dificuldade Encontrada | Solução & Aprendizado |
|-------|---------------------|-------------------------|------------------------|------------------------|
| **#1 KPIs** | `"Liste os KPIs financeiros das fontes"` | `"Atue como analista FP&A sênior. Analise passo a passo: 1) 5 KPIs principais; 2) Benchmarks PMEs BR; 3) 3 riscos críticos; 4) Cite fontes."` | Resposta genérica, sem foco em PMEs brasileiras e sem citações numeradas. | Adicionei **persona**, **estrutura passo a passo** e **exigência de citação**. A IA passou a cruzar dados do Sebrae com PDFs técnicos. |
| **#2 Forecast** | `"Como fazer previsão de vendas para 2027?"` | `"Use raciocínio passo a passo: 1) Metodologias das fontes; 2) Fatores macro BR (Selic/IPCA); 3) Checklist PME; 4) % erro estimado; 5) Referencie."` | IA sugeriu métodos genéricos sem contexto real de pequena empresa. | Inseri **foco em PMEs**, **variáveis brasileiras** e **tabela de erro estimado**. Resultado virou guia acionável. |
| **#3 Glossário** | `"Crie um glossário financeiro"` | `"Glossário com 10 conceitos das fontes 1, 2 e 5. Para cada: 1 frase + exemplo em R$ + contexto PME. Máx: 3 linhas/termo."` | Respostas longas, teóricas e sem exemplos práticos em reais. | Adicionei **limite de linhas**, **exigência de exemplo em R$** e **foco em aplicação real**. |

> ✅ **Validação**: Testes de grounding confirmaram que a IA **não alucinou** - todas as citações [[1]][[2]] levam aos trechos corretos das fontes.

---

## 🎓 Miniguia de Estudo (Entrega Final)

### 📝 Resumos Estruturados

#### **1. KPIs Essenciais para PMEs Brasileiras**
Os 5 indicadores críticos identificados nas fontes:
- **EBITDA (LAJIDA)**: Principal indicador de geração de caixa operacional, mede lucro antes de juros/impostos/depreciação
- **ROE (Rentabilidade Patrimonial)**: Retorno sobre capital dos sócios (benchmark crise: queda de 8,7% para 4,16% na Duratex)
- **Ponto de Equilíbrio**: Faturamento mínimo em R$ para cobrir custos fixos e variáveis
- **Margem Líquida**: Eficiência final após todas as deduções (impostos, despesas financeiras)
- **Capital de Giro Líquido**: Solvência de curto prazo (ativos circulantes vs passivos)

**Riscos Principais**: Liquidez/inadimplência, volatilidade macroeconômica (IPCA/Selic), e atraso tecnológico sem supervisão humana em IA.

---

#### **2. Metodologias de Forecasting para 2027**
Abordagens identificadas para previsão de vendas:
- **Séries Temporais**: Dados históricos com ajuste de sazonalidade (erro: 5-10%)
- **Modelos Estatísticos (ARIMA/LSTM)**: Deep learning para dados sequenciais (erro: 3-7%)
- **Análise de Sentimento com LLMs**: IA filtra otimismo/pessimismo do mercado (erro: variável - alto risco de alucinação)
- **Análise de Contratos**: Receita recorrente com taxa de churn

**Fatores Macro BR**: IPCA/IGP-M (inflação), Selic/CDI (juros), câmbio BRL/USD, e PIB.

---

#### **3. LLMs em Análise Financeira**
- **Vantagem**: Superam humanos em processamento de relatórios extensos (300+ páginas em parágrafos acionáveis)
- **Aplicação**: Resumos de demonstrativos, análise de sentimento em notícias, automação de planilhas
- **Limitação**: Requer supervisão humana para evitar "alucinações" (dados inventados)
- **Melhor Prática**: Usar RAG (Retrieval-Augmented Generation) com fontes confiáveis e exigir citações

---

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

---

### 🔄 Prompts Reutilizáveis

Copie e adapte estes prompts para seus próprios estudos no NotebookLM:

#### **Prompt 1: Análise Rápida de KPIs**
