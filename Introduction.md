## Big Questions / Objectives 

Proposal of what to work on

1. High profile perspective on the needs to get towards reproducibility in the prediction of complex multicomponent systems - for which ecological systems are a prime example but Earth System Models are another - and how advances in workflow technology are needed to achieve that - potentially with a section on case study examples of where we really need this reproducibility in order to keep advancing. Tailed by 5-10 year goal for the development of workflow technology to meet the needs of ecological / earth system research.
2. Discuss further how the specifics of conducting multicomponent multi-dataset inference based research raises new challenges for developing workflows.
3. Discuss the challenges of managing multi-component modelling with workflows 
4. A semantics for decribing workflows? Needed? Helpful?

### Where will be be in 5-10 years

and what can we be doing now to get there

Formal computational workflows rarely prominently feature in scientific research outputs, even if they were part of the research methodology. 
Most benefits from adopting computational workflow software are obvious, such as clarity, automation and accessibility. 
Many of the costs are also well known, such as inflexibility and efficiency. 
Despite these advantages, a number of recent studies in computational environmental sciences have developed their own project-specific workflow solutions  from scratch rather than adopting one of many existing workflow software (e.g. Kepler, Taverna, etc) that have been created specifically to meet these needs. 
These workflows share many common features, but are diverse in the specific features that are implemented. 

Here we analyse why similar scientific workflows have been reinvented so many times and show that this redundant effort highlights the absence of any single software with the essential features required to meet the demands of modern computational inference.
Building on this, we identify the following features that the next generation of workflow software must possess in order to meet the demands of the inference age. 

1. the separation of model structures, parameters and driver datasets 
2. support for multiple modes of abstraction within the same model structure 
3. the ability to overlay a traceability framework over model structures and monitor model behaviour on the basis of such a framework  
4. support for a variety of inference libraries, 
5. the adoption of a provenance tracking rather than workflow paradigm 
6. the ability to structure computational workflows hierarchically 
7. distributed version control for models and data 
8. distributed and cloud based data access and retrieval
9. remote computation and 
10. a richer variety of data and model component interfaces.
