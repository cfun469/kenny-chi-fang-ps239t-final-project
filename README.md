## kenny-chi-fang-ps239t-final-project

This is the final project of POLISCI 239T. In this project, I aimed to make military index like military expense and growth as well as their relevant indices more readible and accessible. For this reason, I made two forms of visualization. Three indices were included to derive more data, they are: military burden, military expense, and military expense as the share of GDP. <br />

The first would be a leaflet interactive map that include all threee indices. By projecting them to a interactive world map, readers would be able to navigate around and have a rough understanding regarding the distribution of military spending. The second set of visualization took advantage of ggplot2. By manipulating the existing data, it derived several other indices like growth rate and moving average of each figure. With these in hand, several other static plots were produced. 

## Dependencies 
1. R, version 3.5.3

## Files

### Data
1. Raw Data
  - SIPRI-Milex-data-1949-2017-1.xlsx: SIPRI (Stockholm International Peace Research Institute) military expenditure database, available here https://www.sipri.org/databases/milex
  - countries_codes_and_coordinates.csv: List of national ISO alpha code, available here https://gist.github.com/tadast/8827699
2. Clean Data
  - mapping_data.csv: Contains shape file and indicators extracted from the SIPRI database. 
  - military_burden.csv: Contains military expense per capita, which is also known as military burden, of each country, directly adapted from the SIPRI data.
  - military_expense.csv: Contains military expense in terms of 2016 US current of each country, directly adapted from the SIPRI data.
  - military_gdp_share.csv: Contains military expense in terms of the share of national GDP, directly adapted from the SIPRI data.
  - military_index_ggplot.csv: The clean version of the adpated military expenditure data, sort by year. However, I failed to group_by country since it automatically added new variables without giving the desirable outcomes.
  - military_index_eight_nation.csv: Contains military indicator and the other indicators of eight countries selected from the datasets above, including growth rate of three indicators mentioned above as well as the rolling average of the military expenditure. 
 3. Shape file: see Readme.txt in the file.
  - Readme.txt
  - TM_WORLD_BORDERS_SIMPL-0.3.dbf
  - TM_WORLD_BORDERS_SIMPL-0.3.prj
  - TM_WORLD_BORDERS_SIMPL-0.3.shp
  - TM_WORLD_BORDERS_SIMPL-0.3.shx
  - TM_WORLD_BORDERS_SIMPL-0.3.zip
### Results
1. gdp_share_rose_plot.png: The rose plot of the military expenditure (% of GDP) from 1992 to 2017.
2. military_burden_and_expense.png: The stacked bar plot of the growth rate of military burden and the line graph of annual military expenditure of eight countries from 1992 to 2017.
3. military_expense_streamgraph.png The moving average of military expenditure of eight countries from 1992 to 2017.
4. military_index_map.html: The interactive map including three indicators from four years: 1992, 2000, 2008, and 2017.
5. military_index_map.rar: The interactive map stored in the rar file to prevent the failure of upload and download.
