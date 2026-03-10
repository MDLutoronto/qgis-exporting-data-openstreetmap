---
title: "Exporting Data from OpenStreetMap for QGIS"
layout: "home"
description: "In the case you need to acquire detailed city data to produce a large-scale map and we don’t have what you’re looking for in our data inventory, there is a chance that the user-contributed maps of OpenStreetMap.org may do the trick. QGIS can query and load this data into your map for a specified area of interest. The data can then be exported into common geospatial file formats."
staff:
    - name: Cole White
      link: https://library.utoronto.ca/staff/cole-white
created_date: 2023-12-08
permalink: "/"  #! Remove this if not the homepage
---

# Exporting Data from OpenStreetMap for QGIS

In the case you need to acquire detailed city data to produce a large-scale map and we don’t have what you’re looking for in our data inventory, there is a chance that the user-contributed maps of OpenStreetMap.org may do the trick. QGIS can query and load this data into your map for a specified area of interest. The data can then be exported into common geospatial file formats.

A third-party plugin called [**OSMDownloader**](https://plugins.qgis.org/plugins/OSMDownloader/) is available that allows for automatic retrieval of OpenStreetMap data for a specified area within the QGIS GUI. After the user interactively specifies an area of interest, this plugin will query and load OSM data into the map. The data can then be used for mapping in QGIS. It can also exported to a shapefile or other geospatial data format if desired.

1. Open QGIS and start a new project.
2. Go to **Plugins** -> **Manage and install plugins**

    <img src='{{ '/assets/images/image.png' | relative_url }}' alt='Under Plugins, select Manage and Install Plugins' title='' width='601' height='' />

3. Search for and install the plugin called '**OSMDownloader**'.

    <img src='{{ '/assets/images/image_0.png' | relative_url }}' alt='In the search bar, type osmdownloader' title='' width='606' height='' />

4. After installing the OSMDownloader plugin, a new button will appear on the toolbar.

    <img src='{{ '/assets/images/image_1.png' | relative_url }}' alt='OSMdownloader will now appear on the toolbar' title='' width='638' height='' />

5. Activate the tool and use it to draw a rectangle around your area of interest. (**Tip**: If you would like to add a basemap to help you visually locate your geographic area of interest, the [QuickMapServices](https://plugins.qgis.org/plugins/quick_map_services/) plugin will allow you to add tiled layers from Google, Esri, NASA, and others).

6. A dialog box will appear showing the coordinates of the extent you've just defined. Choose a save location for the OSM data. Check the 'Load layer after download' box. Click OK.

    ![Select a save location for your OSM data ]({{ '/assets/images/image_2.png' | relative_url }})

7. The OSM data layers will appear on the map and in the Layers pane.

    ![OSM data will appear on the map and in the layer panel on the left hand side ]({{ '/assets/images/image_3.png' | relative_url }})

Tools: [QGIS](https://mdl.library.utoronto.ca/tools/qgis) | Data Format: [Vector](https://mdl.library.utoronto.ca/data-format/vector)

