# MVP - Cobertura Vacinal contra o Sarampo no Brasil

MVP desenvolvido para a Sprint de Engenharia de Dados da Pós-Graduação em Ciência de Dados e Analytics da PUC-Rio.

## Objetivo

Analisar a evolução da cobertura vacinal contra o sarampo no Brasil ao longo dos anos, considerando diferenças temporais e geográficas nos indicadores de vacinação.

## Fontes de dados

- DATASUS / SI-PNI: dados de cobertura vacinal da Tríplice Viral D1, Tríplice Viral D2 e Tetraviral.
- IBGE / SIDRA: dados do Produto Interno Bruto dos municípios brasileiros.

## Tecnologias utilizadas

- Databricks Free Edition
- Python
- PySpark
- Delta Lake

## Arquitetura

O pipeline foi desenvolvido utilizando a arquitetura Medalhão:

- **Bronze:** ingestão dos dados brutos e avaliação inicial da qualidade.
- **Silver:** limpeza, padronização e transformação dos dados.
- **Gold:** integração dos indicadores e preparação das tabelas utilizadas nas análises.

## Notebooks

Os notebooks estão disponíveis na pasta `notebooks` e foram organizados conforme a sequência de desenvolvimento do pipeline:

1. `01_ingestao_bronze.ipynb` - ingestão dos dados de vacinação.
2. `02_qualidade_bronze.ipynb` - avaliação inicial da qualidade dos dados.
3. `03_transformacao_silver.ipynb` - tratamento e transformação dos dados de vacinação.
4. `04_bronze_PIB.ipynb` - ingestão dos dados de PIB.
5. `05_silver_PIB.ipynb` - tratamento dos dados de PIB.
6. `06_Modelagem Gold.ipynb` - consolidação das tabelas analíticas.
7. `07_analise_dados.ipynb` - análises e visualizações dos dados.

## Estrutura do repositório

    mvp-cobertura-vacinal/
    ├── notebooks/
    │   ├── 01_ingestao_bronze.ipynb
    │   ├── 02_qualidade_bronze.ipynb
    │   ├── 03_transformacao_silver.ipynb
    │   ├── 04_bronze_PIB.ipynb
    │   ├── 05_silver_PIB.ipynb
    │   ├── 06_Modelagem Gold.ipynb
    │   └── 07_analise_dados.ipynb
    └── README.md

## Autora

Marina Araujo Gonzaga
