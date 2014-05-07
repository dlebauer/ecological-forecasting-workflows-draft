## Examples

TODO: Write Examples

* Data Conventions
 * MsTMIP -> widely used format by terrestrial ecosystem modelers
 * DataOne: EML describes data as it is, rather than requiring a standard example
 * NEON: has opportunity to provide data "templates" for common types of data collected by ecologists 
  * under development these, not clear that they should set 'the' standard
  * a good place for community feedback on this
  * tradeoff between generality and specificity
 * Aaron Ellison: the first three columns should always be x,y,t (z if relevant); on one hand, of course this isn't normalized; on the other hand, this is a straightforward rule.
* Coding conventions
* Code use/ reuse

### rOpenSci
 * rnoaa -> MsTMIP format
 * taxize -> USDA plants [Genus Species ScientificName CommonName) and BETYdb ([genus species scientificname commonname)  

* rOpenSci Getting data into R: what do workflows need?
 * How can we standardize data formats?
 * EML (ecological metadata language), NeXML (http://www.nexml.org/)
 * estimates of uncertainty / data quality
 * uniform API for multiple sources of data - we're working on this, so far we have 
  * taxonomy (from e.g., NCBI, ITIS, etc.)
  * spatial data (from e.g. GBIF, BISON, iNaturalist, etc.)
 * EML package: can automatically push data and get do
  * Push to KNB/DataONE/FigShare repositories
  * R package eml: https://github.com/ropensci/EML
 * Would it help to write out netcdf files from our NOAA R pkg wrapper to use in other software? And for spatial occurrence data from spocc/rgbif/etc?
 * Data transformations we could provide? e.g, Interpolation of climate data from NOAA

### NEON 
 * community support for desired standards


### MIPS

Model intercomparisons are one of the key areas of future application

### Model Coupling

* what we currently do: CLM + DayCent; BioCro + DayCent
* A better approach
 * CCF1
 * SUMO \cite{van2011multi}