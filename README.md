# qgis-basemaps
A collection of several basemaps in an xml file.

Add `58` basemaps on `QGIS` by right click on XYZ Tiles and load connections.
If you want to add some of the basemaps it's free to make a PR.

Template: 
```
<xyztiles url="...?x={x}&amp;y={y}&amp;z={z}" password="" name="NAME of BASEMAP" referer="..." zmax="19" authcfg="..." username="..." zmin="0"/>
```

To remove all the connections at once. You can use the following code:
```
settings = QgsSettings()
settings.remove('qgis/connections-xyz')
iface.reloadConnections()
```

Note:
Copyrights of the map are the sole responsibility of the user.

A nice script to add basemaps via python console: 
https://github.com/klakar/QGIS_resources/blob/master/collections/Geosupportsystem/python/qgis_basemaps.py