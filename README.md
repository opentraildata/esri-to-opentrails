esri-to-opentrails
==================

Tools for transforming your data to the [OpenTrails](http://opentraildata.org) spec with [ArcGIS](http://arcgis.com). These tools will help you get your data into a place to use the [OpenTrails Converter](http://open-trails.codeforamerica.org/). The Converter is still in active development, on GitHub [here](http://open-trails.codeforamerica.org/).

As of right now, this repo contains the following:

###openTrails.gdb
Contains a skeleton Esri File Geodatabase for either copying, appending, or loading your existing features into. To ensure no loss of attribute data, use the append toolbox tool wich includes attribute mapping. Within an edit session, the load features tool will perform the same action.  

###opentrailsschema.xml  
Using the Import XML Workspace Document toolbox tool, this file will create the skeleton file geodatbase features within a new file geodatabase or an existing file geodatabase or feature dataset.  

###emptyShapefiles.zip  
This zipfile contains skeleton shapefiles for transforming your data into.  

###esri2OpenTrails.tbx
An ArcToolbox containing tools and python scripts for data transformation to the open trails spec. This will soon (hopefully) be replaced with a Python script, per [this issue](http://github.com/opentraildata/esri-to-opentrails/issues/1).
   * Append - copies features with attribute mapping
   * Concatenate Row Values - concatenates the row values for a specified field
   * Delete Identical - Deletes records in a feature class or table which have identical values in a list of fields
   * Esri To Open - will convert either a shapefile or feature class to GeoJSON [Via Project Open Data](https://github.com/project-open-data/esri2open)
   * Generalize - Simplifies the input features using the Douglas-Peucker simplification algorithm  
   * Import XML Workspace Document - this file will create the skeleton file geodatbase features within a new file geodatabase or an existing file geodatabase or feature dataset  
   * Spatial Join - Joins attributes from one feature to another based on the spatial relationship.  

###todo
   * a lot
   * no really
   * beef up initial description
   * add links to Esri docs for toolbox/tool names
   * QA/QC existing descriptions

To contribute, check out or open an [issue](http://github.com/opentraildata/esri-to-opentrails/issues).
