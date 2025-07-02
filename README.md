# 📊 Projeto TelecomX_BR – Análise da Evasão de Clientes

Desenvolvido no contexto do desafio proposto pela plataforma Alura, este projeto tem como objetivo consolidar competências na área de Data Science.

---

## 📉 Apresentação

Este repositório apresenta uma análise detalhada do fenômeno de *churn* (evasão de clientes) na operadora fictícia **TelecomX**. A partir de dados históricos realistas, o estudo visa investigar padrões de cancelamento de serviço, oferecendo insights relevantes para decisões estratégicas e desenvolvimento de soluções orientadas por dados no contexto empresarial.

---

## 🔗 Acesso Interativo

- ▶️ **Acesse o notebook no Google Colab:**  
  [Abrir TelecomX_BR.ipynb no Google Colab](https://colab.research.google.com/drive/1YbHUvrP1sV9MTZMtkGN85w8XUOnnQ_H_?usp=drive_link)

---

## 🎯 Objetivo Geral e Objetivos Específicos

## Objetivo Geral

  O objetivo deste projeto é analisar os dados de cancelamento (churn) dos clientes da TelecomX,    identificando padrões que possam explicar os motivos da evasão. A partir disso, busca-se propor   soluções para reduzir esse comportamento, melhorando a retenção de clientes por meio de uma       análise de dados completa e orientada a decisões estratégicas.
  
## Objetivos Específicos

- Identificar os principais fatores associados ao cancelamento de serviços.
- Compreender o perfil dos clientes mais propensos à evasão.
- Apoiar a construção futura de modelos preditivos de churn.
- Apontar recomendações práticas com embasamento analítico.

---

## 📚 Tecnologias Utilizadas

- Python 3.10+
- Pandas, NumPy
- Matplotlib, Seaborn, Plotly
- Jupyter Notebook

---

## 📂 Estrutura do Repositório

```bash
├── TelecomX_BR.ipynb                        # Notebook principal com EDA e insights
├── telecomx_data_gold.csv                   # Dados tratados
├── requirements.txt                         # Dependências do projeto
└── README.md                                # Documentação do projeto
```

---

### Etapas Realizadas:

### 1. **Importação e Tratamento dos Dados**
- Os dados foram extraídos por meio de uma API, disponibilizados no formato JSON.  
- Realizou-se a normalização dos nomes das colunas e o ajuste adequado dos tipos de dados.  
- Ajuste de tipos de dados e tratamento de valores ausentes.  
- Foram adicionadas novas variáveis derivadas (features), como a métrica `Daily_Charges`.

### 2. **Exploração de Dados (EDA)**
- A variável `Churn`, utilizada como variável-alvo, foi analisada com foco em sua distribuição e impacto.  
- Foram produzidas visualizações para compreender o comportamento dos clientes com base em:
  - Categoria do contrato firmado  
  - Duração de permanência (`tenure`)  
  - Serviços utilizados  
  - Modalidade de pagamento  
  - Valor cobrado 
 
    ---

### 3. **Correlação entre Variáveis**

- Foram investigadas as associações entre os atributos do conjunto de dados e a variável `Churn`.  
- Utilizaram-se gráficos de dispersão e mapas de calor para visualizar o grau de correlação entre as variáveis.

---

## 📊 Dados Utilizados

O conjunto de dados utilizado contempla:

- Informações demográficas dos clientes
- Tipos de contrato e serviços contratados
- Dados de cobrança e método de pagamento
- Indicador de evasão final (`Churn`)

---

## 🔍 Descobertas e Insights

- Clientes com **contrato mensal** apresentam maior propensão ao churn.
- O **tempo de permanência (tenure)** está diretamente relacionado à fidelização.
- A **ausência de serviços como suporte técnico, backup e segurança online** está associada ao cancelamento.
- Clientes com **faturas diárias mais altas** demonstram maior risco de evasão.
- A **cobrança eletrônica (paperless billing)** também está relacionada a um maior nível de churn.

---

## ✅ Recomendações Estratégicas

Com base nos insights obtidos, estas são as principais recomendações para mitigar a evasão de clientes na TelecomX:

- **Incentivar a migração para contratos de longa duração** (anuais ou bienais), oferecendo bonificações como descontos progressivos, serviços adicionais gratuitos ou programas de fidelidade.
- **Aprimorar o onboarding de novos clientes**, com foco nos primeiros 3–6 meses, por meio de comunicação proativa, suporte técnico facilitado e monitoramento da satisfação.
- **Oferecer pacotes de serviços integrados** (como segurança online, backup e suporte premium) com maior valor percebido, promovendo cross-sell e aumentando o engajamento.
- **Auditar e otimizar a qualidade do serviço de internet**, especialmente para clientes de fibra óptica, atuando preventivamente sobre reclamações e problemas técnicos.
- **Desenvolver campanhas de retenção personalizadas**, com base na segmentação de clientes com maior risco de churn (ex.: contratos mensais, baixa permanência ou poucos serviços ativos).
- **Implantar um modelo preditivo de churn**, utilizando variáveis como tipo de contrato, tempo de permanência, valor cobrado e serviços contratados, para prever e agir proativamente sobre clientes em risco.
- **Executar testes A/B** para avaliar a eficácia das estratégias implementadas e realizar ajustes baseados em dados reais.
- **Coletar feedback contínuo** por meio de pesquisas de satisfação e canais de escuta ativa, ajustando as ações às necessidades reais dos clientes.
- **Avaliar o custo-benefício das ações de retenção**, garantindo retorno positivo sobre os investimentos realizados.

---

## 💡 Próximos Passos

A próxima etapa do projeto envolve aprofundar a análise e agregar mais valor com técnicas avançadas de Ciência de Dados e visualização:

- 📈 **Aplicar modelos preditivos** após o balanceamento da variável alvo `Churn`, com foco em melhorar a acurácia e a generalização dos modelos.
- 🔄 **Explorar técnicas de balanceamento**, como o **SMOTE** (Synthetic Minority Over-sampling Technique), além de **validação cruzada** para garantir a robustez dos resultados.
- 📊 **Construir dashboards interativos** para o acompanhamento contínuo das métricas de churn, facilitando a visualização e a tomada de decisão em tempo real por parte das áreas de negócio.

## 🧪 Como Reproduzir o Projeto

1. Clone o repositório:

```bash
git clone 
```

2. Crie e ative um ambiente virtual:

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate   # Windows
```

3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Execute o notebook:

```bash
jupyter notebook
```

---

## 👤 Autoria

Projeto desenvolvido por **Denise Cristine Brandão Leite**, como parte de sua formação em Data Science.

---

## 📄 Licença

Este projeto está licenciado sob os termos da licença MIT.
