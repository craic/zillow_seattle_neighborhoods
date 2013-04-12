# zillow seattle neighborhood maps

The good people at [Zillow](http://www.zillow.com/) have invested a lot of time defining the boundaries of around 7,000 neighborhoods in cities around the USA.

These are in the form of [ESRI ARC Shapefiles](http://en.wikipedia.org/wiki/Shapefile) that can be used as overlays on maps.

You can find these at [Zillow Neighborhood Boundaries](http://www.zillow.com/howto/api/neighborhood-boundaries.htm).

Zillow have kindly made these available to the rest of us under a [Creative Commons license](http://creativecommons.org/licenses/by-sa/3.0/). This allows you to share and modify the data but you need to attribute Zillow and must distribute any derivative forms of the data under the same or similar licenses. Attribution should take the form of including their logo with a link back to their site.

ESRI shapefiles can be read by many types of mapping software, but one big exception to this is [Google Maps](https://maps.google.com/). Overlays in Google Maps are loaded from [KML format](http://en.wikipedia.org/wiki/Keyhole_Markup_Language) files. In addition [GeoJSON](http://www.geojson.org/) is a JSON-based format that is gaining in popularity.

I needed neighborhood boundaries for the City of Seattle in KML format so I can use them in Google Maps. I couldn't find a convenient way to convert from Shapefile directly to KML (although these do exist in some GIS packages) and the solution I came up with involved converting first from Shapefile to GeoJSON and them from GeoJSON to KML. I'll make that software available elsewhere.

This site contains the GeoJSON and KML files for the 78 Seattle neighborhoods defined in Zillow's dataset.

The same approach could be applied to derive GeoJSON and KML files for the entire Zillow US city dataset. I'll see if I can do that in the future... for now it just covers Seattle.


The KML format contains not only data but also styling information. This can be viewed as a benefit or disadvantage of the format. The KML files here all use the same styling information in the XML blocks at the top fo the file. Look for the strings 'ff000000' for the Line Style and '7FAAAAAA' for the fill style. It would be easy enough for you to modify these as needed. Check the KML documentation for guidance on KML styling.



Example page showing the KML datasets


Two things to note about testing KML overlays in Google Maps.







