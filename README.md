# 📊 Análise Exploratória de Dados Socioeconômicos — PNAD Contínua (IBGE)

🔗 **Notebook principal:** [EDA PNAD Contínua — Desemprego](./notebooks/eda_pnad_continua_desemprego_ibge.ipynb)

---

Projeto de **Análise Exploratória de Dados (EDA)** com foco no **mercado de trabalho brasileiro**, utilizando dados oficiais da **PNAD Contínua**, disponibilizados pelo **IBGE** via **API SIDRA**.

O projeto aplica práticas sólidas de **engenharia de dados leve, estatística descritiva e visualização analítica**, convertendo dados brutos em **insights interpretáveis**, com rigor metodológico e clareza na comunicação — alinhado ao workflow esperado de um **Cientista de Dados**.

---

## 🎯 Objetivos do Projeto (EDA)

Este projeto tem como objetivo realizar uma **Análise Exploratória de Dados (EDA)** aplicada ao mercado de trabalho brasileiro, buscando:

- Compreender a **estrutura, granularidade e limitações** dos dados da PNAD Contínua
- Avaliar a **qualidade e consistência** das séries temporais
- Identificar **tendências de longo prazo**, ciclos econômicos e **pontos de inflexão**
- Investigar **padrões sazonais trimestrais** na taxa de desocupação
- Detectar **outliers e períodos atípicos**, associados a choques econômicos
- Explorar **relações estatísticas** entre indicadores derivados da taxa de desocupação
- Aplicar técnicas de **suavização temporal** para redução de ruído
- Gerar **insights e hipóteses analíticas** que possam subsidiar análises preditivas ou inferenciais futuras

---

## 🗂️ Estrutura do Projeto
```
📁 projeto/
│
├── 📓 notebook_principal.ipynb # Pipeline completo de EDA
├── 📊 dados/ # Dados extraídos via API SIDRA
└── 📄 README.md # Documentação técnica do projeto
```

---

## 🔄 Pipeline Analítico

### 1️⃣ Coleta de Dados

- Consumo da **API SIDRA/IBGE**
- Base utilizada: **PNAD Contínua – Taxas e Níveis (Tabela 6468)**
- Conversão e estruturação dos dados em `DataFrame` utilizando `pandas`

### 2️⃣ Limpeza e Preparação

- Renomeação semântica de variáveis
- Construção de **índice temporal trimestral**
- Padronização de categorias e rótulos
- Criação de variáveis auxiliares para análise estatística

### 3️⃣ Análise Exploratória e Visualização

- Séries temporais com **média** e **mediana**
- **Boxplots** para avaliação de distribuição e outliers
- **Matriz de correlação** entre variáveis
- **Média móvel de 4 trimestres** para suavização de tendências
- Análise **sazonal por trimestre do ano**

---

## 💡 Principais Insights Analíticos

- Identificação de **períodos críticos** do mercado de trabalho:
  - 📉 Crise econômica (2015–2016)
  - 🦠 Impactos da pandemia (2020–2021)

- Evidência estatística de **sazonalidade**:
  - Primeiro trimestre historicamente mais fraco
  - Recuperação progressiva ao longo do ano

- Separação clara entre:
  - Indicadores de **curto prazo** (variações trimestrais)
  - Indicadores **estruturais** (variações anuais)

- O **coeficiente de variação** é interpretado como métrica metodológica de dispersão, não como indicador econômico direto

---

## 📈 Resultados Relevantes

- O mercado de trabalho brasileiro apresentou **ciclos prolongados de deterioração**, especialmente entre 2016 e 2021
- A média móvel evidenciou **pontos de inflexão** e persistência das crises
- A análise sazonal confirmou padrões recorrentes de início de ano mais fraco
- As correlações reforçam o papel das variações como indicadores:
  - **Antecedentes**
  - **Confirmatórios** da taxa de desocupação

---

## 🛠️ Stack Tecnológica

- **Python**
- **Pandas** | **NumPy**
- **Matplotlib** | **Seaborn**
- **API SIDRA (IBGE)**
- **Jupyter Notebook**

---

## 📎 Contexto Profissional

Este projeto demonstra competências fundamentais para **Ciência de Dados**, incluindo:

- Manipulação e estruturação de dados reais
- Análise estatística aplicada
- Pensamento analítico orientado a dados socioeconômicos
- Comunicação visual clara e interpretável para tomada de decisão

## ▶️ Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/andrewsantosfraga/eda-unemployment-data.git

2. Crie e ative um ambiente virtual (opcional, mas recomendado):

python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\\Scripts\\activate   # Windows

3. Instale as dependências:

pip install -r requirements.txt

4. Execute o notebook:

eda_labor_market_pnad_continua_ibge.ipynb
---

📬 **Feedbacks, sugestões e conexões profissionais são bem-vindos.**