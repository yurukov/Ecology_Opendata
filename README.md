Ecology related opendata
==============================

#####Data

The data is scraped from the Bulgarian national [registry](http://pdbase.government.bg/forms/public_eprtr.jsp) for industial installations handling or emitting pollutants. It covers all emissions and pollutant transfers in air, water and soil between 2007 and 2012. Most of the data until 2011 is also available in RDF format in the [E-PRTR](http://prtr.ec.europa.eu/TimeSeriesPollutantReleases.aspx). I scraped the national database for ease of use and more full data. 

#####Visualization

The page contains several charts that how a map with all polluting sources, list of pollutants, amounts, tendencies over time, statistics on measurement and estimation. The data on exact estimation metodology and source production type is not shown. The charts are filterable. Zooming and panning the map selects a region and the respective sources. The tables with pollutants allow selecting specific emissions.

#####Implementation

The charts are based on DC, Crossfilter, D3 and Leaflet. I've extended the dataTable chart of DC and created a new chart wrapper for a Leaflet map. The markers in the map detect the zoom level and show icons on greater zoom. On smaller zoom level it shows a "damage area" for the biggest polluters. That circle is scaled according to the zoom level to always cover the same area.

#####Demo:

[http://opendata.yurukov.net/ecology/en](http://opendata.yurukov.net/ecology/en) (English)

[http://opendata.yurukov.net/ecology](http://opendata.yurukov.net/ecology) (Bulgarian)

#####Latest data:

[http://opendata.yurukov.net/ecology/data](http://opendata.yurukov.net/ecology/data)




