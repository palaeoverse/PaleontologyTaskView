---
name: Paleontology
topic: Paleontology
maintainer: William Gearty, Lewis A. Jones, Erin Dillon, Pedro Godoy, Harriet Drage, Christopher Dean, Bruna Farina
email: willgearty@gmail.com
version: 2024-09-23
source: https://github.com/cran-task-views/Paleontology/
---

## Overview

Computational paleontology (or paleobiology) is a thriving field. Gone are the days of just digging up fossils; paleontologists now have the luxury of being able to perform a wide array of complex computational analyses on local and global compendia of fossil occurrence, phylogenetic, and morphological data to study the functional and phylogenetic evolution of organisms, ecosystem function and ecological interactions, paleobiogeographic patterns, and more. Until recently, computational paleontologists have mostly relied on resources designed for evolutionary biologists, ecologists, GISers, and data scientists to accomplish such analyses. However, slowly but surely, resources (including explicit R packages) are being developed to cater to these paleontological tasks.

Therefore, we have assembled this task view to bring together all R packages that are specifically geared towards acquiring, cleaning, visualizing, and/or analyzing various kinds of paleontological and paleontology-adjacent data. We use this venue to showcase the wide variety of R packages available across the paleosciences and to provide a brief contextual overview of each package for a broad audience of R users.

If you have any questions, feel free to reach out to the task view maintainers or the maintainers of specific packages. Questions may also be directed to the [paleonet](https://paleonet.org/) mailing-list after subscription.

## Scope

Packages within the task view fall within one or more of the following task categories:

1.  **Working with paleontological data in R:** packages dedicated to the acquisition, cleaning, manipulation, and/or visualization of paleontological data
2.  **Paleoecology and morphological evolution:** packages that are useful for performing paleoecological and morphological analyses
3.  **Paleobiogeography and biodiversity:** packages that are useful for performing paleobiogeographical and/or paleobiodiversity analyses
4.  **Phylogenetics:** packages that are useful for performing phylogenetic analyses that include paleontological data
5.  **Time series analysis:** packages that are useful for performing time series analyses of paleontological data
6.  **Paleoclimate and Earth system variables:** packages that are useful for acquiring and analyzing paleoclimate and Earth system data

## Working with paleontological data in R

### Getting paleontological data into R

- `r pkg("chronosphere")`
- `r pkg("folio")`
- `r pkg("neotoma2")`
- `r pkg("paleobioDB")`
- `r pkg("rgbif")`
- `r pkg("rgplates")`
- `r pkg("ridigbio")`
- `r pkg("rmacrostrat")`
- `r pkg("rpaleoclim")`

### Cleaning and/or manipulating paleontological data

- `r pkg("CoordinateCleaner")`
- `r pkg("fossilbrush")`
- `r pkg("palaeoverse")`

### Visualizing paleontological data

- `r pkg("deeptime")`
- `r pkg("GEOmap")`
- `r pkg("rphylopic")`
- `r pkg("SDAR")`
- `r pkg("StratigrapheR")`
- `r pkg("tidypaleo")`

## Paleoecology and morphological evolution

- `r pkg("analogue")`
- `r pkg("ecospace")`
- `r pkg("fossil")`
- `r github("HOPE-UIB-BIO/R-Fossilpol-package")`
- `r pkg("rioja")`
- `r pkg("morphospace")`

(and Environmetrics CTV)

## Paleobiogeography and biodiversity

- `r github("josteist/Compadre")`
- `r pkg("divDyn")`
- `r pkg("divvy")`
- `r github("Liudas-Dau/hespdiv")`
- `r pkg("ppgm")`
- `r pkg("sepkoski")`

(and Spatial CTV)

## Phylogenetics

- `r github("evolucionario/cladedate")`
- `r github("rachelwarnock/fbdR")`
- `r pkg("FossilSim")` (`r pkg("FossilSimShiny")`)
- `r pkg("paleobuddy")`
- `r pkg("paleotree")`
- `r pkg("RRphylo")`
- `r pkg("strap")`

(and Phylogenetics CTV)

## Time series analysis

- `r github("klvoje/adePEM")`
- `r pkg("astrocron")`
- `r pkg("evoTS")`
- `r pkg("paleoTS")`
- `r github("HOPE-UIB-BIO/R-Ratepol-package")`
- `r pkg("StratPal")`

(and TimeSeries CTV)

## Paleoclimate and Earth system variables

- `r pkg("Bchron")`
- `r github("rsh249/cRacle")`
- `r pkg("DAIME")`
- `r github("nickmckay/GeoChronR")`
- `r pkg("isogeochem")`
- `r pkg("pastclim")`
- `r pkg("sedproxy")`
- `r pkg("admtools")`
- `r pkg("clam")`

## References
