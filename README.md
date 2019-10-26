# Data Visualization Project

## Data

The data I propose to visualize for my project is Massachusetts Crime dataset
you can download the original file [here](https://ucr.fbi.gov/crime-in-the-u.s/2016/crime-in-the-u.s.-2016/tables/table-6/table-6-state-cuts/massachusetts.xls/output.xls)

## Prototypes

I’ve created a proof of concept visualization of this data. It's 100% stacked column chart and scatter chart, which show crime differnece between different communities in Massachusetts.

[![image](https://wenleicao.github.io/images/data_visualization/stacked_column.PNG)](https://beta.vizhub.com/wenleicao/4d191e28467d4533ab4a1eacf8d7aaf1)

[![image](https://wenleicao.github.io/images/data_visualization/scatter_chart.PNG)](https://beta.vizhub.com/wenleicao/acaf86b2f8ea488e87b3c1e47f79ca38)


## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:
*	Massachusetts community type (map chart)
*	How crime are distributed across Massachusetts? (map chart, total crime count, color based on number)
*	How crime are distributed after weighted by population? (using total crime count/ population, color based on number)
*	100% stacked column chart show crime difference between different community types.
*	Scatter chart between population and crime number, color by city
*	interactive chart, when choose area, community type (in the form of menu instead of checkbox), top 5 /bottom 5 cities in selected area or community will show on the map (this will help people make decision)


## Sketches
The following is the sketches I created. 
[![image](https://wenleicao.github.io/images/data_visualization/sketch.PNG)]

Left 1 chart, create Massachusetts geoshape and map it to its county. This set a stage for later visualization 
left 2 chart, total crime distribution in different city 
left 3 chart, total crime count/population in different city (this will eliminate population factor) 
right 1 chart, different community (city, suburb and rural difference vs. different type of crime) 
right 2 chart, Scatter chart, can compare between cities, same level of population, how high the crime count is. 
Right 3 chart, linked chart, user can choose county and community type to choose upper 3 or bottom 3 crime count city.


## Open Questions
I have not been able to successfully load Massachusetts map yet.  I need to find shape file.
Another challenge is how to map city and county to the map
Third challenge is to filter the chart when user choose a value.  

## Schedule of Deliverables
* 1-2 wk  I will complete R1 and R2 and also try to load map 
* 3-4 wk  complete L1, L2, L3, R3
* 5wk     finalize

## Result of Implementation

Following the sequence of proposal from left to right  

* Massachusetts County Choropleth Map. This helps user understand county boundry and select proper region. You will be surprised how little you know the county name.  For me, a resident of massachusetts for 8 years. Some of county names are new to me. This map have interactive legend, which dynamically highlights the county when you hove mouse over the legend.  
[![image](https://github.com/wenleicao/wenleicao.github.io/blob/master/images/data_visualization/final/Chrolopleth%20map.PNG)](https://beta.vizhub.com/wenleicao/7c20a38e22d8485392c673c005794ad8)  

* Massachusetts Crime Distribution. This is a circle chart on MA map. The circle size stands for the crime number. Every circle will show tooltip indicating which city, county and crime total in 2016. You will notice three bigger circles which is Boston, Worcester and Springfield.
[![image](https://github.com/wenleicao/wenleicao.github.io/blob/master/images/data_visualization/final/total_crime.PNG)](https://beta.vizhub.com/wenleicao/97d58facdffd476cb860c1618cf02d16)   

* Massachusetts Weighted Crime Distribution.  When evaluting safety in a certain area, we need to consider the population as well. Obiviously, more people will have more crime. The crime total / population ratio (crime rate) will be a better measure for evaluating safety. Circle size is correlated with crime rate. When hoving over the circle, tooltip will pop up to show crime ratio and city, county name. From this Chart, you can see some towns have much higher crime ratio than others.   
[![image](https://github.com/wenleicao/wenleicao.github.io/blob/master/images/data_visualization/final/Crime_rate.PNG)](https://beta.vizhub.com/wenleicao/d704c9b0fe7f438c90a59b52e72d37c1)  

* Crime Type Comparison by Communities.  There are three type of Community in MA, City, Suburb and rurual. This 100% stack bar chart is ideal for comparing different crime type. Clearly, rural area has less people, it makes burglary less noticable. Therefore, rual has high proportion of burglary. On the contrary, city area has more people and cars, robbery and motor vehicle crime is higher. 
[![image](https://github.com/wenleicao/wenleicao.github.io/blob/master/images/data_visualization/final/crime_type_differnce.PNG)](https://beta.vizhub.com/wenleicao/cc8d8b881ec545c5ab2fac7d871fb3ea)  

* Crime Ratio Scatter Chart by Population. This Chart give you different angle to look at the data. You can compare crime rate between similar poplation level.  Scatter points are colored by county. You will find several towns in Hampden county are on the top. 
[![image](https://github.com/wenleicao/wenleicao.github.io/blob/master/images/data_visualization/final/city_compare_scatter.PNG)](https://beta.vizhub.com/wenleicao/b520f9b77d26485987a9df4d539eea31)   

* Safe Location Selector. This application can be used for location selector based on crime rate. Menu have been added to the chart so that user can select interested county, community and find top 5 safest cities. This app can be useful for tourist who want to select a place to stay, or real estate investor who want to choose safe place to buy a house et al.
[![image](https://github.com/wenleicao/wenleicao.github.io/blob/master/images/data_visualization/final/City_selector.PNG)](https://beta.vizhub.com/wenleicao/c995ae9a93c14690815217855f935ce2)   

