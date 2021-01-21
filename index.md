---
title       : "Phylogenetics of dispersal"
subtitle    : "BIOL33221: Bioinformatics"
author      : Dr Axel Barlow
job         : "email: axel.barlow@ntu.ac.uk, office: IBRC115"
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : zenburn      # {zenburn, tomorrow, solarized-dark, ...}
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
logo        : ntu-shield.png
biglogo     : NTU_open-graph.png
assets      : {assets: ../../assets}
license     : by-nc-sa
github:
  user: draxelbarlow
  repo: BIOL33221_phylo_dispersal
  branch: "gh-pages"
---



<!-- adding bold and italic options -->
<style>
em {
  font-style: italic
}
strong {
  font-weight: bold;
}
</style>

## Phylogenetics of dispersal

- Population trees
- The process of dispersal
- Examples
- Viral pandemics

--- .class #id

## Essential reading

<embed src="./assets/img/Baldauf - 2003 - Phylogeny for the faint of heart A tutorial.pdf" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" width="100%" style="display: block; margin: auto;" type="application/pdf" />

--- .segue .dark 

## We can calculate phylogenies of different things...

--- .class bg:white

## Species trees

- These are phylogenies of species
- Each tip is a different, reproductively isolated species
- Can be inferred from a variety of data types

<img src="assets/fig/unnamed-chunk-2-1.png" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" width="40%" style="display: block; margin: auto;" />

--- .class bg:white

## Gene trees

- These are phylogenies of individual loci (e.g. a gene)
- Or related sets of loci (e.g. multigene families)
- Each tip is a different allele (i.e. a gene variant)

<img src="assets/fig/unnamed-chunk-3-1.png" title="plot of chunk unnamed-chunk-3" alt="plot of chunk unnamed-chunk-3" width="60%" style="display: block; margin: auto;" />

--- .class bg:white

## Population-level trees

- Each tip is an individual
- Each node is their most recent ancestor (coalescence event)
- Shows the relationships of individuals and populations

<img src="assets/fig/unnamed-chunk-4-1.png" title="plot of chunk unnamed-chunk-4" alt="plot of chunk unnamed-chunk-4" width="60%" style="display: block; margin: auto;" />

--- .segue .dark 

## How does that work?

--- .class bg:white

<img src="./assets/img/mtDNA_tree.svg" title="plot of chunk unnamed-chunk-5" alt="plot of chunk unnamed-chunk-5" width="95%" style="display: block; margin: auto;" />

--- .class bg:white

## Calculating population-level trees

### We'll think about mitochondrial haplotypes (diploid loci 2x more complex)

- Sequence variation provides phylogenetic information
- Similar sequences are more closely related
- Branch lengths are (loosely) proportional to sequence divergence
- Coalescence times also depend on population size
- Described by **coalescent theory**

<img src="assets/fig/unnamed-chunk-6-1.png" title="plot of chunk unnamed-chunk-6" alt="plot of chunk unnamed-chunk-6" width="50%" style="display: block; margin: auto;" />

--- .class bg:white

## Human mitochondrial phylogeny

*Rishishwar L, Jordan IK. BMC Genomics. 2017;18:140. CC BY 4.0*

<img src="./assets/img/Dendrogram_showing_relationships_among_mtDNA_haplotypes_and_the_major_mtDNA_haplogroups.png" title="plot of chunk unnamed-chunk-7" alt="plot of chunk unnamed-chunk-7" width="65%" style="display: block; margin: auto;" />

--- .class #id

## PhyloTree.org visualisation

<iframe src = 'https://www.phylotree.org/tree/index.htm' height='600px'></iframe>

--- .class bg:white

## Geographic occurrence

<img src="./assets/img/haplo_map.png" title="plot of chunk unnamed-chunk-8" alt="plot of chunk unnamed-chunk-8" width="95%" style="display: block; margin: auto;" />

*Rishishwar L, Jordan IK. BMC Genomics. 2017;18:140. CC BY 4.0*

--- .class bg:white

<img src="./assets/img/WorldMigrations2012.png" title="plot of chunk unnamed-chunk-9" alt="plot of chunk unnamed-chunk-9" width="95%" style="display: block; margin: auto;" />

--- .class #id

## PIECE TO CAMERA

--- &twocol bg:white

## The dispersal process

- Imagine 2 Islands: A and B
- B is colonised from A by a single individual
- This transports one lineage from A to the new island B
- Individuals from B are nested within the A clade

*** =left

<img src="assets/fig/unnamed-chunk-10-1.png" title="plot of chunk unnamed-chunk-10" alt="plot of chunk unnamed-chunk-10" width="90%" style="display: block; margin: auto;" />

*** =right

<img src="./assets/img/island_dispersal.png" title="plot of chunk unnamed-chunk-11" alt="plot of chunk unnamed-chunk-11" width="40%" style="display: block; margin: auto;" />

--- &twocol bg:white

## Subsequent expansion

- The newly introduced B population expands
- All individuals are descendants of the founding lineage
- The B clade is nested within A
- A individuals are **paraphyletic** with respect to B

*** =left

<img src="assets/fig/unnamed-chunk-12-1.png" title="plot of chunk unnamed-chunk-12" alt="plot of chunk unnamed-chunk-12" width="90%" style="display: block; margin: auto;" />

*** =right

<img src="./assets/img/island_dispersal2.png" title="plot of chunk unnamed-chunk-13" alt="plot of chunk unnamed-chunk-13" width="40%" style="display: block; margin: auto;" />

--- &twocol

## Examples: Golden Lancehead

*** =left

<img src="./assets/img/Ilha_da_Queimada_Grande_-_Itanhaém3.jpg" title="plot of chunk unnamed-chunk-14" alt="plot of chunk unnamed-chunk-14" width="70%" style="display: block; margin: auto 0 auto auto;" />
*Queimada Grande, Prefeitura Municipal de ItanhaÃ©m, CC BY 2.5*

*** =right

<img src="./assets/img/Bothrops_insularis.jpg" title="plot of chunk unnamed-chunk-15" alt="plot of chunk unnamed-chunk-15" width="70%" style="display: block; margin: auto auto auto 0;" />
*Bothrops insularis, Nayeryouakim, CC BY 4.0*

<img src="./assets/img/Jararaca.jpg" title="plot of chunk unnamed-chunk-16" alt="plot of chunk unnamed-chunk-16" width="70%" style="display: block; margin: auto auto auto 0;" />
*Bothrops jararaca, Fernando Tatagiba, CC BY 3.0*

--- &twocol bg:white

## Examples: Golden Lancehead

*** =left

<img src="assets/fig/unnamed-chunk-17-1.png" title="plot of chunk unnamed-chunk-17" alt="plot of chunk unnamed-chunk-17" width="90%" style="display: block; margin: auto;" />

*Wüster et al. Journal of Zoology 266.1 (2005): 1-10*

*** =right

<img src="./assets/img/Bothrops_insularis.jpg" title="plot of chunk unnamed-chunk-18" alt="plot of chunk unnamed-chunk-18" width="70%" style="display: block; margin: auto auto auto 0;" />
*Bothrops insularis, Nayeryouakim, CC BY 4.0*

<img src="./assets/img/Jararaca.jpg" title="plot of chunk unnamed-chunk-19" alt="plot of chunk unnamed-chunk-19" width="70%" style="display: block; margin: auto auto auto 0;" />
*Bothrops jararaca, Fernando Tatagiba, CC BY 3.0*

--- &twocol

## Examples: Barbados anoles

*** =right

<img src="./assets/img/LA_map.png" title="plot of chunk unnamed-chunk-20" alt="plot of chunk unnamed-chunk-20" width="70%" style="display: block; margin: auto;" />

*** =left

<img src="./assets/img/Martinique's_anole.png" title="plot of chunk unnamed-chunk-21" alt="plot of chunk unnamed-chunk-21" width="75%" style="display: block; margin: auto;" />
*Anolis roquet, Adamhesim, CC BY 4.0*

<img src="./assets/img/Anolis_extremus-m04.jpg" title="plot of chunk unnamed-chunk-22" alt="plot of chunk unnamed-chunk-22" width="40%" style="display: block; margin: auto;" />
*Anolis extremus, Postdlf, CC BY SA-3.0*

--- &twocol bg:white

## Examples: Barbados anoles

*** =right

<img src="./assets/img/LA_map.png" title="plot of chunk unnamed-chunk-23" alt="plot of chunk unnamed-chunk-23" width="70%" style="display: block; margin: auto;" />

*** =left

<img src="./assets/img/roq_ext_MCC.tre.svg" title="plot of chunk unnamed-chunk-24" alt="plot of chunk unnamed-chunk-24" width="45%" style="display: block; margin: auto;" />

*Thorpe et al. Mol phylogenet evol 127 (2018): 682-695.*

--- &twocol bg:white

## Complicating factors

- So far we have considered a **small** and **genetically similar** founding population
- What happens if the founding population is large and genetically diverse?

>- This can "look" like multiple colonisation events
>- And even make the direction of colonisation uncertain

*** =left

<img src="assets/fig/unnamed-chunk-25-1.png" title="plot of chunk unnamed-chunk-25" alt="plot of chunk unnamed-chunk-25" width="90%" style="display: block; margin: auto;" />

*** =right

<img src="./assets/img/island_dispersal3.png" title="plot of chunk unnamed-chunk-26" alt="plot of chunk unnamed-chunk-26" width="40%" style="display: block; margin: auto;" />

--- .segue .dark 

## So what about viruses?

--- &twocol bg:white

## Racoon rabies in Ontario

*Nadin-Davis et al. Virus Research 232 (2017): 123-133. CC BY 4.0*

*** =left

<img src="./assets/img/racoon_rabies_tree.jpg" title="plot of chunk unnamed-chunk-27" alt="plot of chunk unnamed-chunk-27" width="100%" style="display: block; margin: auto;" />

*** =right

<img src="./assets/img/racoon_rabies_map.jpg" title="plot of chunk unnamed-chunk-28" alt="plot of chunk unnamed-chunk-28" width="100%" style="display: block; margin: auto;" />

--- .class bg:white

## Avian influenza H5N1 in Asia

*Tian et al. Proceedings of the National Academy of Sciences 112.1 (2015): 172-177.*

<img src="./assets/img/avian_influenza.jpg" title="plot of chunk unnamed-chunk-29" alt="plot of chunk unnamed-chunk-29" width="65%" style="display: block; margin: auto;" />

--- .class bg:white

## Ebola virus in West Africa

*Suchard, et al. Virus evolution 4.1 (2018): vey016.*

<img src="./assets/img/ebola.png" title="plot of chunk unnamed-chunk-30" alt="plot of chunk unnamed-chunk-30" width="85%" style="display: block; margin: auto;" />

--- .class #id

## Phylogenetics of dispersal

- Population trees
- The process of dispersal
- Examples
- Viral pandemics

--- &thankyou

## Next time

**Bayesian phylogenetics**

