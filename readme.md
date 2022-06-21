GIS

Intial info: 
https://github.com/aariste/GeoJSON-Mapas 
https://datatracker.ietf.org/doc/html/rfc7946

Resources:

https://www.cursosgis.com/pasos-para-crea-una-aplicacion-webgis-profesional/

https://mothergeo-py.readthedocs.io/en/latest/development/how-to/gdal-ubuntu-pkg.html

http://www.sarasafavi.com/installing-gdalogr-on-ubuntu.html

Un ejemplo de importación de un GeoJSON a PostGIS con ogr2ogr:
ogr2ogr -f "PostgreSQL" PG:"dbname=eus_geodb host=localhost port=5432 user=postgres password=postgres" "municipios_eus.geojson" -lco GEOMETRY_NAME=geom -lco FID=gid -progress
