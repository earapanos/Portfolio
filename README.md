<h1 align="center"><a href="https://github.com/earapanos">📖 Eduardo Rapanos Portfolio</h1></a>

<h3>🔗 Index:</h4>

1. <a href="https://github.com/earapanos/Censo22CoordenadasGeograficas">🗺 Coordenadas Geográficas do Censo IBGE 2022 - Dashboard</a>
2. <a href="https://github.com/earapanos/Census10-22-DataAnalytics">🔎 Data Analytics and Visualization - Palhoça, BR </a>
3. <a href="https://github.com/earapanos/Python-Geocoding-Data">🚩 Address Geocoding with ArcGIS API </a>
4. <a href="https://github.com/earapanos/Python-Geocoding-Data">🧭 WebGIS Project for Geoparque Caminhos dos Cânions do Sul (GCCS) </a>

<h2></h2>

<h2 align="center"><a href="https://github.com/earapanos/Censo22CoordenadasGeograficas">1. 🗺 Coordenadas Geográficas do Censo IBGE 2022 - Dashboard</a></h2>

Nessa dashboard você vai poder visualizar os dados das coordenadas geográficas de domicílios. Estes dados foram divulgados pelo Instituto Brasileiro de Geografia e Estatística - IBGE e fazem parte do levantamento realizado pelo Censo demográfico e socioecomômico realizado em 2022.

O objetivo dessa dashboard foi utilizar os dados de coordenadas geográficas disponibilizadas para domicílios e estabelecimentos do IBGE para se analisar espacialmente e geograficamente a sua distribuição nos municípios do Acre, Brasil.

Para que a dashboard pudesse ser construída, foi elaborado um processo de ETL para a normalização dos dados e para que se pudessem ser correlacionadas estas informações com outras tabelas no Banco de Dados Relacional. Com isso foi possível de se obter uma tabela com os nomes dos municípios do estado do Acre e as coordenadas dos domicílios, o que permitiu a representação destas junto ao Looker Studio.

<h4 align="center"><a href="https://lookerstudio.google.com/reporting/29cb3a4c-5ab0-4275-b254-ff0b83562033">  👇 Clique na imagem para acessar o Dashboard. </a></h4>
<a href="https://lookerstudio.google.com/reporting/29cb3a4c-5ab0-4275-b254-ff0b83562033" target="_blank" rel="noreferrer"> <img src="https://github.com/earapanos/Censo22CoordenadasGeograficas/assets/52800638/5919327f-9538-4a53-9a41-304388f35175" alt="dashboard"> </a> 

<h4>Nas tabelas originais você vai encontrar as seguintes variáveis:</h4>


COD_UF (NUMERIC) = Variável numérica com o código da unidade federativa;

COD_MUN (NUMERIC) = Variável numérica com o código do município;

COD_ESPECIE (VARCHAR) = Variável alfanumérica com a categoria e descrição da espécie do endereço e que podem ser:

    1=Domicílio particular
  
    2=Domicílio coletivo
  
    3=Estabelecimento agropecuário
  
    4=Estabelecimento de ensino
  
    5=Estabelecimento de saúde
  
    6=Estabelecimento de outras finalidades
  
    7=Edificação em construção
  
    8=Estabelecimento religioso
  
LATITUDE =  Variávem com a Latitude da Coordenada de Localização da Espécie do Endereço;

LONGITUDE = Variávem com a Longitude da Coordenada de Localização da Espécie do Endereço;

NV_GEO_COORD = Variável com o nível de geocodificação do domicílio ou estabelecimento que podem ser:

    1=Endereço - coordenada original do Censo 2022
  
    2=Endereço - coordenada modificada (apartamentos em um mesmo número no logradouro*)
  
    3=Endereço - coordenada estimada (endereços originalmente sem coordenadas ou coordenadas inválidas**)
  
    4=Face de quadra
  
    5=Localidade
  
    6=Setor censitário


<H3>Fonte de dados:</H3>

Você pode acessar todas as publicações e dados do **Censo de 2022** disponibilizados pelo <a href="https://censo2022.ibge.gov.br/panorama/downloads.html?localidade=BR">IBGE AQUI!</a>


<h2 align="center"><a href="https://github.com/earapanos/Census10-22-DataAnalytics">2.🔎 Data Analytics and Visualization - Palhoça, BR </a></h2>

<div align="center">
  <img src="https://github.com/earapanos/Census10-22-DataAnalytics/assets/52800638/9eafcdbd-d4fb-412b-8b2d-0356138a8bf9" alt="Demonstração">
</div>

<h2>Data Analysis of census Sector Population of 2010 and 2022 Census - Palhoça City, Brazil</h2>
  
Palhoça is a city from east part of Santa Catarina estate and it is located on Florianópolis Metropolitan Region. Palhoça is an economic centre based on services industries and in your territory there are an important natural reserve, that include a huge hydric rosources, forestry, coastal and scenic. These settings makes Palhoça city a strong destinity of migrants in Brazil.

The Brazilian Institute of Geography and Statitics (IBGE as a brazilian acronym) published recently a preview of the population per census sector of all brazilian territory. The results of 2022 Census allow to explore the spatial analysis since there are available the geometries of each census sector.

The definition of IBGE (2024) to census sector is:

"The Census Sector is the smallest territorial unit, formed by a continuous area, entirely contained in an urban or rural area, with an adequate size for research operations and whose totality covers the entire National Territory, which allows to guarantee complete coverage of the Country."

<h3>Objectives:</h3> 

In this notebook I'm going to analyze, compare and create some ways to understand the changes of the data of 2010 and 2022 census from Palhoça City, Brazil.

<h3>Structure of Notebook:</h3>

The notebook is subdivided in this structure:

* Data importing;
* Data analysis;
* Data transforming;
* Data visualization:
  * through the maps;
*2022 vs. 2010 Statitics.
  * bar chart;
 * scatter plot;

<h4 align="left"><a href="https://github.com/earapanos/Census10-22-DataAnalytics/blob/main/data-analytics-and-visualization-palho-a-br.ipynb"> 🖱 Click here to access the Notebook! </a></h4>

<h4 align="left"><a href="https://www.kaggle.com/code/rapanos/data-analytics-and-visualization-palho-a-br"> 🖱 Click here to access the project on Kaggle! </a></h4>

<h2 align="center"><a href="https://github.com/earapanos/Python-Geocoding-Data">3. 🚩 Address Geocoding with ArcGIS API </a></h2>

![openart-image_JECrDnRQ_1715684494402_raw](https://github.com/user-attachments/assets/f26bf0e6-66ea-4538-b885-d908c9a0d9b2)

#### Description

This Python script geocodes addresses from a PostgreSQL database using the ArcGIS API. It connects to the database using psycopg2, a PostgreSQL adapter for Python, and geocodes addresses using the geopy library's ArcGIS geocoder. The script is divided into functions to handle database connection, counting geocodable elements, geocoding addresses, updating the geocoded table, and closing the database connection. The main function orchestrates the process and includes error handling to restart the code in case of failure.

#### Features

*   **Database Connection:** Establishes a connection to a PostgreSQL database.
*   **Element Counting:** Counts the total number of elements and the number of geocodable elements in a specified table and schema.
*   **Address Geocoding:** Uses the ArcGIS geocoder to geocode addresses from the database.
*   **Table Update:** Updates the geocoded table in the database with latitude, longitude, geocoding precision, and formatted address.
*   **Error Handling:** Restarts the code in case of an error, ensuring continuous operation.

#### Usage



1.  Update the database connection parameters (`host`, `database`, `user`, `password`).
2.  Specify the schema, table, address column, precision column, and formatted address column in the `main` function.
3.  Define the municipalities to geocode in the `municipalities` variable.
4.  Run the script to start the geocoding process.

#### Requirements

*   Python 3.x
*   psycopg2
*   geopy

<h2 align="center"><a href="https://github.com/earapanos/GeospatialDataGCCS">4. 🧭 WebGIS Project for Geoparque Caminhos dos Cânions do Sul (GCCS) </a></h2>

<div align="center">
  <img src="https://github.com/user-attachments/assets/3ba7eca3-31ac-4b24-8e34-28934e981726" alt="Demonstração">
</div>

# WebGIS Project for Geoparque Caminhos dos Cânions do Sul (GCCS)

## Project Overview

This WebGIS project is dedicated to publishing detailed geomorphological, geological, and structural data for the territory of the Caminhos dos Cânions do Sul UNESCO Global Geopark (GCCS). The goal is to provide an accessible platform for visualizing and analyzing the unique geological features and processes that define this region. **Explore the WebGIS platform here: [Geospatial Data GCCS WebMap](https://earapanos.github.io/GeospatialDataGCCS/).**

## Data Sources

The data used in this project are derived from the research article:

[Caracterização Morfoestrutural e Morfoescultural no Território do Geoparque Global UNESCO Caminhos dos Cânions do Sul (RS/SC)](https://www.researchgate.net/publication/362291916_Caracterizacao_morfoestrutural_e_morfoescultural_no_territorio_do_Geoparque_Global_UNESCO_Caminhos_dos_Canions_do_Sul_RSSC)

The vector files are available for download from:

[Geospatial Data GCCS - Vector Layers](https://github.com/earapanos/GeospatialDataGCCS/tree/main/layers/vetoriais)
