### Placement of the ρ-WGD Event

This module contains the pipelines used to determine the phylogenetic placement of the whole-genome duplication (WGD) events across grass lineages. 

To test whether the WGD event observed in *S. spicata* is shared with *S. angustifolia*, *P. latifolius*, and core grass species, we employed the **PUG** software. The workflow involves the identification of duplicate gene pair sets (`grass.paralog.txt`) and the estimation of multiple gene trees alongside a reference species tree, following the phylogenomic strategy described by McKain et al. (2016). This approach allowed us to accurately map the ρ-WGD event onto the grass phylogeny.

**Key Resource:**
* **PUG**: [https://github.com/mrmckain/PUG](https://github.com/mrmckain/PUG)
**Command:**
  ```bash
  while read x;do echo $x;mkdir $x;grep $x grass.paralog.txt >$x/$x.paralog.txt;cd $x;perl ${PUG_PATH}/PUG.pl --trees  ../spi_gene_trees --outgroups mac,aco --species ../grass.tre --tree_type Bayesian --name $x --paralogs $x.paralog.txt;cd ..;done <sp.list
  ```
