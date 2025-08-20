**Welcome to the profile page of the Centre for High-Performance Scientific Computing in Terrestrial Systems (HPSC TerrSys) organization GitHub account.**

***HPSC TerrSys enables geosciences by high-performance computing (HPC).***

The HPSC TerrSys repositories are the official home of

- the **[encore Community Land Model (eCLM)](https://github.com/HPSCTerrSys/eCLM)**, a refactored [Community Land Model (CLM) version 5](https://www.cesm.ucar.edu/models/clm), for effiicient stand-alone-use and flexible model integration with atmospheric and hydrologic models,
- the fully coupled, physics-based **Terresterial Systems Modeling Platform ([TSMP1](https://github.com/HPSCTerrSys/TSMP) and [TSMP2](https://github.com/HPSCTerrSys/TSMP2))** regional climate/Earth system model (RCSM, RESM), linking the [ICON atmospheric model](https://www.icon-model.org) with the [eCLM land surface model](https://github.com/HPSCTerrSys/eCLM) and with the [integrated ParFlow hydrologic model](https://github.com/parflow/parflow) through the [OASIS-MCT coupler](https://gitlab.com/cerfacs/oasis3-mct),
- [PDAF-based parallel](https://github.com/PDAF/PDAF) **data assimilation versions** of TSMP1 and TSMP2 and eCLM, 

plus software tools for the pre- and postprocessing and analysis of model data, all necessary auxiliary simulation tools (built systems, workflow engines, external parameter file generators, etc.), complete simulation experiments (incl. configurations, input and reference data), as well as documentation, unless otherwise stated, provided as free and open source software (FOSS), or under a CC BY license for many datasets (see individual LICENSE files).

# Who we are - research groups behind HPSC TerrSys

<details>
<summary>Click for details</summary>
<br>

HPSC TerrSys software, input data etc. are developed and produced by and under the auspices of the research groups of 

- **Stefan Kollet** ([Integrated Modelling of Terrestrial Systems at FZJ/IBG-3](https://www.fz-juelich.de/en/ibg/ibg-3/research-groups/modelling-terrestrial-systems/integrated-modelling-of-terrestrial-systems)),
- **Harrie-Jan Hendricks-Franssen** ([Stochastic Analysis of Terrestrial Systems at FZJ/IBG-3](https://www.fz-juelich.de/en/ibg/ibg-3/research-groups/modelling-terrestrial-systems/stochastic-analysis-of-terrestrial-systems)), and 
- **Daniel Caviedes-Voullieme** ([Simulation- and Data-Lab Terrestrial Systems at FZJ/JSC](https://www.fz-juelich.de/en/ias/jsc/about-us/structure/simulation-and-data-labs/sdl-terrestrial-systems))

at [Research Centre Juelich (Forschungszentrum Jülich, FZJ](https://www.fz-juelich.de/en)) in the [Helmholtz Association of German Research Centres (HGF)](https://www.helmholtz.de/en/). Founded in 2011, [HPSC TerrSys](https://www.hpsc-terrsys.de/en) is a virtual competence center within the [Geoverbund ABC/J](https://www.geoverbund-abcj.de/en), the geoscientific network of the Aachen-Bonn-Cologne-Jülich research region, in Germany.

Very broadly our research interests are on the functioning and (climate change induced) changes of coupled geo-ecosystems, the water and energy cycles therein, characterized by complex feedbacks and interactions, from the groundwater, through the land surface, to the atmosphere, including human interventions, such as anthropogenic water use. 

<!-- add technical e-mail address --> 
Here we provide and share some of our core scientific computing tools for efficient joint cross-institutional development, community reuse, feedback, and potential collaboration, as well as for internal use within HPSC TerrSys.
</details>

# What we provide and how to use the HPSC TerrSys GitHub repositories

<details>
<summary>Click for details</summary>
<br>

This profile page is the top-level, overarching starting point where we

- list different types or categories of repositories, grouped in GitHub Teams, each with their own short description,
- explain the relation of the types or categories of repositories and information provided therein, as part of a modularized simulations,
- introduce a uniform nomenclature we use throughout the repositories, and 
- elaborate on our concept of a "simulation experiment". 

Although each repository provides an independent, mostly standalone piece of information or software and has its own documentation (e.g., as a `README.md` project overview or GitHub Pages), we follow a highly modularized software development, maintenance, and deployment paradigm. Here individual, independent Git repositories are combined (hierarchically), usually by means of Git submodules, to constitute, e.g., a coupled model system or simulation experiment. This leads to a lightweight, transparent, reproducible, maintainable, scalable, versioned, and provenance-enabled software infrastructure.

The TSMP2 RESM follows this paradigm, that supports its properties and features as a versatile "platform" to built and expand our own simulation experiments on.

## Types of information and repository categories (=GitHub Teams)

- [Coupled model systems](https://github.com/orgs/HPSCTerrSys/teams/coupled-model-systems/repositories)
- [Individual model systems](https://github.com/orgs/HPSCTerrSys/teams/individual-model-systems/repositories)
- [Workflow engines](https://github.com/orgs/HPSCTerrSys/teams/workflow-engines/repositories)
- [(Pre-/Post-)processing and setup tools](https://github.com/orgs/HPSCTerrSys/teams/processing-and-setup/repositories)
- [Configurations](https://github.com/orgs/HPSCTerrSys/teams/configurations/repositories)
- [Static or external parameter model input files](https://github.com/orgs/HPSCTerrSys/teams/external-parameters/repositories)
- [Simulation experiments](https://github.com/orgs/HPSCTerrSys/teams/simulation-experiments/repositories)
- [(Generic) data analytics tools](https://github.com/orgs/HPSCTerrSys/teams/data-analytics/repositories)
- [(Model system) auxiliary tools](https://github.com/orgs/HPSCTerrSys/teams/auxiliary-tools/repositories)

These are the current GitHub teams, which contain one or more repositories each.

Each individual repository is assigned to a single type of information or category only.

See [here for the full (unsorted) list](https://github.com/orgs/HPSCTerrSys/repositories) of HPSC TerrSys repositories.

## Research group code ownerships and development leads

Repositories in the above categories are under the auspices of either one of the following research groups at FZJ:

<!-- create teams and add respective repositories -->
- S. Kollet group
- H.-J. Hendricks-Franssen group
- D. Caviedes-Voullieme group

</details>

<!-- 
# How to work with the repositories, our concept of a fully modularized modeling platform and "simulation experiment"

<details>
<summary>Click for details</summary>
<br>

## A modularized simulation platform

Splitting one can maintain
use standalone or in combination

## How to use TSMP2

either standalone or a combination
this is not the documentation for the TSMP2 model 
The overall concepot of using the model system us described here.
see extra docs perhaps, or make this collapsible

## What is a simulation experiment

all components make up a simulation experiment

</details>
-->
<!--
# Current HPSC TerrSys development team

<details>
<summary>Click for details</summary>
<br>

The current development team as of mid 2025 in alphabetical order behind the HPSC TerrSys GitHub repositories with their respective main responsibilities:

<add names after consent>
<ORCIDs?, certainly no e-mails>

See the LICENSE and/or CONTRIBUTERS files or list of Contributors in each repository for details and previous contributors.

</details>
-->
<!--
# Selected publications

<details>
<summary>Click for details</summary>
<br>

Please see the individual repositories for User Guides, Reference Guides, How-Tos, and Tutorials. The Zenodo listings give an overview of research work done using HPSC TerrSys software.

<Zenodo listing? see ParFlow>

## With TSMP

## By HPSC TerrSys

</details>
-->

# User guides

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

<!-- examples: parflow ncar icon cordex -->