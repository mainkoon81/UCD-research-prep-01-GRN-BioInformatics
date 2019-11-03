# Gene-Regulatory-Network

> Background?
 - __Reverse engineering of GRNs?__ 
   - In each type of cell, different genes are expressed (turned on) or silenced (turned off). By identifying which genes in the sick cells are working abnormally, doctors can better diagnose the ailment. One way they do this is to use a **DNA microarray** to determine the expression levels of genes. When a gene is expressed in a cell, it generates `messenger RNA` (mRNA). `**Overexpressed genes** generate more mRNA. This can be detected on the **microarray**`.
   - **Technologies** measuring **gene expression levels**(gene turned on) has created a database for inferring GRNs. However, the nature of these data has made this GRN inferring process very difficult and the large scale quantitative analysis on real biological datasets cannot be performed, to date, as existing approaches are not suitable for **real microarray data** which are noisy and insufficient.

 - __GRN Model__
   - The level of mRNA concentrations can be viewed as a snapshot of the genes expression levels under certain conditions. With a large enough set of snapshots, it should be theoretically possible to uncover the underlying gene regulatory network(GRN). 
   - **Modeling:** We can find parameters of the GRN model from available data. Once built, these GRN models can be used to predict the behaviour of the organism **under certain conditions**, related to different treatments or diseases(predict its behaviour under different conditions).
     - `genes` are viewed as **variables** that change their (expression) values in time.
       - Depending on the type of variables used, methods can be classiﬁed as discrete or continuous, deterministic or stochastic, or as hybrid methods
     - two typical approaches:
       - 1) coarse-grained model
         - less detail on interations b/w genes
         - typically rely on **discrete variables**
         - ex) Boolean networks, Bayesian networks, Petri Nets, rule sets, etc.
       - 2) fine-grained model
         - large network, complicated interactions b/w genes, an enormous number of parameters. 
         - typically based on **continuous variables**
         - ex) S-Systems(Systems of Differential Equations), ANN, thermodynamic models, Hybrid Petri Nets, or analysing only subnetworks of the entire GRN, etc.
       - Both inference and analysis of them are difficult, thus global(high-level) analysis of the network has its attractions.
         - Combining levels of detail in a top-down or bottom-up approach..moving from the `coarse` to the `fine` or vice versa...

 - __GRN fitting Method and inference__ 
   - Why EA ? Genetic Algorithm as an optimization method?
     - these are known to cope well with a large solution space!
     - it can be applied to both synthetic and real "gene expression" data from DNA microarrays.
     - when only limited data are available, it leads to **under-specfication of the system**`(i.e. the limited number of data points combined with the large number of parameters)`**. Under these circumstances, **EA**s become a good alternative to other fitting methods. as they provide an efficient way of spanning the promising areas of the solution space!
   - Checkpoint(A): Scalability?
     - how it works based on...all the genes or subset of them in the network????
     - quantitative behaviour:
       - ability to reproduce data (indentifying the most important interactions ?)
       - parameter quality by size?
   
   - Checkpoint(B): Robustness to noise? 
     - With the presence of noise, show best balance for sensitivity-specificity ?
     - With the presence of noise, show best qualitative behaviour ?
  
  





















































