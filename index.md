<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

# **CyVerse Self-Guided Course** 

This self-guided course will take you through the basics of using CyVerse USA.

------------------------------------------------------------------------

**Tutorial Maintainer(s)**

Who to contact if this guide needs fixing. You can also email <learning@cyverse.org>

| Maintainer | Institution | Contact |
|------------|-------------|---------|
| Michele Cosi | University of Arizona | <cosi@arizona.edu> |
|  Jeffrey Gillan | University of Arizona | <jgillan@arizona.edu> |
|  Tyson Lee Swetnam | University of Arizona | <tswetnam@cyverse.org> |

------------------------------------------------------------------------

## Table of Contents

* [Agenda](agenda.md) 
* [Course Overview](step1.md)
* [CyVerse Background](step2.md)
* [Tour of the Discovery Environment (DE)](step3.md)
* [Data Management I](step4.md) 
* [Data Management II](step5.md) 
* [Data Management III](step6.md) 
* [DE: Executable Analyses](step7.md)
* [DE: Interactive Analyses](step8.md) 
* [Advanced Applications](final_step.md) 

## Perequisites

### Downloads, access, and services

*In order to complete this tutorial you will need access to the
following services*

| Prerequisite | Preparation Notes | Link/Download |
|--------------|-------------------|---------------|
| CyVerse account | You will need a CyVerse account to complete this exercise | [User Portal](https://user.cyverse.org){target=_blank} |
  VICE Access | You must have permission to use Discovery Environment VICE applications; request access on the user portal (under 'Services') | [Request Access](https://user.cyverse.org/services){target=_blank} |

*You will also need software to transfer data into and out of the Data Store. We recommend using Cyberduck for Mac and Windows users, and iCommands or GoCommandsfor Linux users.*

| Prerequisite | Preparation Notes | Link/Download |
|--------------|-------------------|---------------|
| [CyberDuck](https://learning.cyverse.org/ds/cyberduck/){target=_blank} | 3rd party software for upload/download to Data Store | [Windows, Mac OS X](https://cyberduck.io){target=_blank} |
| [GoCommands](https://learning.cyverse.org/ds/gocommands/) | CyVerse created software for upload/download to Data Store | [Windows, Linux, Mac OS X](https://github.com/cyverse/gocommands){target=_blank} |
|[iCommands](https://learning.cyverse.org/ds/icommands/){target=_blank} | iRODS Consortium software for upload/download | [Linux, Mac OS X](https://docs.irods.org/4.3.0/icommands/user/){target=_blank} |

### Platform(s)

*We will use the following CyVerse platform(s):*

| Platform | Interface | Link  | Platform Tour |
|----------|-----------|-------|---------------|
| [![DS](assets/de/menu_items/dataIcon.png){width="20"}](https://de.cyverse.org/data){target=_blank} [Data Store](https://de.cyverse.org/data){target=_blank} | GUI & CLI | [Data Store](https://cyverse.org/data-store){target=_blank}{target=_blank} | [Data Store Guide]() |              
| [![DE](assets/de/logos/deIcon.png){width="20"}](https://de.cyverse.org/data){target=_blank} [Discovery Environment](https://de.cyverse.org/de){target=_blank} | GUI | [DE](https://cyverse.org/discovery-environment) | [DE Guide](){target=_blank} |         

### Application(s) used

**Discovery Environment App(s):**

| App Name | Version | Description | App Link | Notes/Other |
|----------|---------|-------------|----------|-------|      
| RStudio Geospatial | `4.3.1` | [Rocker-Project RStudio](https://rocker-project.org/images){target=_blank} | <a href="https://de.cyverse.org/apps/de/3031d3b0-15e7-11ee-847b-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/geospatial-4.3.1-blue?style=plastic&logo=rstudio"></a> | [:material-github: Dockerfile](https://github.com/cyverse-vice/rstudio-geospatial){target=_blank} |
| Jupyter Lab Datascience | `4.0.1` | [Project Jupyter](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html){target=_blank} | <a href="https://de.cyverse.org/apps/de/cc77b788-bc45-11eb-9934-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/Datascience-latest-orange?style=plastic&logo=jupyter"></a> | [:material-github: Dockerfile](https://github.com/cyverse-vice/jupyterlab-datascience){target=_blank} |
| Ubuntu Desktop | `22.04` | [Kasm Ubuntu](https://hub.docker.com/r/kasmweb/ubuntu-jammy-desktop){target=_blank} | <a href="https://de.cyverse.org/apps/de/26e8dca0-550b-11ee-8aa2-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/Ubuntu-22.04-green?style=plastic&logo=X.Org"></a> | [:material-github: Dockerfile](https://github.com/cyverse-vice/kasm-ubuntu){target=_blank} |

-----------------------------------------------------------------------

**Funding and Citations:**

CyVerse is funded by the Arizona Board of Regents the National Science Foundation [![NSF](assets/nsf.png){width="25"}](https://nsf.gov){target=_blank} under Award Numbers:

[![NSF-0735191](https://img.shields.io/badge/NSF-0735191-blue.svg)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=0735191){target=_blank}  [![NSF-1265383](https://img.shields.io/badge/NSF-1265383-blue.svg)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1265383){target=_blank}  [![NSF-1743442](https://img.shields.io/badge/NSF-1743442-blue.svg)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1743442){target=_blank}

Please cite CyVerse appropriately when you make use of our resources, see [CyVerse citation policy](https://cyverse.org/policies/cite-cyverse){target=_blank}.

-----------------------------------------------------------------------

**Fix or improve this documentation**

  - Search for an answer:
     [CyVerse Learning Center](https://learning.cyverse.org){target=_blank}
  - Send feedback: <tutorials@cyverse.org>
  
------------------------------------------------------------------------

[:material-rocket: Learning Center Home](http://learning.cyverse.org/)
