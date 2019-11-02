# Gene-Regulatory-Network

> Background?
 - __Reverse engineering of GRNs?__ 
   - In each type of cell, different genes are expressed (turned on) or silenced (turned off). By identifying which genes in the sick cells are working abnormally, doctors can better diagnose the ailment. One way they do this is to use a **DNA microarray** to determine the expression levels of genes. When a gene is expressed in a cell, it generates `messenger RNA` (mRNA). `**Overexpressed genes** generate more mRNA. This can be detected on the **microarray**`.
   - **Technologies** measuring **gene expression levels**(gene turned on) has created a database for inferring GRNs. However, the nature of these data has made this GRN inferring process very difficult and the large scale quantitative analysis on real biological datasets cannot be performed, to date, as existing approaches are not suitable for **real microarray data** which are noisy and insufficient.

 - __GRN__
   - The level of mRNA concentrations can be viewed as a snapshot of the genes expression levels under certain conditions. With a large enough set of snapshots, it should be theoretically possible to uncover the underlying gene regulatory network(GRN). 
   - **Modeling:** We can find parameters of the GRN model from available data. Once built, these GRN models can be used to predict the behaviour of the organism **under certain conditions**, related to different treatments or diseases(predict its behaviour under different conditions).
     - `genes` are viewed as **variables** that change their (expression) values in time.
       - Depending on the type of variables used, methods can be classiﬁed as discrete or continuous, deterministic or stochastic, or as hybrid methods
     - two typical approaches:
       - 1) coarse-grained model
         - less detail on interations b/w genes
         - typically rely on **discrete variables**
       - 2) fine-grained model
         - large network, complicated interactions b/w genes, an enormous number of parameters. 
         - typically based on **continuous variables**
       - Both inference and analysis of them are difficult, thus global(high-level) analysis of the network has its attractions.
         - For coarse-grained models: Boolean networks, Bayesian networks, Petri Nets, rule sets, etc.
         - For fine-grained models: Systems of Differential Equations, ANN, thermodynamic models, Hybrid Petri Nets, or analysing only subnetworks of the entire GRN, etc.
         - Combining levels of detail in a top-down or bottom-up approach..moving from the coarse to the fine or vice versa...




 - __Quantitative GRN modelling and inference__ 
   - Use EA ? Genetic Algorithm?
     -  it can be applied to both synthetic and real "gene expression" data from DNA microarrays. 
   - Can reproduce biological behaviour?
   - Scalability?
   - Robustness to noise? 
  





















































