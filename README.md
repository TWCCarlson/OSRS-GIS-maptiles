# OSRS-GIS-maptiles
Tilemap images of the OSRS world

# Purpose
This repository serves as a raw data source for usage in Leaflet or similar GIS mapping frameworks. Use 
`https://raw.githubusercontent.com/TWCCarlson/OSRS-GIS-maptiles/master/0/{z}/0/{y}/{x}.png`
as the source URL for Leaflet's `tileLayer` to access the tiles.

# Method
Files were generated using PIL for image rescaling (quality is preserved) and `pyvips`'s `dzsave` (for speed, gdal2tiles.py works but is excruciatingly slow).