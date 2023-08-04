# *Clustering* dos municípios cearenses - Eleições 2022

## **Objetivo do projeto**

Obter e extrair dados a fim de analisar (dados da votação, mas também de votação por indicadores socioeconômicos) e *clusterizar* os municípios cearenses com base na proporção de votos nos **principais candidatos aos cargos de: governador, senador e presidente (1º e 2º turno).**

## **Etapas do projeto**

### Obtenção de extração dos dados:

Os dados foram obtidos ou extraídos utilizando a biblioteca `selenium`. Os dados eleitorais foram coletados com automação *web* a partir do portal de dados abertos do TSE.
![image](https://github.com/DamodaraBarbosa/clustering_municipios_eleicoes_2022_ceara/assets/107199898/c75d622e-6467-46a2-b917-71f8166271ab)

Os dados de resumo de alguns indicadores socioeconômicos do IBGE foram extraídos por meio de *web scraping*.

### Extração e tratamento dos dados:

Os obtidos do TSE são compactados, sendo necessária a sua descompactação. Para isso, uma classe **Extract** foi instanciada com base na biblioteca `zipfile`. Ambos os dados (eleição e IBGE) foram tratados para que estivessem num formato mais pronto para as análises posteriores e *clusterização*.

### Análise dos dados:

Para obter diferentes *insights*, foram feitas diversas análises. Tanto de um panorama mais geral para entender o número de zonas e seções eleitorais, e as cidades com o maior número destas, mas também a contribuição de votos de cada município para eleição no estado.

Assim como análises mais focadas nos cargos disputados. A visualização de dados foi feita utilizando a biblioteca `plotly`. Também foi feito o uso da biblioteca `geobr` a fim de obter dados geoespaciais.

![image](https://github.com/DamodaraBarbosa/clustering_municipios_eleicoes_2022_ceara/assets/107199898/b5121ce3-4502-45a5-8cdd-d3820ad61278)

### *Clustering* dos municípios cearenses e análise de seus perfis:

A modelagem foi feita utilizando o algoritmo *KMeans* e teve como base a proporção de votos válidos para os principais candidatos que disputaram os cargos de governador e senador do estado, além de presidente (3 candidatos para o 1º turno e 2 candidatos no 2º turno). No estado do Ceará não houve disputa no 2º turno para governador.

![image](https://github.com/DamodaraBarbosa/clustering_municipios_eleicoes_2022_ceara/assets/107199898/d84cf9f7-bbbb-42ee-933d-6fe93d4a36c4)

Ademais, após a definição dos *clusters* foi feita a **análise do perfil eleitoral de cada um deles.**

## **Como executá-lo?**

A pasta `dataprocessing` contém o pacote com as classes utilizadas para coletar, extrair e baixar os dados. O código está documentado.
Além disso, o arquivo `requirements.txt` contém as versões da ferramentas utilizadas no projeto.

## Desenvolvido por

Damodara Barbosa, Cientista de Dados e Instrutor de Ciência de Dados
LinkedIn: https://www.linkedin.com/in/damodarabarbosa/
