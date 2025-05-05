# Chat_bot_IA_Desafio_inovacao_2025
Bot de trading com IA para o VIII Desafio em Ciência de Dados - Investe.AI - JCPOLI 2025.
# Investe.AI - Bot de Trading com Aprendizado por Reforço

Bot de trading automatizado desenvolvido para o VIII Desafio em Ciência de Dados - JCPOLI 2025.

## 🔍 Visão Geral

Este projeto implementa um sistema de trading automatizado baseado em técnicas de Inteligência Artificial para operação em ambiente simulado de bolsa. O sistema utiliza:

- Aprendizado por Reforço (RL) para tomada de decisões de investimento
- Análise de dados financeiros e indicadores técnicos
- Processamento de linguagem natural para análise de notícias
- Backtesting rigoroso para validação das estratégias

## 👥 Equipe: Data Investor´s

- Robson Porto Rasmussen - Engenharia de Computação
- Marney Samuell Araújo Valente Freitas - Engenharia de controle e automação
- Jacion Antônio da Silva - Ciência de Dados
- Bruna Maria Grazielli Anapaz de Souza - Engenharia de produção

## 📂 Estrutura do Projeto

```
Chat_bot_IA_Desafio_inovacao_2025/
├── dados/                     # Dados brutos e processados
├── notebooks/                 # Jupyter notebooks para análises
├── codigo_principal/          # Código fonte do sistema
├── modelos_treinados/         # Modelos salvos
├── interface/                 # Interface Streamlit
├── testes/                    # Testes unitários
└── documentacao/              # Documentação
```

## 📊 Dataset

Nosso modelo utiliza dados de séries temporais do mercado financeiro obtidos através da API do Yahoo Finance. Incluímos:

- Dados históricos de preços (OHLCV)
- Indicadores técnicos derivados
- Dados fundamentalistas
- Análise de sentimento de notícias (via API)

Todos os dados estão disponíveis na pasta `dados/` com séries históricas até 31/12/2024, conforme exigido no edital.

## 🤖 Componentes Principais

### 1. Coleta e Processamento de Dados
Implementamos pipelines automatizados para coleta de dados financeiros de fontes públicas, incluindo pré-processamento, normalização e feature engineering.

### 2. Modelagem de Predições
Utilizamos uma combinação de modelos de séries temporais e aprendizado profundo para estimar distribuições de retornos futuros.

### 3. Agente de Aprendizado por Reforço
Nosso agente é treinado usando o algoritmo [nome do algoritmo RL] para otimizar decisões de trading (comprar, vender, manter) com base nas previsões de mercado.

### 4. Sistema de Backtesting
Framework rigoroso para simular operações em dados históricos, incluindo custos de transação realistas e controle de risco.

### 5. Interface de Visualização
Dashboard interativo em Streamlit para acompanhamento de desempenho e análise de decisões do bot.

## 🔧 Instalação e Configuração

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/Chat_bot_IA_Desafio_inovacao_2025.git
cd Chat_bot_IA_Desafio_inovacao_2025

# Configurar ambiente virtual
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate

# Instalar dependências
pip install -r requirements.txt

# Executar o dashboard
streamlit run app/main.py
```

## 📈 Métricas de Avaliação

Avaliamos nosso bot com as seguintes métricas:

- Retorno Total: Lucro acumulado no período de teste
- Índice Sharpe: Retorno ajustado ao risco
- Taxa de Acerto: Percentual de operações vencedoras
- Drawdown Máximo: Queda máxima do patrimônio
- Métricas por Decisão: Taxa de acerto específica para compras, vendas e manutenções

## 🔄 Reproducibilidade

Para garantir resultados reproduzíveis, fixamos as seguintes seeds:

```python
# Seeds para reproducibilidade
RANDOM_SEED = 42
np.random.seed(RANDOM_SEED)
tf.random.set_seed(RANDOM_SEED)
torch.manual_seed(RANDOM_SEED)
```


## 🔗 Links Úteis

- Documentação do edital:(https://congressos.pucgoias.edu.br/iv-jornada-cientifica-da-escola-politecnica-e-de-artes)
- Trello do projeto:(https://trello.com/b/Tgk4YwNA/viii-desafio-em-ciencias-de-dados-investeia-seu-bot-sua-solucao-sua-estrategia)
- Colab do projeto: (https://colab.research.google.com/drive/1Gf0mQXns7cyPqCAYKdrfaNRmXE3Dt4c5?usp=sharing&authuser=1#scrollTo=i50lSKb-cvH1)
