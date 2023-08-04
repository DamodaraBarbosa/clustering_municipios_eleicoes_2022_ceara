# *Clustering* dos municípios cearenses - Eleições 2022

## Objetivo do projeto

Obter e extrair dados a fim de analisar (dados da votação, mas também de votação por indicadores socioeconômicos) e *clusterizar* os municípios cearenses com base na proporção de votos nos **principais candidatos aos cargos de: governador, senador e presidente (1º e 2º turno).**

## Etapas do projeto

### Obtenção de extração dos dados:

Os dados foram obtidos ou extraídos utilizando a biblioteca `selenium`. Os dados eleitorais foram coletados com automação *web* a partir do portal de dados abertos do TSE.
![image](https://github.com/DamodaraBarbosa/clustering_municipios_eleicoes_2022_ceara/assets/107199898/c75d622e-6467-46a2-b917-71f8166271ab)

Os dados de resumo de alguns indicadores socioeconômicos do IBGE foram extraídos por meio de *web scraping*.

### Extração e tratamento dos dados:

Os obtidos do TSE são compactados, sendo necessária a sua descompactação.
