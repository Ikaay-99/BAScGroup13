Full code <a>https://gist.github.com/Ikaay-99/698362f3b2d69990fef3cff7c8a24604</a>

<h2>Choropleth Maps</h2>
<p>Plotting a choropleth map requires two forms of input: Geometrical Info (coordinates, regions, etc.) and Values. Since our study focused on the USA, plotting choropleth maps was relatively straightforward given Plotly's inbuilt USA State GeoJSON. This automatically maps US States to their geometric outlines using their two-letter codes as an identifier. A column was added for all relevant CSV documents to include the two-letter state code for each US territory. For example, Arizona is identifiable as AZ.
​
To implement, we set the location property of the choropleth to be fetched from the CODE column of the dataframe and the location-mode property was set to 'USA-States'. Similarly, the z property (values to be colour-coded) was to be fetched from the relevant column. Below is a snippet of the code producing a choropleth map of the density of black residents in US States.
  
add snippet on website

<p>Finally, to limit the scope of the choropleth map to just the USA, the geo_scope property of the plot layout was set to 'usa'. The hover text of the graph provided a breakdown of the statistics in use. This was achieved by creating a new dataframe column called 'text', which iterated over the states, storing data from each row, and held the hover text as a formatted string.
  
<h2>Regression</h2>
<p>Plotly allows us to make least-squares regression lines straight away by including the trendline argument in out scatter plot call. To make a ordinary least-squares regression line, we set this argument to 'ols'. We can also retrieve the statistical results of the regression analysis as shown in the snippet below.
  
add snippet

We wanted the results of our regression to be viewable as an image file. Plotly allows us to print out the results to the terminal as text, but not as an image. This was a strange task as it required us to map a string (which has no dimensions or spatial properties) to an image. After some trial-and-error and research, we settled on a solution which produced an elegant image ideal for monospace fonts. The code is shown in the snippet below.

add snippet

<h2>Bar Charts</h2>
<p> Plotly allows us to make bar charts quite easily using either the go.Bar or px.bar calls utilising the graph objects and express classes respectively. I opted for the former as it allows for greater flexibility with styling. Furthermore, in the case of the funding chart, the graph objects library allows us to create customisable stacked bar charts. Below is a snippet of the code used to produce the stacked bar chart from the dataframes created using the funding data. A slight challenge was specifying a dataframe based on row criteria. Selecting a group of columns by name or range is fairly straightforward, but rows function differently. After research, I opted for the .isin function call, with the argument being a list of the relevant row names (in this case, our case study states).
  
add snippet

<p>To create a stacked bar chart, the relevant data fields must be given input to separate data arguments in the function call go.Bar. Then, the bar mode must be set to stack in the styling/layout section. It is also necessary to specify the orientation argument as 'h' meaning horizontal. For the fatal encounters bar chart, we had to also specify its x-axis to be reversed, so as to achieve the 'back-to-back' effect. Below is a snippet showing the styling method for the fatal encounters bar chart.
  
add snippet

<h2>Case Study</h2>
<p> This visualisation is composed of two plots superimposed on one another: a bubble scatter plot (whose sizes depended on the number of fatal encounters) and a line scatter plot (with funding ratio against time). Due to the library's limitations and the multiple dataframes being worked with, it proved simplest to input most of the data manually for each state. As such, the line plots were traced separately for each state. Below is a snippet showing the construction of Florida's data.

add snippet

<p> A blank plot was created by calling go.Figure(). Then, the line traces for each state were added to the blank plot in turn. The bubbles were also added to the same plot. For ease of viewing, the sizes of the bubbles were scaled up 50x across all states and values.  Colours of the lines were made to be coordinated for each state and distinct from the others. Below is a snippet showing how this was achieved for Florida.

add snippet

<p> Finally, the hover text was appended for each bubble using a for loop. The data was fetched from the dataframe field corresponding to the iterative cycle. Snippet below:
  
add snippet
