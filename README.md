# covidlessbestroute
For implementing the proposed system Google Collaboratory platform is used as
an interface.
I.Web Scraping
Web scraping is a technique of extracting data from a website. The required libraries 
to be imported are tabula, pandas. The procedural steps to be followed are
1.Identify the target website: The Aim is to get the number of covid cases in each
district of Telangana. Choose the official website for accurate information.
2. Daily update of covid cases: The number of cases change on a daily basis.
Automate the URL for cases update.
3. Extract the required data.
4. Save the data in a CSV file.
II.Map Generation using folium
Folium is a data visualization library in Python that was built to help people
visualize geospatial data. With Folium, one can create a map of any location in the
world with the help of latitude and longitude values. Consider latitudes and
longitude values of 32 districts of Telangana to plot in a map. Check the values
from any official website. Join the places which have road route possible using
circle marker, polyline functions.
III. Application of Dijkstra algorithm
A Graph is a non-linear data structure consisting of nodes and edges. Dijkstra algorithm is a
greedy algorithm which is used for finding the shortest distance, or path, from
starting node to target node in a weighted graph. This algorithm makes a list of the
shortest path from the starting node, the source, to all other nodes in the graph.
Here the aim is not to get the shortest distance but to get the path with less covid
cases. So, consider districts as nodes and number of covid cases as edges and
follow the same Dijkstra algorithm.
Using the CSV module, we convert the csv file extracted into a dictionary in
python. Take a class naming Graph and write functions for adding nodes and
edges. For instance, take two places A and B which have direct road route. For A
to B consider the cost as the number of covid cases of A and vice versa. So, take a
bidirectional graph with different costs.
IV.Route Generation
From the Dijkstra algorithm, output is obtained in the form of a list. Again, the list
is shown visually on the map generated. The route is highlighted with any specific
color.
