# Outline / Proposed Paper Structure

## Title

Some options

* **Advancing Software for Ecological Forecasting**
* **Reproducibility in ecological and environmental modelling: whether and why scientific workflows, and where next?**
* **Advances in software to accelerate ecological and environmental inference**

## Definition & Aim

Ecological forecasting is predicting the future properties of ecological systems    

In this paper we will identify promising future software solutions accelerating the rate of production of useful ecological forecasts.

## Introduction

* A common goal in ecology and environmental sciences is to build useful predictive models of ecological systems
* Often in ecology and environmental sciences those models are of complex dynamical systems for which we have an incomplete understanding of how the system works or how easy it is likely to be to predict its behaviour
* Much endeavour is spent on understanding these systems better, with the stated intention to improve our ability to predict them into the future.
* However our discipline regularly finds itself in the situation of having multiple complex models of apparently the same thing making quite different predictions but with limited ability to understand model-data differences and model-model differences.
 * Model-data differences because using different datasets, or using datasets in different ways, or unclear processing of data, or assumptions behind the data
 * Model-model differences because of different models of different complexity without clarity about differences in effects of different formulations, or how the same assumptions were implemented differently etc.
* We also increasingly need to use models and data with formally quantified probabilities associated with them - this is especially in the spirit of ecological forecasting. However this increases computational complexity even more.
* What we need is the ability to conduct clean analyses of the sources and contributions of model-data differences and model-model differences. Ultimately many of us want to build better predictive models but get slowed down after a particular degree of model complexity by intractability and non-reproducible work.
* Improving complex models of eco-env systems can often be laborious and intractable and yet many of the problems targeted by research have a short deadline within which to provide solutions. Others are just being held back by an inability to rigorously test models.
 * CITE MIP's here and NEON 
* In relation to this there are many efforts to add clarity to the process of ecological and environmental analytics in general, from improved methods to access, and specify access to heterogeneous datasets, to being clear about model specifications and assumptions, to describing analytical workflows and to labelling outputs.
* However, there is still progress to be made
 * Elaborate on recent best practices papers (Wilson 2013, [Hampton et al 2014](https://peerj.com/preprints/549v1/))
* Here we take a detailed look at the research and development pipeline involved in developing ecological and environmental system models for ecological forecasting to identify key areas that we believe if improved would lead to major improvements in the production of useful ecological forecasts.
* Ultimately we want to reduce redundancies, leverage community participation, produce the next generation of modular and extensible software that will advance scientific discovery

##  What it takes to do Ecological Forecasting Well

(part of Introduction?)

\cite{Niu_2014}

## Data

* Data as inputs to models and analyses
 * Heterogeneous data access, use and citation, access from remote
* Data as outputs from models and analyses
 * Metadata etc..
 * What to do about probabilistic data
 * Also how to visualize and communicate uncertainty
* Propose an example data conventions to enable more widespread adoption and interoperability
	
## Modularity and Interoperability

_Matt Jones (Lead), with Ferdinando Villa, Jeroen  Steenbeek

* Ways to enable modularity in code components, list options and probability of success
 * e.g. well written and commented - limited
 * e.g. conforming to a DSL - restrictive
 * e.g. in the cloud as a service or compiled as an executable
 * e.g. a combination of these - yes, but realistic?
* Propose a code module interoperability convention.
* Example application: propose use of common photosynthesis libraries (Farqhar / Ball-Berry and alternatives + temperature scaling routines) that can be simultaneously used across scales (this is already done, but everyone implements them separately). This could facilitate more collaborative efforts, e.g. because user's of different models could contribute to the same library (e.g. adding additional functionality).

## Modeling Software

* Perhaps some sort of overview of the key ads and disads of common current software used in ecol forecasting pipeline, e.g. a top 10 software (R, MATLAB, FORTRAN, Excel, Kepler, Mathematica...)
 * (Aaron Ellison has done a search of software cited in ESA Journals, could this be extended to include compiled languages?) 
	-- Brian Inouye (FSU) has a larger (longer) more comprehensive dataset on software used in ESA journals, and is interested in joining this effort (AME talked with him at ESA)
 * The almost ubiquitous use of R and whether better to keep with it and make it better or highly recommend against it.
 * 	--R is hardly "ubiquitous", although it is used about 30% of the time in ecological publications
 * When are compiled languages used (and why?)
* Distil what we like of these into to what we would like and not like in future
* Model Intercomparison, Benchmarking [Andy Fox]

## Ontologies and Semantics 

_Ferdinando Villa (Lead), with Matt Jones, others_

* Definitions
* (How) Can O&S help us to connect models to models and data to models better than we do?
* What have ontologies and sematics done for us?
* Propose a minimal list of O&S conventions?
	
## Workflows and Provenance 

_link to Modularity and Interoperability section?_

* Focus on what new things we want and need from a WF or Prov.
* Briefly summarise what's great and what's not about WF;  Critiques of particular workflows? What works what doesn't?
 * Lack of well-specified interfaces to model components; 
 * technical barriers / learning curve
  * User interface GUI vs. programmatic. Level of Bugginess
 * project dependence on a particular software; 
 * difficulty selecting modular components from different systems, or flexibility to easily migrate
   * (for example, to chain workflows across domains, e.g. climate <--> ecology <--> economic model two-way coupling
* Why do groups decide to create new workflow systems rather than adapting an existing system?
  * Are ecological demands on wf systems special?
* The development of prov tracking
* Propose a list of WF&Prov features that would really accelerate ecological forecasting
 * Plug-and-play
  * What are the key barriers to plug-n-play ecological forecasting?
  * Can we describe model and data  semantically to provide plug-n-play within wf systems?  
 * Straightfoward User interface 
 * Standard grammars for defining data-data and data-model and model-model interfaces

## Computation and Cloud

* Different options for coupling code
* Are we saying any more than wanting to work with the cloud as if it's a permanently accessible alternative computer?
* Identify some key advances in cloud that would really help
 * The ability to archive VMs of exactly your computer's state when produced results
  * (Ilkay - SDSC has a new machine specifically for VM's?)
  * PEcAn distributed as VM's
  * iPlant now has a VM service
 * The production of data and code in the cloud
 * Remote access of data via cloud
 * Pushing processing to the cloud.

## Conclusions

TO BE DETERMINED

