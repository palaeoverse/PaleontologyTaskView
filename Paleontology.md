---
name: Paleontology
topic: Paleontology
maintainer: William Gearty, Lewis A. Jones, Erin Dillon, Pedro Godoy, Harriet Drage, Christopher Dean, Bruna Farina
email: willgearty@gmail.com
version: 2024-10-04
source: https://github.com/cran-task-views/Paleontology/
---

## Overview

Computational paleontology is a thriving field. Gone are the days of just digging up fossils; paleontologists now have the luxury of being able to perform a wide array of complex computational analyses on local and global compendia of fossil data to study the evolution of organisms and the environments they live in. Until recently, computational paleontologists have mostly relied on resources designed for evolutionary biologists, ecologists, GISers, and data scientists to accomplish such analyses. However, slowly but surely, R resources are being developed to cater to these paleontological tasks.

Therefore, we have assembled this task view to bring together all R packages that are specifically geared towards acquiring, cleaning, visualizing, and/or analyzing various kinds of paleontological and paleontology-adjacent data. We use this venue to showcase the wide variety of R packages available across the paleosciences and to provide a brief contextual overview of each package for a broad audience of R users.

If you have any questions, feel free to reach out to the task view maintainers or the maintainers of specific packages. Questions may also be directed to the [palaeoverse google group](https://groups.google.com/g/palaeoverse) or the [paleonet](https://paleonet.org/) mailing list.

## Scope

Packages within the task view fall within one or more of the following broad categories:

1.  **[Wrangling paleontological data](#wrangling-paleontological-data):** packages dedicated to the acquisition, cleaning, manipulation, and/or visualization of paleontological data
2.  **[Paleoecology and morphological evolution](#paleoecology-and-morphological-evolution):** packages that are useful for performing paleoecological and morphological analyses
3.  **[Paleobiogeography and biodiversity](#paleobiogeography-and-biodiversity):** packages that are useful for performing paleobiogeographical and/or paleobiodiversity analyses
4.  **[Phylogenetics](#phylogenetics):** packages that are useful for performing phylogenetic analyses that include paleontological data
5.  **[Time series analysis](#time-series-analysis):** packages that are useful for performing time series analyses of paleontological data
6.  **[Stratigraphy and sedimentology](#stratigraphy-and-sedimentology):** packages that are useful for acquiring and analyzing stratigraphic or sedimentological data
7.  **[Paleoclimate](#paleoclimate):** packages that are useful for acquiring and analyzing paleoclimate data

## Wrangling paleontological data

### Acquiring paleontological data

- `r pkg("paleobioDB")` has functions to query, download, process, and visualize occurence and taxonomic data from the [Paleobiology Database](https://paleobiodb.org/#/) (PBDB).
- `r pkg("rgbif")` can query and download biological and paleontological occurrence data from the [Global Biodiversity Information Facility](https://www.gbif.org) (GBIF).
- `r pkg("ridigbio")` can query and download biological and paleontological specimen record data from [iDigBio](https://www.idigbio.org/).
- `r pkg("neotoma2")` can query, download, and manipulate data from the [Neotoma Paleoecology Database](https://www.neotomadb.org/), which specializes in fossil data holdings at timescales covering the last several decades to the last several million years.
- `r pkg("sepkoski")` contains data on the stratigraphic ranges of fossil marine animal genera from Sepkoski's (2002) published compendium.
- `r pkg("folio")` contains datasets for teaching quantitative approaches and modeling in archaeology and paleontology.
- `r pkg("chronosphere")` can download time-stamped versions of various paleontological, paleoenvironmental, and paleoecological [databases](https://chronosphere.info/data/), including BioDeepTime (Smith et al. 2023), Triton (Fenton et al. 2021), the [Paleobiology Database](https://paleobiodb.org/#/), and the [Ancient Reef Traits Database](https://art.nat.fau.de/).

### Cleaning and/or manipulating paleontological data

- `r pkg("palaeoverse")` has functionality to support data preparation and exploration for paleobiological analyses with a focus on improving code flow, reproducibility, and accessibility.
- `r pkg("CoordinateCleaner")` can perform automated flagging of common spatial and temporal errors in biological and paleontological collection data.
- `r pkg("fossilbrush")` can perform automated detection and resolution of taxonomic and stratigraphic errors in fossil occurrence datasets.
- `r pkg("rgplates")` can query the [GPlates](https://www.gplates.org/) desktop application and [web service API](https://gws.gplates.org/) to reconstruct past positions of geographic entities (e.g., plates, coastlines, and coordinates) based on user-selected rotation models. The `palaeorotate` function in `r pkg("palaeoverse")` can be used to query the GPlates API for fossil occurrences across multiple time intervals.

### Visualizing paleontological data

- `r pkg("deeptime")` extends the functionality of the [`ggplot2`](https://ggplot2.tidyverse.org/) package to help facilitate the plotting of data over long time intervals. Several functions are available to add highly customizable timescales to a variety of types of visualizations.
- `r pkg("palaeoverse")` has functions for visualizing occurrence data through time and across space in base R. The `axis_geo` function can be used to add a timescale to a base R plot.
- `r pkg("GEOmap")` includes a set of routines for making map projections, topographic maps, perspective plots, and geological maps.
- `r pkg("rphylopic")` can query and fetch silhouettes of biological and paleontological organisms from the [PhyloPic](https://www.phylopic.org/) database.

## Paleoecology and morphological evolution

### Paleoenvironmental reconstruction

- `r pkg("rioja")` implements a number of numerical methods for inferring the value of an environmental variable from a set of species abundances.
- `r pkg("analogue")` has functions for the prediction of environmental data from species data by fitting Modern Analogue Technique and Weighted Averaging transfer function models.

Users may also find packages in the `r view("Environmetrics")` task view useful for analyzing ecological and environmental data.

### Quantifying ecological and morphological evolution

- `r pkg("ecospace")` implements Monte Carlo simulations of ecological diversification models, using a user-specified ecospace (trait space) framework.
- `r pkg("fossil")` has functions for estimating shared species/beta diversity, species area curves, and geographic distances and areas.
- `r github("HOPE-UIB-BIO/R-Fossilpol-package")` has functions for processing and standardizing global palaeoecological pollen data.
- `r pkg("Morphoscape")` implements adaptive landscape methods (first described by Polly et al. 2016) for the integration, analysis and visualization of biological trait data on a phenotypic morphospace.
- `r pkg("RRphylo")` can be used to estimate variation and shift in the rate of phenotypic evolution with fossil data using phylogenetic ridge regression.
- `r pkg("paleoTS")`, `r pkg("evoTS")`, and `r github("klvoje/adePEM")` have functions for fitting evolutionary models to morphological time series (see [Time series analysis](#time-series-analysis) for more information).

Also see the `r view("Phylogenetics")` task view for details about studying discrete and continuous morphological evolution in a phylogenetic context.

## Paleobiogeography and biodiversity

- `r github("josteist/Compadre")` can be used to estimate rates of speciation/origination, extinction, and sampling using Bayesian capture-mark-recapture techniques.
- `r pkg("divDyn")` has functions to describe the sampling and diversity dynamics of fossil occurrence datasets.
- `r pkg("fossil")` has functions for estimating species richness (Chao 1 and 2, ACE, ICE, Jacknife) and shared species/beta diversity.
- `r pkg("divvy")` has functions to conduct spatial subsampling for biogeography and biodiversity studies and calculate common biodiversity and range-size metrics.
- `r github("Liudas-Dau/hespdiv")` has functions to conduct hierarchical spatial sampling and perform analysis and visualization of these samples.
- `r pkg("ppgm")` can be used to conduct paleophylogeographic modeling of climate niches and species distributions.

Users may also find packages in the `r view("Spatial")` task view useful for analyzing paleobiogeography.

## Phylogenetics

- `r pkg("paleotree")` provides tools for transforming, a posteriori time-scaling, and modifying phylogenies containing extinct lineages.
- `r pkg("FossilSim")` can be used to simulate fossil occurrence data on phylogenetic trees under mechanistic models of speciation, fossil preservation, and fossil recovery. Quick simulations can be conducted in a graphical user interface with `r pkg("FossilSimShiny")`.
- `r pkg("paleobuddy")` can be used to simulate phylogenetic trees and fossil records with custom speciation, extinction, and fossil sampling rates.
- `r github("rachelwarnock/fbdR")` has functions for estimating speciation and extinction rates from phylogenetic trees and fossil occurrence data.
- `r github("evolucionario/cladedate")` has functions to use a MonteCarlo approach to generate empirical calibration information from the fossil record.
- `r pkg("RRphylo")` can be used to estimate variation and shift in the rate of phenotypic evolution with fossil data using phylogenetic ridge regression.
- `r pkg("strap")` has functions for the stratigraphic analysis of phylogenetic trees.

Also see the `r view("Phylogenetics")` task view for broader details about conducting various analyses in a phylogenetic context.

## Time series analysis

- `r pkg("paleoTS")` facilitates the analysis of paleontological temporal sequences of trait values by fitting evolutionary models using maximum likelihood.
- `r pkg("evoTS")` facilitates univariate and multivariate analysis of evolutionary sequences of phenotypic change over time. The package extends the modeling framework available in `r pkg("paleoTS")`.
- `r github("klvoje/adePEM")` has functions for assessing the adequacy of models of phenotypic change within lineages, like those fit by `r pkg("paleoTS")` and `r pkg("evoTS")`.
- `r pkg("StratPal")` can be used to simulate biological processes in the time domain (e.g., trait evolution, fossil abundance), and examine how their expression in the rock record (stratigraphic domain) is influenced based on age-depth models, ecological niche models, and taphonomic effects.
- `r pkg("astrocron")` can conduct routines for astrochronologic testing, astronomical time scale construction, and time series analysis. Also included are a range of statistical analysis and modeling routines that are relevant to time scale development and paleoclimate analysis.
- `r github("HOPE-UIB-BIO/R-Ratepol-package")` has functions for estimating rate of change (RoC) from community data in time series.

Also see the `r view("TimeSeries")` task view for broader details about conducting time series analyses.

## Stratigraphy and sedimentology

### Acquiring stratigraphic and sedimentological data

- `r pkg("rmacrostrat")` can fetch geological data from [Macrostrat](https://macrostrat.org/) relevant to the spatial and temporal distribution of sedimentary, igneous, and metamorphic rocks as well as data extracted from them.

### Analyzing stratigraphic and sedimentological data

- `r pkg("admtools")` can be used to estimate age-depth models from stratigraphic and sedimentological data.
- `r pkg("Bchron")` has functions for quick calibration of radiocarbon dates under various calibration curves.
- `r pkg("clam")` can be used to perform 'classical' age-depth modelling of dated sediment deposits.
- `r github("nickmckay/GeoChronR")` has functions to generate state-of-the-art age models, create time-uncertain ensembles, analyze those ensembles with a number of commonly-used techniques, and visualize the results in an intuitive way.
- `r pkg("rbacon")` can be used to perform age-depth modelling using Bayesian statistics to reconstruct accumulation histories for deposits, through combining radiocarbon and other dates with prior information on accumulation rates and their variability.
- `r pkg("isogeochem")` can be used to quickly calculate isotope fractionation factors and apply paleothermometry equations.
- `r pkg("DAIME")` can be used to model the effects of changing deposition rates on geological data and rates.

### Visualizing stratigraphic and sedimentological data

- `r pkg("StratigrapheR")` can be used to generate highly customizable lithologs for stratigraphic and sedimentological data from outcrop sections and borehole logs with R base graphics. `r pkg("SDAR")` can be used to make similar, albeit less customizable, graphic logs with grid graphics.
- `r pkg("tidypaleo")` provides a set of functions with a common framework for age-depth model management, stratigraphic visualization, and common statistical transformations.

## Paleoclimate

### Acquiring and manipulating paleoclimate reconstruction data

- `r pkg("rpaleoclim")` can fetch paleoclimate data from [PaleoClim](http://www.paleoclim.org/), high resolution paleoclimate surfaces covering the whole globe. This includes data on surface temperature, precipitation and the standard bioclimatic variables commonly used in ecological modelling, derived from the HadCM3 general circulation model and downscaled to a spatial resolution of up to 2.5 minutes.
- `r pkg("pastclim")` has methods to easily access, manipulate, and use paleoclimate reconstructions.

### Reconstructing and modelling paleoclimate

- `r github("mchevalier2/crestr")` can be used to create probabilistic reconstructions of past climate change from fossil assemblage data.
- `r github("rsh249/cRacle")` can be used to perform the Climate Reconstruction Analysis using Coexistence Likelihood Estimation (CRACLE) method to estimate climate and paleoclimate from vegetation using large repositories of biodiversity data.
- `r pkg("sedproxy")` can be used to conduct forward modelling of sediment archived climate proxy records based on hypothesized "true" past climate (e.g., climate model output), sedimentation, and sampling.

## References

- Fenton, I.S., Woodhouse, A., Aze, T., Lazarus, D., Renaudie, J., Dunhill, A.M., Young, J.R. and Saupe, E.E., 2021. Triton, a new species-level database of Cenozoic planktonic foraminiferal occurrences. Scientific Data, 8(1), 160. `r doi("10.1038/s41597-021-00942-7")`.
- Polly, P. D., Stayton, C. T., Dumont, E. R., Pierce, S. E., Rayfield, E. J., & Angielczyk, K. D. 2016. Combining geometric morphometrics and finite element analysis with evolutionary modeling: towards a synthesis. Journal of Vertebrate Paleontology, 36(4). `r doi("10.1080/02724634.2016.1111225")`
- Sepkoski, J. J. 2002. A compendium of fossil marine animal genera. Bulletins of American Paleontology, 363, 1–560. <https://www.biodiversitylibrary.org/item/40634>
- Smith, J., Rillo, M.C., Kocsis, Á.T., Dornelas, M., Fastovich, D., Huang, H.H.M., Jonkers, L., Kiessling, W., Li, Q., Liow, L.H. and Margulis-Ohnuma, M., 2023. BioDeepTime: A database of biodiversity time series for modern and fossil assemblages. Global Ecology and Biogeography, 32(10), 1680-1689. `r doi("10.1111/geb.13735")`
