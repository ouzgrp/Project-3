# Project 3

Team members: Oz, Tue, Mirta and Maham

Project Topic : Canada's Financial Aid Visualizer

This project is an addition to the Project 1 with a new data regarding the Canada's Financial Aid. The first project was focused on world happinesss index, while project 3 is showing the amount of financial aid that Canada sent to other countries in the world. Furthermore, this project compares the financial aid amount with the hapiness index, democracy index, human development index and type of goverment (authoritarian, hybrid, flawed democracy and full democracy). 

The data for this project was used from the four data sources and comined to csv file (combinedData3.csv), please see the data sources links below. 

The project has four different Javasript files that contains codes to create D3 map vizulation:
  - scales.js: creating scales for each variable (hapiness, democracy index, etc) with a linear relationship between input and output usinf     d3.scaleLinear, d3. scaleQuantize, d3.scaleband and d3.scaleLog
  - scripts.js: using svgmap for creating interactive world map so we can compare data between each coutry, adding Flowline
  - controller.js: codes for filtering the map and creating democracy, HDI and happiness bar
  - compare.js: developing comparison tools between countries and adding to bar chars
  - jquery.autocomplete.min.js - Ajax Autocomplete for jQuery allows to create autocomplete/autosuggest boxes for text input fields

Js are then added to the html 

 <script src='https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.0/jquery.min.js'></script>
    <script src='js/jquery.autocomplete.min.js'></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
    <script src='js/scales.js'></script>
    <script src='js/scripts.js'></script>
    <script src='js/controller.js'></script>
    <script src='js/compare.js'></script>

The final result is interactive world map that has a an option to check indexes in each country, has a filter option for flow line, showing details of each country and comparison tool.

<img width="1138" alt="worlmap" src="https://github.com/ouzgrp/Project-3/assets/125240038/404d3508-dc8c-4da0-8acd-b8bed116d4f5">


    
  

Features:

-filter metrics to display on map
-filter lines showing flow of money by amount
-compare government type, aid, HDI, etc of 2 countries, with autocomplete
-tooltips showing chart of data about each country when hovering over on map
-option to filter out which arcs to display by aid threshold
-selector to change which variable is shown on the choropleth
-comparison tool to compare data for two different countries

======================================

Data Sources:

HDI - http://hdr.undp.org/en/data

Happiness - http://worldhappiness.report/ed/2016/

Democracy Index - http://www.eiu.com/public/thankyou_download.aspx?activity=download&campaignid=DemocracyIndex2016

Foreign aid - https://www.international.gc.ca/department-ministere/open_data-donnees_ouvertes/dev/statistical_report_country-rapport_statistique_pays.aspx?lang=eng
