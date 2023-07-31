# cs416_d3

Narrative Visualization
Dileep Pasumarthi (dileepp2)
Link: https://pvsdileepoutlook.github.io/cs416_d3/
 Introduction:
For the final project, I created a narrative visualization dashboard that explains how the age distribution changed worldwide. It’s hosted on Git Hub in the link above. 

Narrative visualization is performed using “interactive slideshow”. First screen with “mouse over” looks as below. 


Image 1

A user can perform following actions


User can select a particular year (2010) in the picture above. Doing so will give them a distribution of world population in age groups divided by 5 years.
There’s annotation of the value of the bar chart at the beginning of each chart (white color text)
Hovering over a particular bar gives user a tooltip which has information about selected bar
User can also click particular bar which then let’s them drilldown to another chart.
Clicking on “Play all years” will start a nice animation of how the distribution changed over span of 100 years

On clicking a particular bar, it opens up another line chart for user to visualize more information:

Image 2

This is a line chart that conveys how the percentage of a particular age group changed over the span of 100 years
It has points in red color until the select year
All future years are marked in grey for easy understanding and distinguishing
Each data point can be hovered upon, which opens up more information about the data point.

How it met the guidelines of the project
This is an interactive slideshow structure, which lets the user navigate between 10 different slides and exploration into each bar was allowed.
Scenes follow a template for visual consistency. When the different slide is selected, several container elements are cleared and repopulated (bar chart, line chart, etc)
Visualization is rich with annotations, tooltips/popups
To the left of the bar chart, there is an annotation of the particular bar. Its always populated depending on a slide without any user interaction
The bar chart has a tooltip (image 1), which populates various information about the current point upon mouse hover
The line chart has another textbox that conveys the information about datapoint upon “mouseover”
Color changes for “mouseover”, “mouseclick”, “mouse out” etc are handled for easy understanding
The data is read from an external data source which has a call-back function
Several parameters exist to store the state of narrative visualization. Few things mentioned
“Age group” selected. This context is stored and propagated to the next chart too to facilitate the building of line chart and various other popups
“Year” selection is also stored to facilitate “red and grey” points distinguishing in line chart
Data is fetched accordingly based on year selection
Triggers like year selection help facilitate transition from one slide to another.
