### Phylogeny and Divergence Time Estimation

This folder contains the data, scripts, and configuration files utilized to reconstruct the species tree and estimate evolutionary divergence times across major grass lineages. 

#### 1. Species Tree Reconstruction
We reconstructed a maximum likelihood (ML) phylogeny using a concatenated alignment of 295 single-copy orthologous genes (`merge.final.fa`). The inference was performed using RAxML-NG under the GTR+G substitution model, evaluating node support with 1,000 bootstrap replicates.

**Command:**
```bash
raxml-ng --all --msa merge.final.fa --model GTR+G --prefix T4 --bs-metric fbp,tbe --tree pars{20},rand{20} --bs-trees 1000 --outgroup mac
```
#### 2. Divergence Time Estimation
To provide a temporal framework for the origin of grasses and the ρ-WGD event, divergence times were estimated using MCMCtree from the PAML package. This analysis applied a relaxed molecular clock calibrated with two fossil records: 
the Poaceae crown node (>65 Ma) and the Pooideae crown node (>47.8 Ma), with the root age constrained to a maximum of 150 Ma.

**Command:**
```bash
mcmctree mcmctree.ctl
```
