Full code <a>https://gist.github.com/Ikaay-99/698362f3b2d69990fef3cff7c8a24604</a>

<h2>Choropleth Maps</h2>
<p>Plotting a choropleth map requires two forms of input: Geometrical Info (coordinates, regions, etc.) and Values. Since our study focused on the USA, plotting choropleth maps was relatively straightforward given Plotly's inbuilt USA State GeoJSON. This automatically maps US States to their geometric outlines using their two-letter codes as an identifier. A column was added for all relevant CSV documents to include the two-letter state code for each US territory. For example, Arizona is identifiable as AZ.
​
To implement, we set the location property of the choropleth to be fetched from the CODE column of the dataframe and the location-mode property was set to 'USA-States'. Similarly, the z property (values to be colour-coded) was to be fetched from the relevant column. Below is a snippet of the code producing a choropleth map of the density of black residents in US States.
