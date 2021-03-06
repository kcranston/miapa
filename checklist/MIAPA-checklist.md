MIAPA Checklist
===============
The MIAPA (minimum information about a phylogenetic analysis) checklist details the list of metadata necessary for researchers to evaluate or reuse a published phylogeny.


The Checklist
-------------

   * Topology
      * The topology itself, possibly as an identifier of a database (such as a !TreeBASE) record 
      * Is this a gene tree or species tree?
      * It is a tree or a network?
      * Is topology rooted or not?
      * The type of consensus if this a consensus topology (that summarizes the topology inference in some way, rather than being directly provided by the inference method)?
      * The topology should be "well described", as applicable to the inference method being used. For example, a likelihood for maximum likelihood analysis. For Bayesian analyses this should also include the burn-in period excluded, and the convergence of the chain(s). This may also include more then one topology, for example a sample from the posterior probability distribution for Bayesian, or equally scoring topologies for a maximum parsimony analysis. 
   * OTUs: All terminal nodes should be appropriately labelled and referenced in one of the following ways. Internal nodes need not be.
      * A meaningful external identifier (a combination of database or resource and identifier/accession within that database).
      * For specimens, museum, collection (if applicable), and specimen identifier. Alternatively, if a specimen is not in a museum collection, use the laboratory, laboratory collection, and accession within that collection.
      * Precise (GPS) georeferences for specimens are highly desirable (but not always available). 
   * Branch lengths: Some measure of branch length required unless it is not applicable to the analysis method.. Further semantics of the measure should be implied by the tree inference method. 
   * Branch support: Some value of branch support should be provided, for example posterior probability, or bootstrap value, unless it is not applicable to the analysis method.
   * Character matrix: aligned data matrix that is the basis for the tree (by having been the input for the tree inference method)
      * Data type must be provided, for example DNA, RNA, protein, morphology, etc.
      * For molecular matrices, the accession numbers (and respective database(s) if different from Genbank) of the sequences used for each row must be provided.
      * a mapping that relates each row identifier to a tip of the topology
      * a mapping that relates each accession number or specimen identifier to a row label
   * Alignment method
      * name of software used, version of program
      * parameters used (or default if default values were used).
      * whether alignment was manually corrected or edited
   * Tree inference method
      * name of software used, version of program
      * parameters used, including model of evolution, and optimality criterion
      * character weights if (normally then morphological) characters were weighted. (Typically, inference programs provide these in their log files, and thus the information could be copied from there.)

