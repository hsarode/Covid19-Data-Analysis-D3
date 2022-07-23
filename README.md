# Covid-19-Data-Analysis-D3
![image](https://user-images.githubusercontent.com/88155960/180598259-3b7f4e41-05a5-4c3e-b9bb-7d0804877af2.png)

The dataset for this dashboard has been taken from [Covid-19 Data](https://github.com/owid/covid-19-data/tree/master/public/data)
by Our World in Data.

The dashboard comprises of 3 layouts, a map, a scatterplot, and line graphs. The map shows total cases from each country colored according to the intensity of cases. It tells us about how geographic location of a country affects the pandemic. 

The scatterplot shows the relation between wealth of population and its effect on pandemic. The bubbles represent country, and the color of the bubble represents the life expectancy of the people in that country. We can notice that with an increase in the GDP of a country the handwashing facilities have gone up along with the life expectancy. This tells us that countries with a higher GDP are more likely to smoothly sail through any new waves due to their higher life expectancy and higher number of handwashing facilities.

The line graph shows the total cases, total deaths, total vaccinations, and total boosters that have been recorded day wise for that specific country. This shows us the evolution of pandemic and the effect of vaccines and boosters on cases.

All the layouts have interactions with one another. The inner working of the code has been documented properly in the code for the dashboard


## Features

- Cross interactivity between all graphs
- Brushing possible on line graphs
- Data filtering by clicking on the data point
- Mouse click and hover events to display more information
- Automatic scaling of axes when data updates


## Run Locally

To visualize this dashboard, open the HTML file in any live server. For 
Visual Studio Code users, an extension called live server is available
that can be used. Once live server has been installed, right click on the file
and click "Open with Live Server" and the dasboard will display 
in your web browser.
## Screenshots
### Automatic Scaling of graphs
The ‘evolution of pandemic’ graphs by default show data of India. We can click on any country on the map or on the bubble from scatterplot which will automatically scale the graphs under ‘evolution of pandemic’ to show data from that country only. So, for example if we click on Russia, we get data about Russia and the y axis scale gets updated automatically 

### Use of cross-layout brushing in which moussing over one data point in one chart highlights multiple associated data points in another chart. 
![image](https://user-images.githubusercontent.com/88155960/180598273-07c30de6-41ff-4f14-a058-4f4d73b99551.png)

By default, all the layouts are shown at 100% opacity. When mouse is hovered upon any country from the map, the corresponding country’s bubble in ‘Wealth of population vs evolution of pandemic’ gets highlighted. Here, we mouseover Sudan on the map and the bubble displaying Sudan in the 2nd graph gets highlighted.

Similarly, when mouse is hovered over any bubbles in the scatterplot, the corresponding country gets highlighted in the map as shown below. Kazakhstan gets highlighted when hovered over that bubble.
A mouseover function has been defined for both the scatterplot and the map. During mouseover, the second layout is selected and faded to an opacity of 10% and the country selected is filtered in the second layout which then gets 100% opacity.

### Use of cross-layout brushing in which dragging a rectangle over several data points in one chart highlights multiple associated data points in another chart
Below we can see that the map on the left the legend and the colors of the countries on the map. The color is representative of the total cases in that country. When we perform brushing on graphs below ‘Evolution of pandemic’ between April 2021 and October 2021 we see that the legend on the graph changes and the countries change color to show updated number of cases between the time period where brushing occurs as shown in second screenshot.

![image](https://user-images.githubusercontent.com/88155960/180598279-7c635518-ed4a-4bd7-b747-1e9e6795c65a.png)
![image](https://user-images.githubusercontent.com/88155960/180598286-1cf04c7a-d33c-4a30-8725-784a4ded6c35.png)