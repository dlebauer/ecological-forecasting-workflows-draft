**TODO** Parse into sections above

### NOTES MADE DURING MEETING 1
 * Topics

   * Benefit from having a large enough project to work with
     * e.g bioinformatics -> bioKepler
     * openTopography.org
    
Statistics
   * Developing worksflow models for data-constrained models of systems.

   * Finite  state machine as model to model communication
   * UVCDat http://uvcdat.llnl.gov/
   * Bob Cook: MstMIP / model intercomparison
 
   * Anticipate key workflow/software needs for 5-10 years time
   * Workflows as a means to get the community to work together
   * If ecological forecasting is to become a reality - we need workflows to deliver that
   * Model component interoperation  - going from molecules to blue whales
   * Models (and model components) as hypotheses
   * Benchmarking models <- a perfect place for workflows
   * Scenario testing
   * Having WF system handle uncertainty would be useful
   * Need mechanism to represent model outputs and model performance
   * Identify translators for model inputs & outputs
   * e.g. Adopt MSTMIP standards for variables 
   * merging across scales 
   * end to end modeling -> is there any meaning to this?
     * Beth Fulton, Ken Rose
     * don't do it; not sufficiently adaptable
     * keep it simple, solve one prob. at a time
     * keep data in native format rather than homogenize
   * What are the low hanging fruit?
   * Optimal levels of complexity in workflow 
     * also, model complexity
   * Detection of scale shifts, using scale as object of observation
     * Auto characterisation of sig changes in ecological data and model predictions.
Identifying red flags in data observations  and model predictions
   * Transparent / efficient access to data, computing <- ability to combine both in a transparent way
   * provenance tracking -> captured as reproducible research objects
   * adopting best practices w/in community
   * business model to sustain software; combining big, heterogeneous data, 
   * references: Madin 2007, Madin 2008, Berkeley 2005


Day 2 Discussion
-------------------------
 * Why have so many groups decided to create their own workflow rather than adapt an existing system?
   * Are ecological demands on wf systems special?
 * Can we describe model components semantically to provide plug-n-play within wf systems?  
 * What are the key barriers to plug-n-play ecological forecasting?
   * Getting data providers online to not only provide read, but also write access through open APIs
   * Provide mechanism to describe a desired standard data product
     * Can be the target of data transformation as input to a model, or can describe existing raw data to decide which are transformable to that target
   * Licenses? (e.g., ESA ecological archives has unclear licenses for reuse)
   * Lack of well-specified interfaces to model components; 
Standard grammars for defining data-data and data-model and model-model interfaces


Proposal of what to work on

1. High profile perspective on the needs to get towards reproducibility in the prediction of complex multicomponent systems - for which ecological systems are a prime example but Earth System Models are another - and how advances in workflow technology are needed to achieve that - potentially with a section on case study examples of where we really need this reproducibility in order to keep advancing. Tailed by 5-10 year goal for the development of workflow technology to meet the needs of ecological / earth system research.
2. Discuss further how the specifics of conducting multicomponent multi-dataset inference based research raises new challenges for developing workflows.
3. Discuss the challenges of managing multi-component modelling with workflows 
4. A semantics for decribing workflows? Needed? Helpful?


Publishing derived data sets. 
Automated data input and output (e.g. what NEON is working on)

ncML - 

Top 10 blockers/necessary developments to plug-and-play ecosystem forecasting: key development requirements for the next 5-10 years

Achieving greater levels of interoperability:


Paper Outline
---------------------


Titles:

* "Reproducibility in ecological and environmental modelling: whether and why scientific workflows, and where next?"
 * "Software practices that promote interoperability {and reproducibility} for ecological forecasting"

* rhetorical approach framework
 * name and define practice
 * what do you want to achieve and how to get there
 * pros and cons
 * examples

Outline/Topics

 * Intro general background of sw best practices (e.g., White paper), plus acknowledge these are well-established software engineering practices
 * Discussion of desiridata: Reproducible, Traceable, Usable, Comparable, {Reusable}
   * define the terms
   * why are they useful
     * within context of increasing applied relevance
     * increased efficiency within research groups
     * building community: standing on shoulders of giants
 * Recommended Practices (pros, cons/limitations, benefits, example of use); presented in heirarchy of stages ... 
   * Version and archive and share code
     * Gists versus repos versus releases
   * Use Functions: abstract and generalize, DRY
     * Example from eco forecasting
   * Well-specified interfaces (APIs) and modules
     * Consistent contracts between modules
     * Hooks for other software to interact
     * Version control of APIs and modules
     * Example from eco forecasting
   * Avoid letting implementation leak into interface
     * e.g., JAGS requires integer site names for iteration, constraining data inputs
     * e.g., weather downscaling algorithm that works based on column order or specific naming conventions
   * Automate data processing (not in Excel)
     * Auditable, repeatable
     * Example
   * De-couple data from code: use data repository APIs, use open, portable data representation formats {like CSV, and NetCDF}
     * No hard coded paths
     * Isolate data I/O in separate modules (e.g., a) call to the web, collect raw payload, b) downstream processing)
     * References to data in *accessible* repository systems (e.g., via DOI)
     * Deal with access control issues (public versus private examples)
     * Version control of data (e.g., DataONE, dat, ...)
     * See diatribes about reasons to share data
     * Example from eco forecasting
   * Use a consistent error handling and propagation strategy
   * Use composable workflow systems (e.g., R, Kepler) to link components
     * Benefit: reuse and mix and match modules for various applications
     * Benefit -- documents end-to-end process
     * Example: Benefit of Automation: show LeBauer example of automation
   * Document the workflow and process and code
     * Use literate programming to link implementation to documentation
     * Doxygen, ROxygen, knitr
     * write for humans; clear variable names
   * {Provide License and metadata} - or can we ref this in other papers?
   * Formally test models
     * Separate unit and integration testing
     * Test with a wide variety of data bounds / prevent decline of model skill
   * Be aware of scaling and integration choices, use broker/wrapper components to couple components that operate at multiple scales or rates
     * Expose module constraints in documentation
       * e.g., scale constraints, normality constraints, etc.
   * Report uncertainty in input and output data
     * Can we recommend specific uncertaininty representations, or at least list them?
     * A typology of uncertainty measures, with a serialization approach
 * Education/Workforce dev and Collaboration topics? 
   * Need to train EES students e.g., software carpentry as starting point
   * Build on this with the best practices
 * Error handling (See recommendation above -- should this be in the recs section?)
   * useful messages
 * examples and/or case studies (or integrated into practices above)



