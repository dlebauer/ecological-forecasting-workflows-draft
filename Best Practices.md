# Best Practices in Ecological Computing (Appendix? Separate Paper?)

...intentional play on "Best Practices in Scientific Computing \cite{Wilson_2014}, which we should start by discussing.

_These are notes from a group brainstorm / wishlist about what we wish everyone else did. **should narrow focus on a meaningful contribution.** On the one hand, perhaps a valuable consensus and good information. On the other hand, a big scope, could be a separate paper, perhaps an appendix or perspectives piece. 'thoughts from the meeting' _

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



