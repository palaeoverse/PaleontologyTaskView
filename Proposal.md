**Submission: Open an issue in the ctv repository with the title CRAN task view proposal: MyTopic where MyTopic should be replaced with the intended name of the task view in CamelCase.**



**Scope: Include one or two paragraphs about the scope of the task view, outlining the inclusion and exclusion criteria as well as relevant sections within the topic.**

Phylogenetic methods are for inferring evolutionary relationships (family trees) of organisms. A recent innovation is phylogenetic networks: relaxing the tree metaphor so that a single node may have more than one parent (due to hybridization or other factors). These trees are used for many questions in the fields of ecology and evolution (more rarely in other fields, like linguistics), such as looking at how speciation has changed through time or across different groups of organisms, understanding how characters have changed through time, and more. There was long a task view on this area; it was removed after the maintainer was nonresponsive during the move from R-forge to GitHub, but a new primary maintainer has been added.

The task view will include packages that do all the above. It will not include packages that are not used in the evolution and/or ecology domains (i.e., other packages that use decision trees, network diagrams in general, and so forth). It will include packages on CRAN but also ones available in other repositories like github: many of the key packages in the field rise to prominence before getting on CRAN or, once on, may sometimes rotate off (a risk for research software, especially given that many of the authors are biologists who may spend months in the field). 

**Packages: Include a tentative list of packages for the task view. This should encompass the "core" packages and a collection of relevant packages, ideally grouped by sections within the topic. It is not important, yet, that the list of sections or packages is already exhaustive.**

Please see https://github.com/bomeara/PhylogeneticsTaskView/blob/main/Phylogenetics.md for a list of packages and sections.

**Overlap: Comment on potential overlap with already existing task views as well as with task views that might be created (or split off) in the future.**

There was for some time a genetics task view that was a potential overlap, but which focused more on within species rather than between species processes. There is potential overlap with Environometrics and WebTechnologies as interfaces to the sorts of data used in phylogenetic analyses, but in practice the number of potentially overlapping packages is low.

**Maintainers: The proposal should be made by the person willing to act as the principal maintainer for the task view. Furthermore, task views should have teams of additional 1-5 co-maintainers and possible candidates for these can be listed as well in the proposal.**

Will Gearty will be primary maintainer.
