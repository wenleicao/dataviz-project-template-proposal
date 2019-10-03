# Data Visualization Project

## Data

The data I propose to visualize for my project is Massachusetts Crime dataset
you can download the original file [here](https://ucr.fbi.gov/crime-in-the-u.s/2016/crime-in-the-u.s.-2016/tables/table-6/table-6-state-cuts/massachusetts.xls/output.xls)

## Prototypes

I’ve created a proof of concept visualization of this data. It's a ... and it shows ...

[![image](https://wenleicao.github.io/images/data_visualization/stacked_column.PNG)](https://beta.vizhub.com/wenleicao/4d191e28467d4533ab4a1eacf8d7aaf1)

[![image](https://wenleicao.github.io/images/data_visualization/scatter_chart.PNG)](https://beta.vizhub.com/wenleicao/acaf86b2f8ea488e87b3c1e47f79ca38)


## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:
*	Massachusetts community type (map chart)
*	How crime are distributed across Massachusetts? (map chart, total crime count, color based on number)
*	How crime are distributed after weighted by population? (using total crime count/ population, color based on number)
*	100% stacked column chart show crime difference between different community types.
*	Scatter chart between population and crime number, color by city
*	interactive chart, when choose area, community type (in the form of menu instead of checkbox), top 10 /bottom 10 cities show on the map (this will help people make decision)


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
 The other challenge how to map city and county to the map
Another challenge is to filter the chart when user choose a value.  

## Schedule of Deliverables
* 1-2 wk  I will complete R1 and R2 and also try to load map 
* 3-4 wk  complete L1, L2, L3, R3
* 5wk     finalize

