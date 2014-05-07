# Introduciton

## Start with the Workshop Description

The scalability, availability and usability of software used in scientific workflows strongly influence the pace and direction of research in ecological forecasting.  Many independent scientists, groups, and development teams have developed customized software to enable ecological synthesis and prediction. We are looking ot move to the next step, so that scientists can transition from developing their own workflows to sharing solutions. (perhaps an analogy to some well-enginered piece of lab equipment - Licor, GC/MS, etc, etc. - no one builds their own any more, at best you have one or more highly trained operators. 

This paper will address many of the motivations and obstacles shared among these groups. _yes, but we want to be speaking to a larger audience here_ To do so, we focus on existing opportunities for interoperability and define a future path toward more modular and interoperable software and data. Focus on interoperable data and models and uncertainty accounting will provide the foundation for integrating models, data and statistical methods used in data-assimilation and prediction workflows. Challenges include allowing common systems for model specification, algorithm control, and output processing from these different systems so that they can be used more modularly as part of a complete workflow.

The key objectives of this workshop are to identify solutions that exist or are under development, especially those which would benefit from collaboration. In addition, we plan to build new organizational networks and community resources. Ultimately, these will reduce redundancies, leverage community participation, and produce the next generation of more modular, extensible software that will advance scientific discovery.  Specific outcomes will include a) a website through which to share resources and establish standards b) one or more papers on current state and future prospects of ecological forecasting software, c) plans for integration of existing tools and d) future collaborations.


## Some Definitions:
 * workflows
 * provenance
 * reanalysis, prediction, hyptohesis generation and testing
 * simulation models
 * model-data synthesis
   
Examples:

from simple (R) to complex (ARIES, \cite{Villa_2014}) 

* R ... start here because it has broad familiarity
 * Automated provenance tracking w/in R (e.g. analytic web)
    * R as a workflow itself - this is essentially folks using knitr with markdown or latex - which has very little structure other than separating text from code blocks
    * Kepler modules as frontend to R code


High Performance Computing, Big Data, 
   * Parallelization of code; access to different scheduler engines; evolving landscape
   * Workflow branches based on needs of node (e.g. I/O, flops, ram)
     * helps w/ scalability. 
   * Uncertainty, multi-scale coupling
     * how to couple independent codes; model-to-model coupling; transformation


## Big Questions / Objectives 

### Where will be be in 5-10 years

and what can we be doing now to get there