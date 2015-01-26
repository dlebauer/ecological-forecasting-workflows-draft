# Discussion

### Some discussion topics raised during workshop

* Needs from workflow engines in the future
* Why we haven't adopted a common workflow system
* Standardising across data formats and model input output formats
* Benchmarking models against multiple datasets
* Model intercomparisons
* Red flag systems for when data and model outputs are differing from expected behaviours
* Adding semantics to model and data inputs and outputs and probabilities
* Metadata standards that will work for ecological forecasting
* state of reproducibiilty
* best practices data life cycle


### Open Questions

* Metadata/data standardization and interoperability
  * how to define and share probabilistic results?
  * easier to describe 'data' than model output

## Moving Forward (5-10 years)


### Parallel, Sequential, and Synchronized modeling

Modularity and Interoperability.

What will / do integration of heterogeneous _codes_ as well as _data_ look like? 

* MIPS are parallel workflows (e.g. differen models of the same)
* What about sequential workflows (of complex simulation models) of, e.g. met dynamical downscaling -> ecosystem -> economics models? New opportunities for cross-domain optimization and propagation of uncertainty (e.g. dynamically coupled codes are easier to link as stocahstic equations).
* Synchronized models (e.g. where models overlap in some but not all outputs, e.g. 1) SUMO \cite{van2011multi} (climate models). This can be done, an alternative to model 'coupling', e.g. with CLM, 




* leaders, where to look (rOpenSci, SSI, everyone's projects), which niches each of these fill
* 


_Matt Jones ... _

What do we need to do to up our game, computationally, in producing actionable predictions of ecosystems - data input standards, workflows, probabilities, cloud

* We talked for a long time about this but ultimately decided that the scope is on par with the Software Sustainability Institute, rather than a paper like this. 
* But what are some of the key points (and how will the SSI help solve these?) (covered by Matt's talk ... 


Other things ...
 * in R: Commit to S4 classes instead of S3, all languages: well-specified APIs, contractual committment
 * continuous integration e.g. Travis-CI (or is this too high level?)
 * testing (too high level?)
 * 





## Conclusion

The key objectives of this paper were to identify solutions that exist or are under development, especially those which would benefit from collaboration.

... reduce redundancies, leverage community participation, and produce the next generation of more modular, extensible software that will advance scientific discovery.  
