# SalesInsight PY

## 1. Objetivo do projeto

O SalesInsight PY é um projeto de análise de dados de vendas desenvolvido em Python. Seu objetivo é transformar dados brutos em informações úteis para compreender o desempenho comercial, identificar produtos e categorias relevantes e analisar o comportamento dos clientes.

O projeto utiliza um conjunto de dados de vendas em formato CSV e organiza o processo em etapas de inspeção, limpeza, transformação, análise, visualização e exportação de resultados.

## 2. Funcionalidades

O projeto contempla as seguintes funcionalidades:

- **Inspeção dos dados:** análise das dimensões, colunas, tipos de dados, valores ausentes e registros iniciais.
- **Limpeza dos dados:** tratamento de textos, conversão de datas, correção de tipos e remoção de registros com datas inválidas.
- **Transformação dos dados:** cálculo da receita total por venda e criação de colunas derivadas para análises temporais e classificação de valores.
- **Análise de vendas:** cálculo de métricas por mês, produto, categoria e região.
- **Segmentação de clientes:** classificação dos clientes nos segmentos Bronze, Prata e Ouro, conforme o valor total de suas compras.
- **Visualização dos resultados:** geração de gráficos para facilitar a interpretação dos dados.
- **Processamento reutilizável:** utilização de funções e da classe `AnalisadorDeVendas` para organizar as etapas do projeto.
- **Exportação dos resultados:** geração de arquivos CSV, JSON e imagens PNG.

## 3. Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Git e GitHub

## 4. Dados utilizados

O arquivo `vendas.csv` contém um conjunto de dados sintético com 200 registros de vendas e 8 colunas originais:

- `id_venda`
- `data_venda`
- `cliente`
- `produto`
- `categoria`
- `regiao`
- `quantidade`
- `preco_unitario`

Durante a etapa de limpeza, foram identificados 6 registros com datas inválidas. Esses registros foram removidos para evitar inconsistências nas análises temporais. Após o tratamento, o conjunto de dados ficou com 194 registros válidos.

## 5. Como executar o projeto

O projeto foi desenvolvido em um notebook Jupyter no Google Colab.

1. Acesse o arquivo `SalesInsight-PY.ipynb` neste repositório.
2. Abra o notebook no Google Colab.
3. Disponibilize o arquivo `vendas.csv` no ambiente de execução.
4. Execute as células na ordem apresentada no notebook.
5. Consulte os resultados das análises, os gráficos e os arquivos exportados.

As bibliotecas utilizadas devem estar disponíveis no ambiente Python. Caso necessário, instale as dependências antes de executar o notebook.

## 6. Organização dos resultados

Durante a execução, o projeto gera arquivos na pasta `outputs/`, incluindo:

- `metricas_por_mes.csv`
- `segmentacao_clientes.csv`
- `estatisticas_gerais.json`
- Gráficos PNG na pasta `outputs/graficos/`

Esses arquivos permitem consultar os resultados sem precisar refazer manualmente cada análise.

## 7. Conceitos aplicados

O desenvolvimento do projeto permitiu aplicar os seguintes conceitos:

- Leitura e manipulação de arquivos CSV.
- Inspeção, limpeza e transformação de dados.
- Tratamento de datas e tipos de dados.
- Criação de colunas derivadas.
- Agregação e cálculo de métricas com Pandas.
- Segmentação de clientes.
- Visualização de dados.
- Exportação de resultados em diferentes formatos.
- Criação de funções reutilizáveis.
- Programação orientada a objetos com a classe `AnalisadorDeVendas`.
- Organização de um projeto utilizando Git e GitHub.

## 8. Decisão técnica

Uma das decisões técnicas do projeto foi remover os registros com datas inválidas durante a etapa de limpeza.

Essa decisão foi tomada porque as datas são necessárias para agrupar e analisar as vendas por mês, trimestre e ano. Manter registros com datas inválidas poderia comprometer a consistência dessas análises.

A limpeza foi realizada com conversão de datas utilizando `errors="coerce"`, seguida da remoção dos registros que apresentaram datas inválidas.

## 9. Possíveis melhorias futuras

Como melhorias futuras, o projeto poderá incorporar novas métricas comerciais, filtros interativos, visualizações adicionais e mecanismos automatizados para atualização dos dados.

## 10. Demonstração em vídeo

**Link do vídeo:** 

O vídeo apresentará o objetivo do projeto, sua execução, as principais funcionalidades, a organização do desenvolvimento e uma decisão técnica adotada durante a análise dos dados.
