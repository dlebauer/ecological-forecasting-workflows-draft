## Examples

### Workflow Software

from simple (R) to complex (ARIES, \cite{Villa_2014}) 

* R ... start here because it has broad familiarity
 * Automated provenance tracking w/in R (e.g. analytic web)
    * R as a workflow itself - this is essentially folks using knitr with markdown or latex - which has very little structure other than separating text from code blocks
    * Kepler modules as frontend to R code
* Summary of workflow software from meeting ... what would a 'feature' matrix look like?


### Data Conventions
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


### Model Coupling

* what we currently do: CLM + DayCent; BioCro + DayCent
* A better approach
 * CCF1
 * SUMO \cite{van2011multi}
 * 

### High Performance Computing, Big Data, 
   * Parallelization of code; access to different scheduler engines; evolving landscape
   * Workflow branches based on needs of node (e.g. I/O, flops, ram)
     * helps w/ scalability. 
   * Uncertainty, multi-scale coupling
     * how to couple independent codes; model-to-model coupling; transformation
