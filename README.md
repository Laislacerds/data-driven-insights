# Projeto Data Driven Insights

## Descrição do Projeto

Este projeto teve como objetivo explorar, transformar e visualizar dados utilizando Python e suas bibliotecas como pandas, numpy e matplotlib, com foco em gerar insights descritivos a partir da análise da base de dados **Sales Data Sample**.

## Base de Dados

- **Nome:** Sales Data Sample  
- **Quantidade de linhas:** 2.823  
- **Quantidade de colunas:** 25  
- **Descrição:** Dados simulados de vendas contendo informações sobre pedidos, produtos, clientes, valores, datas e localização.

## Etapas Realizadas

### 1. Importação e Exploração Inicial dos Dados
- Leitura do arquivo CSV com pandas.
- Visualização das primeiras linhas do DataFrame.
- Análise das linhas e colunas.
- Exibição dos nomes das colunas.
- Verificação dos tipos de dados (varchar, inteiros, floats).
- Conversão da coluna `ORDERDATE` para tipo datetime para facilitar análises temporais.

### 2. Manipulação de Dados com Listas, Dicionários e Tuplas
- Extração da coluna `PRODUCTLINE` em uma lista para análise inicial da rotatividade dos produtos.
- Criação de um dicionário mapeando produtos e países para entender a distribuição geográfica.
- Definição de tuplas com dados selecionados de uma linha, facilitando a análise combinada de múltiplos atributos.

### 3. Estruturas Condicionais e Laços
- Aplicação de condições para classificar valores da coluna `PRICEEACH` como alto, médio ou baixo.
- Uso de laços `for` para somar os cinco primeiros valores de preço unitário.
- Uso de laço `while` para encontrar o primeiro valor que ultrapasse um limite predefinido.

### 4. Operadores Aritméticas
- Criação de uma nova coluna `Desconto` que aplica um desconto fictício de 10% sobre o preço unitário (`PRICEEACH`).
- Visualização das primeiras linhas para confirmar o cálculo.

### 5. Operações com NumPy
- Transformação da coluna `QUANTITYORDERED` em array NumPy.
- Realização de operações vetorizadas: soma constante, potência ao quadrado.
- Aplicação de operações agregadas como soma e média.

### 6. Manipulação com Pandas
- Filtragem dos dados para selecionar vendas com quantidade superior a 10.
- Uso de `.value_counts()` para contagem de linhas por categoria de produto.
- Agrupamento dos dados por `PRODUCTLINE` para análise de volume total de vendas.

### 7. Visualização de Dados
- **Gráfico de Linha:** Evolução do total de vendas ao longo do tempo (por mês).
- **Gráfico de Barras:** Volume total de vendas por linha de produto.
- **Gráfico de Dispersão:** Relação entre preço unitário (`PRICEEACH`) e quantidade vendida (`QUANTITYORDERED`).

### 8. Insights Obtidos
- Identificação de que a linha de produtos **Motorcycles** tem alta rotatividade e volume de vendas.
- Maior venda individual analisada foi de R$ 5.205,27.
- Produtos com preço unitário menor tendem a ser vendidos em maiores quantidades, comportamento típico de consumo.
- Visualização de picos de vendas e identificação de produtos mais rentáveis.
- Confirmado que a base contém dados categóricos, numéricos e temporais, sem dados booleanos.
- Alguns dados de data foram convertidos para datetime para melhor análise temporal.
- Perguntas para futuras investigações diferença entre países, clientes com maior ticket médio e previsão de vendas.

## Como Executar

1. Clone o repositório:
Abra o arquivo data_driven_insights.ipynb no Google Colab.
Execute as células sequencialmente para acompanhar a análise e visualizações.
Importe a base de dados para dentro do google colab. Disponibilizei a base de dados na pasta Sales_data_sample. Base de dados extraida do Kaggle.

## Tecnologias e Bibliotecas

Python 3.x

pandas

numpy

matplotlib

Google Colab (para execução do notebook)

## Contato
LinkedIn: www.linkedin.com/in/laíslacerda
