# Example for participatory planning in the town Zug, Switzerland

Link to the application: [participatory-planning-zug-brueggli](https://esri.github.io/participatory-planning/?settings=https://raw.githubusercontent.com/SaschaBrunnerCH/participatory-planning-zug-brueggli/main/participatory-planning-settings.json)

Based on the application from https://github.com/Esri/participatory-planning

Steps to create a new participatory planning application for switzerland:
1. Create an account on www.arcgis.com
2. Create a [WebScene](https://doc.arcgis.com/en/arcgis-online/get-started/get-started-with-scenes.htm) with [SceneViewer](https://www.arcgis.com/home/webscene/viewer.html)
   - Use Basemap [Imagery](https://www.arcgis.com/home/webscene/viewer.html?layers=10df2279f9684e4a9f6a7f08febac2a9) with integrated [SWISSIMAGE 10 cm](https://www.swisstopo.admin.ch/de/geodata/images/ortho/swissimage10.html) from Swisstopo
   - Design your own Basemap to draw on with [ArcGIS Vector Tile Style Editor](https://developers.arcgis.com/vector-tile-style-editor/) or use the existing one [Participatory Planning Vector Tile Layer](https://zurich.maps.arcgis.com/home/item.html?id=5cf1abb43c25482e8a9e373953498999)
   - Use [Scenelayer: 3D Buildings Switzerland](https://www.arcgis.com/home/item.html?id=a714a2ca145446b79d97aaa7b895ff95) published by Esri Suisse based on the Swisstopo data [swissBUILDINGS3D 2.0](https://www.swisstopo.admin.ch/de/geodata/landscape/buildings3d2.html) published 
   - Read the Blog ["Swisstopo-Präzision in Esri Grundkarten und 3D Diensten"](https://arcgis.esri.de/swisstopo-praezision-in-esri-grundkarten-und-3d-diensten/) for more information about the data
4. Create an account on www.github.com
5. Create a new repository or create a [GitHub Gist](https://gist.github.com/) for the configuration-file
6. Create a [configuration-file](https://github.com/Esri/participatory-planning/blob/master/CONFIGURATION.md) with the following content:
   - `planningArea` contains the Web Mercator coordinates of the planning area
   - `planningAreaName` is the name of the area shown in the welcome screen of the app
   - `webSceneId` point to the webscene created above
