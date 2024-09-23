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

- `r pkg("paleobioDB")` has functions to query, download, process, and visualize occurence and taxonomic data from the [Paleobiology Database](https://paleobiodb.org/#/).
- `r pkg("rgbif")` can query and download biological and paleontological occurrence data from the [Global Biodiversity Information Facility](https://www.gbif.org) (GBIF).
- `r pkg("ridigbio")` can query and download biological and paleontological specimen record data from [iDigBio](https://www.idigbio.org/).
- `r pkg("neotoma2")` can query, download, and manipulate data from the [Neotoma Paleoecology Database](https://www.neotomadb.org/), which specializes in fossil data holdings at timescales covering the last several decades to the last several million years.
- `r pkg("folio")` contains datasets for teaching quantitative approaches and modeling in archaeology and paleontology
- `r pkg("chronosphere")` can download time-stamped versions of various paleontological, paleoenvironmental, and paleoecological [databases](https://chronosphere.info/data/), including BioDeepTime (Smith et al. 2023), Triton (Fenton et al. 2021), the [Paleobiology Database](https://paleobiodb.org/#/), and [Ancient Reef Traits Database](https://art.nat.fau.de/).

#### Acquiring paleontology-adjacent data

- `r pkg("rmacrostrat")` can fetch geological data from [Macrostrat](https://macrostrat.org/) relevant to the spatial and temporal distribution of sedimentary, igneous, and metamorphic rocks as well as data extracted from them.
- `r pkg("rpaleoclim")` can fetch paleoclimate data from [PaleoClim](http://www.paleoclim.org/), high resolution paleoclimate surfaces covering the whole globe. This includes data on surface temperature, precipitation and the standard bioclimatic variables commonly used in ecological modelling, derived from the HadCM3 general circulation model and downscaled to a spatial resolution of up to 2.5 minutes.

### Cleaning and/or manipulating paleontological data

- `r pkg("palaeoverse")` has functionality to support data preparation and exploration for palaeobiological analyses, improving code reproducibility and accessibility.
- `r pkg("CoordinateCleaner")` can perform automated flagging of common spatial and temporal errors in biological and paleontological collection data.
- `r pkg("fossilbrush")` can perform automated detection and resolution of taxonomic and stratigraphic errors in fossil occurrence datasets.
- `r pkg("rgplates")` can query the [GPlates](https://www.gplates.org/) API to reconstruct past positions of geographic entities (e.g., plates, coastlines, and coordinates) based on user-selected rotation models.

### Visualizing paleontological data

- `r pkg("deeptime")` extends the functionality of 'ggplot2' to help facilitate the plotting of data over long time intervals. Several functions are available to add highly customizable timescales to a variety of types of visualizations.
- `r pkg("GEOmap")` includes a set of routines for making map projections, topographic maps, perspective plots, and geological maps.
- `r pkg("rphylopic")` can query and fetch silhouettes of biological and paleontological organisms from [PhyloPic](https://www.phylopic.org/).
- `r pkg("StratigrapheR")` can be used to generate highly customizable lithologs for stratigraphic and sedimentological data from outcrop sections and borehole logs with R base graphics. `r pkg("SDAR")` can be used to make similar, albeit less customizable, graphic logs with grid graphics.
- `r pkg("tidypaleo")` provides a set of functions with a common framework for age-depth model management, stratigraphic visualization, and common statistical transformations

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

- Fenton, I.S., Woodhouse, A., Aze, T., Lazarus, D., Renaudie, J., Dunhill, A.M., Young, J.R. and Saupe, E.E., 2021. Triton, a new species-level database of Cenozoic planktonic foraminiferal occurrences. Scientific Data, 8(1), 160. `r doi("10.1038/s41597-021-00942-7")`.
- Smith, J., Rillo, M.C., Kocsis, Á.T., Dornelas, M., Fastovich, D., Huang, H.H.M., Jonkers, L., Kiessling, W., Li, Q., Liow, L.H. and Margulis‐Ohnuma, M., 2023. BioDeepTime: A database of biodiversity time series for modern and fossil assemblages. Global Ecology and Biogeography, 32(10), 1680-1689.
