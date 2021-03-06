# QGIS Gazetteer Plugin

Adds a gazetteer search panel to QGIS 1.8 / 2.0 which by default searches [GeoNames](http://www.geonames.org/), [Yahoo (place search)](http://developer.yahoo.com/geo/geoplanet/) and [OSM Nominatim](http://wiki.openstreetmap.org/wiki/Nominatim) plus an [Astun Technology](http://astuntechnology.com) iShare address search.

## Available Gazetteers

All searches are performed via a web service call. The available searches can be configured in `gazetteers/config.ini`, each gazetteer requires a corresponding set of config / logic in it's own python file in `gazetters`.

The [qgis-gazetteer-search](https://github.com/mixedbredie/qgis-gazetteer-search) repository by [mixedbredie](https://github.com/mixedbredie) is a good choice if you'd like to roll your own search webservice such as one based on the LLPG (Local Land and Property Gazetteer) or LSG (Local Street Gazetteer) used in Great Britain.

## Installation

The plugin files need to live in a directory called `gazetteersearch` inside the QGIS Python plugins directory.

*Windows note:* The QGIS plugin directory should be under `C:\Documents and Settings\<Username>\.qgis2\python\plugins\` (Windows XP) or `C:\Users\<Username>\.qgis2\python\plugins\` (Windows +7).

*QGIS 1.8 note:* QGIS 1.8 stores it config under a `.qgis` directory.

### Using git

If you are using `git` then simply clone the repository into your QGIS python plugins directory:

    cd ~/.qgis2/python/plugins/
    git clone https://github.com/AstunTechnology/QGIS-Gazetteer-Plugin.git gazetteersearch

## Copyright and usage of gazetteers

### GeoNames

GeoNames data is licensed under [Creative Commons Attribution 3.0 License](http://creativecommons.org/licenses/by/3.0/), further details regarding usage can be found on the [GeoNames website](http://www.geonames.org/).

### Yahoo

Yahoo place search is subject to the [Yahoo! APIs Terms of Use.](http://developer.yahoo.com/terms/), further details regarding usage can be found on the [Yahoo GeoPlanet website](http://developer.yahoo.com/geo/geoplanet/).

### OSM Nominatim

Use of the OSM Nominatim search is subject to the [Nominatim usage policy](http://wiki.openstreetmap.org/wiki/Nominatim_usage_policy). OpenStreetMap data is © OpenStreetMap contributors and available under the [Open Database Licence](www.openstreetmap.org/copyright).
