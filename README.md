# H3
H3 Geospatial Indexing System by UBER
Installation of H3 library and other details of H3 could be found in this Git Repo - https://github.com/uber/h3


This file lets you convert a list of H3 hashes to a Geojson File.
This Geojson file could be directly used in QGIS for visualization.


# H3 to Geojson:

Having said you have a file (CSV or TXT) containing list of H3's , you could use this script to convert them to Polygons which can be visualised in QGIS, etc..,

Sample:
-----

ID,H3_lv9

001,89be455030bffff

002,89be455a9d7ffff

003,89be712e0d7ffff

004,89be712e187ffff

005,89be713b00bffff

-----


# Geojson to H3:

Providing a Geojson file (Polygons, not MultiPolygons) these polygons are converted into H3 hashes for whichever resolution you want it in.

Sample:
-----

{ "type": "FeatureCollection", "features": [ 
{"geometry": {"coordinates": [[[144.24458943898117, -36.81068932659823], [144.24424589601577, -36.808741307215], [144.24198873049681, -36.807999331551756], [144.2400750480967, -36.80920533649371], [144.240418486149, -36.811153350732056], [144.2426757115154, -36.811895365174685], [144.24458943898117, -36.81068932659823]]], "type": "Polygon"}, "properties": {"H3_9": "89be455030bffff", "ID": "001"}, "type": "Feature"},
{"geometry": {"coordinates": [[[144.26713886048103, -36.733684574830974], [144.26679506910068, -36.73173640426567], [144.2645396522763, -36.730995101320666], [144.26262796702395, -36.732201930160066], [144.26297165369925, -36.734150095642825], [144.26522713033287, -36.73489143737008], [144.26713886048103, -36.733684574830974]]], "type": "Polygon"}, "properties": {"H3_9": "89be455a9d7ffff", "ID": "002"}, "type": "Feature"},
{"geometry": {"coordinates": [[[146.00818827144815, -36.546935805742336], [146.00780093220138, -36.54498643436366], [146.00552062365446, -36.544276433835954], [146.0036275890673, -36.545515768336095], [146.00401482491515, -36.54746513887627], [146.00629519875042, -36.548175175756164], [146.00818827144815, -36.546935805742336]]], "type": "Polygon"}, "properties": {"H3_9": "89be712e0d7ffff", "ID": "003"}, "type": "Feature"},
{"geometry": {"coordinates": [[[145.96912023231013, -36.55488232848217], [145.9687338468292, -36.55293297014657], [145.96645395343177, -36.552222248357126], [145.96456038034188, -36.553460848496414], [145.96494666237933, -36.55541020589771], [145.96722662095146, -36.556120964095406], [145.96912023231013, -36.55488232848217]]], "type": "Polygon"}, "properties": {"H3_9": "89be712e187ffff", "ID": "004"}, "type": "Feature"},
{"geometry": {"coordinates": [[[146.38615304889177, -36.594408365781064], [146.38575589142212, -36.59245911826116], [146.38346814561754, -36.591755758435575], [146.38157749070078, -36.5930016103783], [146.38197454489836, -36.59495085797025], [146.3842623572862, -36.59565425354879], [146.38615304889177, -36.594408365781064]]], "type": "Polygon"}, "properties": {"H3_9": "89be713b00bffff", "ID": "005"}, "type": "Feature"} ] }

-----


Sample Images of H3 (Resolution 12 and 13)

![Test Image 4](https://github.com/kapil-grv/H3/blob/master/H3-lv12_13_sample.png)
