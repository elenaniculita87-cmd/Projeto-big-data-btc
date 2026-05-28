Projeto de Big Data: Previsão de Mercado Financeiro com PySpark

Este projeto foi desenvolvido no âmbito da Unidade Curricular de Processamento de Big Data da Pós-Graduação em Data Science do ISLA Santarém. O objetivo principal é a implementação de um pipeline de Machine Learning escalável, utilizando o ecossistema Apache Spark para prever a direção dos retornos do Bitcoin (BTC/USDT).

🚀 Objetivo
Implementar um pipeline end-to-end que inclui:

Ingestão e ETL: Organização dos dados segundo a arquitetura Medallion (Bronze, Silver, Gold).

Engenharia de Features: Criação de indicadores técnicos (RSI, MACD, Médias Móveis).

Machine Learning: Aplicação de redução de dimensionalidade (PCA) e modelagem preditiva com pyspark.ml (Regressão e Classificação).

👥 Elementos do Grupo:
Elena Bobil - a22502168 
João Paulo Francisco - a22510741 


🏗️ Estrutura do Projeto
btc_04h_usdt_binance.parquet: Dataset utilizado.
Projeto_de_Big_Data.ipynb: Notebook principal com o código e a análise científica.
README.md: Documentação do projeto.

🛠️ Tecnologias Utilizadas
Linguagem: Python 3.x
Framework: Apache Spark (PySpark MLlib)
Formato de Dados: Apache Parquet (Armazenamento columnar otimizado)
Ambiente: Jupyter Notebook

📈 Metodologia de Validação
Dada a natureza de séries temporais dos dados financeiros, evitámos a divisão aleatória (train_test_split) em favor de uma divisão temporal rigorosa (80% treino / 20% teste), prevenindo assim o data leakage (vazamento de informação futura para o treino).

🚀 Como executar
1 - Certifica-te de ter o Spark instalado ou utiliza um ambiente como o Google Colab.
2 - Clona o repositório:
git clone https://github.com/teu-usuario/teu-repositorio.git
3 - Instala as dependências necessárias:
pip install pyspark
4 - Abre o ficheiro Projeto_de_Big_Data.ipynb no Jupyter ou no VS Code e executa todas as células (Run All).
