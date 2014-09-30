esri-to-opentrails
==================

Tools for transforming your data within Esri software to the open trails spec.  

###openTrails.gdb
Contains a skeleton Esri File Geodatabase for either copying, appending, or loading your existing features into. To ensure no loss of attribute data, use the append toolbox tool wich includes attribute mapping. Within an edit session, the load features tool will perform the same action.  

###opentrailsschema.xml  
Using the Import XML Workspace Document toolbox tool, this file will create the skeleton file geodatbase features within a new file geodatabase or an existing file geodatabase or feature dataset.  

###emptyShapefiles.zip  
This zipfile contains skeleton shapefiles for transforming your data into.  

###esri2OpenTrails.tbx  
ArcToolbox containing tools and python scripts for data transformation to the open trails spec.
   * Append - copies features with attribute mapping
   * Concatenate Row Values - concatenates the row values for a specified field
   * Delete Identical - Deletes records in a feature class or table which have identical values in a list of fields
   * Esri To Open - will convert either a shapefile or feature class to GeoJSON [Via Project Open Data](https://github.com/project-open-data/esri2open)
   * Generalize - Simplifies the input features using the Douglas-Peucker simplification algorithm  
   * Import XML Workspace Document - this file will create the skeleton file geodatbase features within a new file geodatabase or an existing file geodatabase or feature dataset  
   * Spatial Join - Joins attributes from one feature to another based on the spatial relationship.
