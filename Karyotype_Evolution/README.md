# Karyotype Evolution Protocol

This module contains the source data and analytical scripts used to reconstruct the ancestral grass karyotype (AGK) and trace chromosomal rearrangements across major grass lineages.

* **`Species/`**: Contains the input genomic data (e.g., coding sequences, annotations) for the diverse grass species and outgroup taxa used in our comparative analyses.
* 
| Abbreviation | Scientific Name | Subfamily |
| :--- | :--- | :--- |
| **stSp** | *Streptochaeta spicata* | Anomochlooideae |
| **olLa** | *Olyra latifolia* | Bambusoideae |
| **raGu** | *Raddia guianensis* | Bambusoideae |
| **erCu** | *Eragrostis curvula* | Chloridoideae |
| **orTh** | *Oropetium thomaeum* | Chloridoideae |
| **lePe** | *Leersia perrieri* | Oryzoideae |
| **orSa** | *Oryza sativa* | Oryzoideae |
| **alse** | *Alloteropsis semialata* | Panicoideae |
| **coLa** | *Coix lacryma-jobi* | Panicoideae |
| **ecHa** | *Echinochloa haploclada* | Panicoideae |
| **erOp** | *Eremochloa ophiuroides* | Panicoideae |
| **paHa** | *Panicum hallii* | Panicoideae |
| **saSp** | *Saccharum spontaneum* | Panicoideae |
| **seVi** | *Setaria viridis* | Panicoideae |
| **soBi** | *Sorghum bicolor* | Panicoideae |
| **phLa** | *Pharus latifolius* | Pharoideae |
| **aeBi** | *Aegilops bicornis* | Pooideae |
| **aeSh** | *Aegilops sharonensis* | Pooideae |
| **avAt** | *Avena atlantica* | Pooideae |
| **brDi** | *Brachypodium distachyon* | Pooideae |
| **brSt** | *Brachypodium stacei* | Pooideae |
| **hoMa** | *Hordeum marinum* | Pooideae |
| **loPe** | *Lolium perenne* | Pooideae |
| **puTe** | *Puccinellia tenuiflora* | Pooideae |
| **seCe** | *Secale cereale* | Pooideae |
| **thEl** | *Thinopyrum elongatum* | Pooideae |

* **`Ancestral_Grass_Karyotype/`**: Houses the reconstructed ancestral grass karyotypes. To facilitate replication and further research, we provide the ancestral gene order and sequence formatted for both `jcvi` and `wgdi` input requirements.
* **`Karyotype_Mapping/`**: Contains the vector-format karyotype diagrams presented in Figure 4. These figures visualize the macro-syntenic mapping results, illustrating the synteny blocks, breakpoints, and collinearity data that demonstrate the relationship between the post-ρ AGK and extant grass species.
