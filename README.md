# Projeto Imobiliária - Análise de Dados com Pandas

## Descrição do Projeto

Este projeto foi desenvolvido para uma empresa imobiliária com o objetivo de realizar análises exploratórias de dados utilizando a biblioteca Pandas em Python. O foco principal foi entender as características dos imóveis disponíveis para aluguel, identificar padrões e gerar insights valiosos para as equipes de Machine Learning e Desenvolvimento.

## Base de Dados

A base de dados utilizada contém informações sobre imóveis para aluguel, incluindo:

- Tipo de imóvel  
- Bairro  
- Valor do aluguel  
- Condomínio  
- Número de quartos, suítes e vagas de garagem  
- Área do imóvel  
- IPTU  

## Principais Análises Realizadas

### 1. Análise Exploratória Inicial
- Carregamento e inspeção inicial dos dados  
- Identificação das colunas e tipos de dados  
- Estatísticas básicas dos valores de aluguel  

### 2. Análise por Tipo de Imóvel
- Cálculo do valor médio de aluguel por tipo de imóvel  
- Filtragem para remover imóveis comerciais  
- Análise de percentual de cada tipo de imóvel na base de dados  

### 3. Foco em Apartamentos
- Filtragem para trabalhar apenas com apartamentos  
- Cálculo da média de quartos por apartamento  
- Análise dos bairros com os valores médios mais altos  

### 4. Tratamento de Dados
- Lidando com valores nulos (preenchimento com zero)  
- Remoção de registros inconsistentes (valores zerados)  
- Exclusão de colunas não necessárias  

### 5. Filtros Avançados
- Apartamentos com 1 quarto e aluguel menor que 1200  
- Apartamentos com pelo menos 2 quartos, aluguel menor que 3000 e área maior que 70  

### 6. Criação de Novas Colunas
- Colunas numéricas: Valor por mês (aluguel + condomínio) e Valor por ano  
- Colunas categóricas: Descrição completa do imóvel e indicação de suíte  

## Principais Comandos Pandas Utilizados

- `pd.read_csv()` - Para carregar os dados  
- `head()`, `tail()`, `info()` - Para inspeção inicial  
- `groupby()` - Para agregações por categoria  
- `mean()`, `value_counts()` - Para cálculos estatísticos  
- `query()` - Para filtragem de dados  
- `isnull()`, `fillna()`, `drop()` - Para tratamento de dados  
- `to_csv()` - Para exportar os dados processados  
- `plot()` - Para visualização de dados  

## Resultados e Saídas

O projeto gerou vários insights valiosos, incluindo:

- Gráficos de barras mostrando valores médios por tipo de imóvel  
- Percentual de cada tipo de imóvel na base de dados  
- Ranking de bairros com os valores mais altos  
- Dataframes filtrados com imóveis que atendem a critérios específicos  

## Arquivos Gerados

- `dados_apartamentos.csv` - Contém apenas dados de apartamentos após tratamento  
- `dados_completos_dev.csv` - Contém todos os dados com as novas colunas criadas  

## Como Utilizar

1. Clone o repositório ou baixe os arquivos  
2. Execute o notebook `projeto_imobiliaria.py` em um ambiente Python com Pandas instalado  
3. Os dados serão carregados automaticamente da URL fornecida  
4. Siga as células sequencialmente para reproduzir as análises  

## Requisitos

- Python 3.x  
- Pandas  
- Matplotlib (para visualizações)  

---

Este projeto demonstra o poder da biblioteca Pandas para análise e manipulação de dados no contexto imobiliário, fornecendo bases sólidas para tomada de decisões e desenvolvimento de modelos mais avançados.
