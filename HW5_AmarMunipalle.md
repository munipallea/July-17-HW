![](toronto.jpg)

# Dashboard of Toronto Real Estate Market based on 2001,2006,2011 and 2016 census data

## Welcome Sheet:

Introductory sheet with a stunning of TOR at night accompanied by an inspiring quote by Prince highlighting the city's soul and diversity.

## Welcome

Uses MAPBOX API to present a cartographic view of average price by neighbourhood. Size of each dot represents average house value (larger the value, bigger the dot); the associated monthly shelter costs are coded on a continoux color palatte. Thus a large dot with a 'blueish' tinge represents a price with higher than average value and associated shelter costs. Hovering over a 'dot' presents additional detail on underlying price distribution including average house value, shelter costs and geospatial information by neighbourhood.

[mapbox](mapbox.com)


## Shelter vs. Owned

This tab includes line charts produced on bokeh. (link to bokeh)
They represent average monthly shelter costs for owned and rented dwellings and also average home values. The correlations between these series are obvious. Uptrending home price values have resulted in higher shelter costs for both owned and rented accomodations creating likely an affordability problem. Shelter cost appreciation has grown significantly in relation to wages and inflation.


## Supply vs Demand

Uses bokeh to compare increase in TOR population and the corresponding increase in housing supply. A visual examination of graph suggests that housing supply has moved in pace with population increase; implying that atleast a portion of the price increase could be attributed to some speculative activity and not supply constraints. Per Analyticsvidhya 'Bokeh is a Python library for interactive visualization that targets web browsers for representation. This is the core difference between Bokeh and other visualization libraries. Look at the snapshot below, which explains the process flow of how Bokeh helps to present data to a web browser.' This explains the power of these graphs.


## Top Expensive Neighbourhood

1. This graph relies on hvplot to present top expensive neighbourhoods in terms of average price. HVPLOTs rich feature set including ability to zoom, pan, hover and save images are presented with side bar buttons. Users are urged to click on these links.
2. Sunburst plots visualize hierarchical data spanning outwards radially from root to leaves. The sunburst sector hierarchy is determined by the entries in labels (names in px.sunburst) and in parents. The root starts from the center and children are added to the outer rings.Sunburst chart orders shelter costs, by neighbourhood, by year in a hierarchial manner. Clicking on chart provides a deep dive on any particular year. Colour palette on the side provides a continuum of costs (lighter is more expensive).Reset back to original graph acheived by clicking again on the sunburst graph.


## Yearly Market Analysis

This tab includes 4 bar charts produced on bokeh represent market supply of housing stock by category. For each year, dwelling types e.g. detached, condos are presented. While on an upward trend, number of dwelling types have not kept pace with price moves indicating that a shortage of supply has impacted .


## Neighbourhood Analysis

This tab includes three panes
1. Average Home Value by neighbourhood across all neighbourhoods and years. By clicking dropdown menu user can choose neighbourhood of choice
2. A facet bar graph partitions a plot into a matrix of panels. Each panel shows a different subset of the data - in this facet each panel shows average price by TOR neighbourhood at 4 data points at 5 year intervals - 2001,2006,2011 and 2016. The side colour palette presents a visual identification of ranges.The facet provides an ability to compare several data points (4years * appx 100 neighbpurhood) in a single image and greatly supports trend analysis. In this case the secular trend of increasing home prices across all neighbourhoods in TOR.
3. Dwelling type (e.g. row house, semi-detached) by year and neighbourhood to visualize trends at the neighbourhood level


Sources:

[Statscan](https://www12.statcan.gc.ca/census-recensement/2011/as-sa/fogs-spg/Facts-cma-eng.cfm?LANG=Eng&GK=CMA&GC=535)
