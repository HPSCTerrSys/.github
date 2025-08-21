**Welcome to the profile page of the Centre for High-Performance Scientific Computing in Terrestrial Systems (HPSC TerrSys) organization GitHub account.**

**_HPSC TerrSys enables geosciences by high-performance computing (HPC)._**

## Introduction

<details>
<summary>Click for details</summary>
<br>

The HPSC TerrSys repositories are the official home of

- the **[encore Community Land Model (eCLM)](https://github.com/HPSCTerrSys/eCLM)**, a refactored [Community Land Model (CLM) version 5](https://www.cesm.ucar.edu/models/clm), for effiicient stand-alone-use and flexible model integration with atmospheric and hydrologic models,
- the fully coupled, physics-based **Terresterial Systems Modeling Platform ([TSMP1](https://github.com/HPSCTerrSys/TSMP) and [TSMP2](https://github.com/HPSCTerrSys/TSMP2))** regional climate/Earth system model (RCSM, RESM), linking the [ICON atmospheric model](https://www.icon-model.org) with the [eCLM land surface model](https://github.com/HPSCTerrSys/eCLM) and with the [integrated ParFlow hydrologic model](https://github.com/parflow/parflow) through the [OASIS-MCT coupler](https://gitlab.com/cerfacs/oasis3-mct),
- [PDAF-based parallel](https://github.com/PDAF/PDAF) **data assimilation versions** of TSMP1 and TSMP2 and eCLM, 

plus software tools for the pre- and postprocessing and analysis of model data, all necessary auxiliary simulation tools (built systems, workflow engines, external parameter file generators, etc.), complete simulation experiments (incl. configurations, input and reference data), as well as documentation. Unless otherwise stated, all is provided as free and open source software (FOSS), or under a CC BY license for many datasets (see individual LICENSE files).

This profile page is the top-level, overarching starting point where we

- list different types or categories of repositories, grouped in GitHub Teams, each with their own short description,
- explain the relation of the types or categories of repositories and information provided therein, as part of modularized simulations,
- thereby introduce a uniform nomenclature we use throughout the repositories, and 
- elaborate on our concept of a modularized "simulation experiment" and procedures on how to use the repositories in combination. 

</details>

## HPSC TerrSys GitHub research groups

<details>
<summary>Click for details</summary>
<br>

HPSC TerrSys software, data, information products, etc. are developed and produced by and under the auspices of the research groups of 

- **Stefan Kollet** ([Integrated Modelling of Terrestrial Systems at FZJ/IBG-3](https://www.fz-juelich.de/en/ibg/ibg-3/research-groups/modelling-terrestrial-systems/integrated-modelling-of-terrestrial-systems)),
- **Harrie-Jan Hendricks-Franssen** ([Stochastic Analysis of Terrestrial Systems at FZJ/IBG-3](https://www.fz-juelich.de/en/ibg/ibg-3/research-groups/modelling-terrestrial-systems/stochastic-analysis-of-terrestrial-systems)), and 
- **Daniel Caviedes-Voullieme** ([Simulation- and Data-Lab Terrestrial Systems at FZJ/JSC](https://www.fz-juelich.de/en/ias/jsc/about-us/structure/simulation-and-data-labs/sdl-terrestrial-systems))

at [Research Centre Juelich (Forschungszentrum Jülich, FZJ](https://www.fz-juelich.de/en)) in the [Helmholtz Association of German Research Centres (HGF)](https://www.helmholtz.de/en/). Founded in 2011, [HPSC TerrSys](https://www.hpsc-terrsys.de/en) is a virtual competence center within the [Geoverbund ABC/J](https://www.geoverbund-abcj.de/en), the geoscientific network of the Aachen-Bonn-Cologne-Jülich research region, in Germany.

<!-- ToDo: create teams of the research groups and add respective repositories according to code ownership, if this has the unanimous consent of the group leads, better: add a link behind each group above, saves space
### Research group code ownerships and development leads

Repositories in the above categories are under the auspices of either one of the following research groups at FZJ:

- S. Kollet group
- H.-J. Hendricks-Franssen group
- D. Caviedes-Voullieme group
-->

**Our research focus in a nutshell**

Very broadly, our research interests are on the functioning and (climate change induced) changes of coupled geo-ecosystems, the water and energy cycles therein, characterized by complex feedbacks and interactions, from the groundwater, through the land surface, to the atmosphere, including human interventions, such as anthropogenic water use. 

**FOSS and FAIR**

<!-- ToDo: add technical e-mail address --> 
Here we provide and share some of our core scientific computing tools for efficient joint cross-institutional development, community reuse, feedback, and potential collaboration, as well as for internal use within HPSC TerrSys.

</details>

## Repository content and categories (=GitHub Teams)

<details>
<summary>Click for details</summary>
<br>

<!-- ToDo: sort in all repositories of HPSC TerrSys, which have not yet been assigned to a category; one needs to be either GitHub organization Owner to add repos to a Github Team, or a GitHub Team Owner / Maintainer and repo Owner / Admin at the same time -->
<!-- ToDo: maybe put this as quicklinks up front to the top of the page, depends on HPSC TerrSys community feedback -->

- [Coupled model systems](https://github.com/orgs/HPSCTerrSys/teams/coupled-model-systems/repositories)
- [Individual model systems](https://github.com/orgs/HPSCTerrSys/teams/individual-model-systems/repositories)
- [Workflow engines](https://github.com/orgs/HPSCTerrSys/teams/workflow-engines/repositories)
- [(Pre-/Post-)processing and setup tools](https://github.com/orgs/HPSCTerrSys/teams/processing-and-setup/repositories)
- [Configurations](https://github.com/orgs/HPSCTerrSys/teams/configurations/repositories)
- [Static or external parameter model input files](https://github.com/orgs/HPSCTerrSys/teams/external-parameters/repositories)
- [Simulation experiments](https://github.com/orgs/HPSCTerrSys/teams/simulation-experiments/repositories)
- [(Generic) data analytics tools](https://github.com/orgs/HPSCTerrSys/teams/data-analytics/repositories)
- [(Model system) auxiliary tools](https://github.com/orgs/HPSCTerrSys/teams/auxiliary-tools/repositories)

These are the current GitHub Teams, i.e., the repository categories (according to the type of information). These GitHub Teams contain one or more repositories each. Each individual repository is assigned to a single type of information or category (i.e., Team) only. Large files, e.g., readily prepared external parameter files for ICON, are usually stored under an open LFS Git repository outside GitHub. The repositories follow a certain naming scheme, seperated by underscores: `<type of content>_<model-system_specific-identifier>`, e.g., `NML_ICON_...`, `EO_ICON_...`.

See [here for the full (unsorted) list](https://github.com/orgs/HPSCTerrSys/repositories) of HPSC TerrSys repositories.

</details>

## Overarching concepts and procedures running HPSC TerrSys simulations

<details>
<summary>Click for details</summary>
<br>

<!-- this mightbe also called the "platform" concept, but this might be misleading, then platform is used in a more abstract meaning but it si s also the name of the TSMP1/2 -->
To make best use of the software and data of the HPSC TerrSys GitHub, and to explain how we run and organize many of our simulations in HPSC TerrSys,here's a quickstart guide to 
1. our concept of a fully modularized modeling platform, 
2. what we understand as a "simulation experiment" (SimExp),
3. the procedure to get a SimExp started and maintained, 
4. SimExp examples (that also serve as quickstart, test, benchmark use cases).

### Modularized simulation platform concept

<details>
<summary>Click for details</summary>
<br>

> ❗ **Important**  
> Each repository provides an independent piece of software, data, or information and has its own documentation (e.g., as a `README.md` project overview or GitHub Pages), LICENSE and may be used standalone. It is up to the user.

- With HPSC TerrSys a highly modularized software development, maintenance, and deployment paradigm, which also affects our simulations. 
- Individual, independent Git repositories are combined (hierarchically), usually by means of Git submodules, to constitute, e.g., a coupled model system or simulation experiment. This leads to a lightweight, transparent, reproducible, maintainable, scalable, versioned, and provenance-enabled software and simulation infrastructure. <!-- [See details below](#overarching-simulation-concept-and-procedures). -->
- The TSMP RESMs (TSMP1 and TSMP2), e.g., follow this paradigm, that supports the properties and features of **TSMP as a versatile "platform" to built and expand simulation experiments** on, whether the fully coupled model system is used or only component models thereof.

</details>

<!-- publication in JOSS planned -->
### Modularized "simulation experiments" (SimExp)

<details>
<summary>Click for details</summary>
<br>

> ❗ **Basic principles, use Git to maintain and organize a simulation**  
> - With a SimExp everything is version-controlled via Git. The SimExp consists of modular parts or components. The parts or components are themselves Git repositories. They may be integrated as Git submodules (our preferred procedure we explain here). 
> - A specific combination of the modular parts or components is combined with each other in a single SimExp's Git repository, constituting the "experiment repository". 
> - Each (versioned) Git submodule can be identified by its unique Git commit hashes. The SimExp Git repository is characterized on top itself by its commits (major releases may be assigned a Git tag, i.e. its a specific release of this experiment). 

> ✅ **Overall benefits of the HPSC TerrSys SimExp concept**
> 
> Simulations are: Portable, reproducible, lightweight, easy to implement, highly flexible, provenance-enabled, interchangable, open, easy to revise and discuss

**Implications from using Git and Git submodules** 

- A SimExp is usually stored also on a repository hub, as a dedicated [Git repository](https://github.com/orgs/HPSCTerrSys/teams/simulation-experiments/repositories).
- A SimExp Git repository contains a ready-to-use SimExp, which may be \*installed\* to "reproduce" (as close as possible, depending on the compute hard- and software environments) that very simulation or serve as a test case or benchmark or a template and starting point for a new SimExp. (E.g., the [TSMP2 workflow engine](https://github.com/HPSCTerrSys/TSMP2_workflow-engine) features a EURO-CORDEX-type, EUR-12 model domain, ERA5-driven evaluation run with TSMP2 in climate mode.)
- Changes in the Git submodules are tracked in the respective Git repositories of the Git submodules (a submodule in the parent SimExp is just a pointer (i.e., a specific Git commit hash) from the parent SimExp Git repository to another Git repository), but they appear as commits in the SimExp Git history. (`git submodule status --recursive`) 

**Some technical aspects**

- Such a SimExp is stored typically in a dedicated (unified -- if using, e.g., the workflow engine) directory tree on an HPC system. 
- We try to avoid nested submodules, i.e. submodules inside submodules.
- A SimExp may be identified by a unique self-explanatory SimExp-ID (e.g., based on or inspired by the Data Reference Syntax definition from the [CORDEX archive specification](https://zenodo.org/records/15047096)). This is usually the directory name of the SimExp root directory.
- Once running stable, the Git-tracked files of a SimExp (i.e., not the model results or boundary conditions) usually do not change much anymore. As the commit hashes of the submodules as they are checked out are stored with the SimExp parent Git repository, the exact same SimExp is reproduced by means of the unique commit hashes of the SimExp parent Git repo and those of the submodules, if the parent SimExp repo is cloned (i.e., reused). (`git clone --recurse-submodules <url>` clones the parent SimExp repo, initializes the submodules, checks out each submodule at the exact commit hash stored with the parent.)
- If very specific modifications of a submodule are needed, which lead to a substantial divergence from its origin, and which are not relevant to be shared, a submodule may be transferred into a simple directory of the SimExp parent repo and tracked from there.
- Despite the fact that changes of a specific repository (e.g., a model configuration, i.e., namelist file) can be reflected in the Git history or branches, SimExp components are specific for a single purpose, i.e., a 12km simulation would use a different repository in the configuration category as a 3km simulation, and so forth. 
- Despite the fact that once installed and used on an HPC system, the same model components (e.g., external parameter fields) exist alongside each other, each with a different SimExp, they only exist once in the main Git repository hub on GitHub. Depending on redundancies and filesystem and energy efficiency concerns, input data may be shared on a filesystem level by symbolic links.
- Model outputs remain untracked.

**Additional noteworthy implications**

- With each simulation, hashes of the checked-out commits can be stored with the meta data of the simulation results, or a seperate history files, for provenance tracking.
- If the changes to the components of a SimExp and the SimExp changes themselves are made frequently and promptly to their origins on the repository hub, the `repo-versions.txt` file with commit hashes and remote URLs suffices to reproduce a complete SimExp, from building, through preproprocessing, simulation, to archiving.
- Using the SimExp as a parent Git repo (with submodules), unintended changes to, e.g., the configuration and setup, workflow engine etc. can easily be detected.
- If it is not crucial to have frozen versions (=fixed commit hashes) for a SimExp components, the complete SimExp or parts thereof can be very quickly updated. (`git pull && git submodule update --init --recursive`)
- The commit history of the SimExp parent repository may serve as a changelog of the SimExp. 

> **The contents of a SimExp**
>
> A SimExp entails \*everything\* that determines the simulation and its results. I.e., a SimExp contains: 
> - the model source code, the compiled model, the built system incl. machine-dependent compile-time and run-time environments; 
> - the workflow to set up the model domain and to process external parameter input data, initial conditions, and boundary conditions;
> - a workflow engine to efficiently run the model system (test runs, ensemble runs, long climate runs), orchestrating all data > handling, processing, start and restarts, etc.; 
> - configurations for pre-/post-processing set up and the simulation itself; 
> - postprocessing tools for data conversions (e.g., CMORization) and / or analyses; 
> - monitoring tools; 
> - data handling and archival tools; 
> - a short human-readable experiment or run description documentation (aka simulation leaflet); 
> - all input data (or detailed information, configurations and tools to produce these data at any time).

<!-- ToDo: have more git code snippets in text -->

</details>

### The procedure of using TSMP2 with a modularized simulation platform and SimExp

<details>
<summary>Click for details</summary>
<br>

With TSMP2 the SimExp concept is realized through the [TSMP2 workflow engine (WFE)](https://github.com/HPSCTerrSys/TSMP2_workflow-engine). The [TSMP2 WFE has its own documentation](https://hpscterrsys.github.io/TSMP2_workflow-engine); nevertheless a brief overview is given here in the context of the modularized SimExp concept presentation.

> **_NOTE:_** As an experienced user you may still just retrieve TSMP2 including the built system and, e.g., an external parameter file dataset for a specific setup and install, and then you may setup, and run TSMP2 on your own, without, e.g., using the TSMP2 WFE or any namelist we provide. The TSMP2 WFE and the Git-based SimExp handling may be more efficient though.

**SimExp typical directory tree as used by HPSC TerrSys TSMP2** 

```
<SimExp-ID>/
|    
|---- ctl/
|    |---- logs/
|    |---- {pre,sim,pos,viz}_ctl/
|---- dta/
|    |---- forcing/
|    |---- geo/
|    |---- restart/
|    |---- simres/
|---- nml/
|---- src/
|---- run/
```

- `ctl` simulation experiment management (e.g., run-control scripts)
- `dta` all SimExp-related data; `geo` with external parameter fields, `simres` with simulation results, etc., may be symbolic links
- `nml` namelist(s) (maybe multiple namelists from different  repositories)
- `src` source code of the numerical models and some auxiliary tools
- `run` simulation and processing directory, no long-term storage of data 
- `README.md` human-readable experiment description

**Example SimExp with TSMP2**

Some pseudo-code steps to run a real-data pan-European climate simulation using TSMP2 with a EURO-CORDEX CMIP6-downscaling experiment setup and configuration: Please follow the documentation for the [TSMP2 WFE here](https://hpscterrsys.github.io/TSMP2_workflow-engine).

<!-- 
ToDo: 
Some addons.
Additional remarks: Please control that you commit and push whenever you do changes.
-->

</details>

### Existing SimExp

<details>
<summary>Click for details</summary>
<br>

We are in the process of providing our main SimExps (i.e., incl. all parts and components) used with TSMP1 and TSMP2, or ParFlow and eCLM standalone, e.g., from the DETECT CRC project and from EURO-CORDEX CMIP6 simulations through the HPSC TerrSys repository hub. 

<!-- ToDo: Add the example, make sure the repo works, alternatively to above, one might get the very same SimExp straight away from the SimExp repos -->

</details>

</details>

<!--

## Current HPSC TerrSys development team

<details>
<summary>Click for details</summary>
<br>

</details>

## Selected publications

<details>
<summary>Click for details</summary>
<br>

Please see the individual repositories for User Guides, Reference Guides, How-Tos, and Tutorials. The Zenodo listings give an overview of research work done using HPSC TerrSys software.

### With TSMP

### By HPSC TerrSys

</details>

-->

## User guides

<details>
<summary>Click for details</summary>
<br>

Incomplete quick links to user guides (also referenced from the respective parent repositories): 

- **TSMP1/TSMP2**
  - [TSMP1 Docs](https://hpscterrsys.github.io/TSMP/index.html)
  - [TSMP2 Workflow Engine](https://hpscterrsys.github.io/TSMP2_workflow-engine/INDEX.html)
  - [TSMP2-PDAF](https://hpscterrsys.github.io/pdaf/INDEX.html)

- **Component models**
  - [ICON](https://docs.icon-model.org/)
  - [eCLM](https://hpscterrsys.github.io/eCLM/INDEX.html)
  - [ParFlow](https://parflow.readthedocs.io/en/latest/index.html)
  - [OASIS3-MCT](https://gitlab.com/cerfacs/oasis3-mct/-/raw/OASIS3-MCT_5.0/doc/oasis3mct_UserGuide.pdf?inline=false)

- **Tools**
  - [eCLM static file generator](https://github.com/HPSCTerrSys/eCLM_static-file-generator/blob/main/README.md)
  - [SLOTH](https://hpscterrsys.github.io/SLOTH/)

</details>
