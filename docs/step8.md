[de]: assets/de/logos/deIcon.svg
[home]: assets/de/menu_items/homeIcon.svg
[data]: assets/de/menu_items/dataIcon.svg
[apps]: assets/de/menu_items/appsIcon.svg
[analysis]: assets/de/menu_items/analysisIcon.svg
[vice]: assets/de/logos/deviceIcon.png

# Interactive Analyses

!!! tip "Learning Objectives"

    - Request VICE access.
    - Launch and access VICE application.
    - Configure the VICE application and run an analysis.
    - Save the outputs of a VICE application to your Data Store.

**Description:**

The Visual Interactive Computing Environment [![][vice]{width=30}](https://user.cyverse.org/services){target=_blank} [VICE](https://user.cyverse.org/services){target=_blank} allows you to work with popular interactive data science applications such JupyterLab, RStudio, Linux shell and others. In this exercise we will cover a simple introductory use case that allows us to complete our goal of visualizing a phylogenetic tree.

*In this exercise we will:*

1.  Launch an RStudio session, loading the sequence alignments created earlier in the course.

2.  Install an R package and create a phylogenetic tree from the alignment, saving it to a file.

3.  Save our work to the Data Store and terminate the application.

??? tip "Why use VICE"

    The Discovery Environment excels at running compute intensive analyses non-interactively. 
    
    In other words, once you launch a job in the DE, you get an output, but to start a new analysis (for example to tweak parameters), you need to relaunch that job, and await new results. 
    
    This style of computing allows you to run large jobs that require lots of resources. However, several analyses we'd like to do are interactive -- we need to visualize and manipulate parameters on the fly -- for example, creating a figure where you need to see and adjust the results of an upstream analysis. 
    
    This kind of work is often done using tools like R and RStudio, or other programing tools such as Jupyter. Hence VICE!

There are a few common categories of featured interactive applications:

1.  Terminal Access
 	- Basic Ubuntu Terminal: <a href="https://de.cyverse.org/apps/de/5f2f1824-57b3-11ec-8180-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/BASH-terminal-white?style=plastic&logo=gnometerminal"></a>

    - LANDIS-II Command Line Interface: <a href="https://de.cyverse.org/apps/de/098f69c2-1d8e-11ed-9071-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/BASH-terminal-white?style=plastic&logo=gnometerminal"></a>

2.  Integrated Development Environments (IDE)
	- <a href="https://de.cyverse.org/analyses/1f3d3938-5673-11ee-b112-008cfa5ae621" target="_blank"><img src="https://img.shields.io/badge/RStudio-latest-blue?style=plastic&logo=r"></a>
	- <a href="https://de.cyverse.org/apps/de/c2227314-1995-11ed-986c-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/Datascience-latest-orange?style=plastic&logo=jupyter"></a>
 	- <a href="https://de.cyverse.org/apps/de/091c830a-4be1-11ec-aad9-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/VS%20Code-latest-6C33AF?style=plastic&logo=visualstudiocode"></a>
  
3.  Web Server Applications
  	
    - StreamlitApps, ShinyApps, WebGL, HTML5, etc. 

4.  Virtual Desktop Environments (e.g., Apache Guacamole, NoVNC, Xpra)
	- <a href="https://de.cyverse.org/apps/de/b5e65b52-0de5-11ee-9b7a-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/Ubuntu-22.04-green?style=plastic&logo=X.Org"></a>
	- <a href="https://de.cyverse.org/apps/de/4affa3c0-1362-11ee-bf34-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/QGIS-22.04-green?style=plastic&logo=qgis"></a>

CyVerse hosts the container recipes (Dockerfiles) of its featured apps on GitHub: <https://github.com/cyverse-vice/>. These images are maintained by CyVerse staff.


---

<div class="video-container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/PPFD7z4XOVc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

------------------------------------------------------------------------

## Getting VICE Access

To minimize inappropriate use, VICE is a restricted service, currently accessible from CyVerse US. You must request access to use.

1.  Visit the [User Portal](https://user.cyverse.org/services){target=_blank} and **Services**; look for [![][vice]{width=30}](https://user.cyverse.org/services){target=_blank} [DE VICE](https://user.cyverse.org/services){target=_blank} and select the **REQUST ACCESS** link.

??? tip "Ensure your request is approved"

    Ensure that your CyVerse account is associated with a valid email address from an organization ending with `.org`, an educational institution with `.edu`, or government `.gov`. 
    
    We do not grant access to commercial email addresses, e.g., `@gmail.com` `@yahoo.com` `@msn.com` etc.

## Launching a VICE application

??? tip "Featured Apps"

    [![][vice]{width=60}](https://de.cyverse.org/apps){target=_blank}

    CyVerse maintains featured apps from the [Rocker-Project](https://rocker-project/images){target=_blank}, [Project Jupyter](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html){target=_blank}, and [Visual Studio Code](https://code.visualstudio.com/docs/remote/create-dev-container){target=_blank}

    | quick launch | Base Images |
    | ------------ |-------------|
    | <a href="https://de.cyverse.org/apps/de/3548f43a-bed1-11e9-af16-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/Verse-latest-blue?style=plastic&logo=rstudio"></a> | [Rocker-Project](https://rocker-project/images){target=_blank} |
    | <a href="https://de.cyverse.org/apps/de/cc77b788-bc45-11eb-9934-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/Datascience-latest-orange?style=plastic&logo=jupyter"></a> |[Project Jupyter](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html){target=_blank} |
    | <a href="https://de.cyverse.org/apps/de/091c830a-4be1-11ec-aad9-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/VS%20Code-latest-6C33AF?style=plastic&logo=visualstudiocode"></a> | [Visual Studio Code](https://code.visualstudio.com/docs/remote/create-dev-container){target=_blank} |


    These containers are built from community maintianed container stacks, with a few additonal packages for use in CyVerse DE.

1. If necessary, log into the [![][de]{width=25}](https://de.cyverse.org){target=_blank} [Discovery Environment](https://de.cyverse.org){target=_blank}.

2. Click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} and navigate to your `results/` folder in the` tutorial_folder/`; click the (Add Folder button) and create a folder called `rocker_output/` inside your tutorial folder.

3.  Use this Quick Launch link <a href="https://de.cyverse.org/apps/de/48b6e7ae-8b64-11ec-92dc-008cfa5ae621/launch" target="_blank"><img src="https://img.shields.io/badge/Verse-latest-blue?style=plastic&logo=rstudio"></a> or click on [![][apps]{width=20}](https://de.cyverse.org/apps){target=_blank} [Apps](https://de.cyverse.org/apps){target=_blank} to launch thev featured **Rocker RStudio Latest** App. You can also use the DE search bar to search for this application in the Apps category.

4. Launch the application and adjust the following:
    
    Under "Analysis Info", for **Output Folder** click **Browse** and navigate to and select the `rocker_output` created above. click **Next**;

    For "Parameters", under "Input Folder" click **Browse** and navigate to the `tutorial_folder`, then the **results** folder and select the `muscle_output` folder where your Muscle analysis results should be located; click **Select Current Folder**; then **Next**;
    
    Click **Next** to skip Advanced Settings;
   
    Click **Launch Analysis** to launch your application

5.  In the navigation, click on the (Analyses) view. Your application will be listed as "Submitted" for a few minutes (usually just a few, but more depending on both the size of the application software and any imported datasets).

6.  When the Status of the launch is Running, click on the (link out icon); a new tab where your VICE application will run should open in your browser.

??? tip "Launching VICE Apps"

    Even when the application has entered 'Running' status, you may still have to wait some additional time for input data to be transferred onto the resource with the new container. 

## Completing our analysis in R

Once you have your RStudio session, it will behave the same as a RStudio session running on your local Desktop. 

Some potential benefits of running RStudio in VICE include more processing power (especially if you choose additional resources at launch -- see the Advanced Settings).

Since this session is running on CyVerse hardware, transferring large data will also happen at increased speed. To complete our analyses, we will install the [`ape` package](https://cran.r-project.org/web/packages/ape/index.html){target=_blank} and compute a phylogenetic tree.

??? tip "Using RStudio"

    While you don't need to be an expert R user to complete this section, familiarity with R will help since we won't be going into specific detail about this example.

??? tip "Locating your files in RStudio"

    The data we loaded at launch of the VICE application will be in the `/home/rstudio/work/data/input` directory.

From the R console, enter the following commands:

``` {R title="script.r"}
# install and load the needed R library
install.packages("ape")
library(ape)

#Read in the aligned DNA fasta file
alignment <- read.FASTA ("~/work/data/input/muscle_output/fasta.aln", type="DNA")

# Create a distance matrix for the sequences
dist_mtrx <- dist.dna(alignment)

#Compute a neighbor-joining tree
nj_tree <- nj(dist_mtrx)

# plot the tree
plot.phylo(nj_tree)

# save the tree to a file
write.tree(nj_tree, file = "~/work/data/output/tree.newick")

#OR save to your CyVerse Data Store directly in the file browser
write.tree(nj_tree, file = "~/work/home/YOUR_CYVERSE_USERNAME/tutorial_folder/rocker_output/tree.newick")
```

You should have visualized the resulting tree and also created the file `tree.newick` in your work directory.

## Terminating your VICE session and saving work to the Data Store

Once you have completed your work, you can save your work to the Data Store and terminate your VICE application.

??? tip "Extending Analysis Time"

    VICE applications typically have a 48-hour run time. 
    
    Unless you request an extension, your application will save data in the `~/work/data/outputs` folder to your `analyses/` folder when it terminates. 
    
    It is recommended that you save your work to the Data Store before time expires.

1.  In the Analyses pane of the Discovery Environment, select your unning RStudio VICE application.

2.  Under **More Actions**, select **Terminate**; confirm Termination on the pop-up notice.

3.  When the VICE application has the status completed, click the folder icon to view the folder on your data store where results will be written. It may take time for all outputs to be saved depending on the size of the data generated.

??? tip "Transfering your data"

    You don't have to terminate your analyses to save your work to the Data Store. 
    
    From within the RStudio environment using the terminal, you can use iCommands to transfer data (See Data Store Guide on iCommands). 

    RStudio does allow you to download files and plots directly back to your local computer. Use the "Export" features present in the file pane.

------------------------------------------------------------------------

**Output/Results**

| Output | Description |
|--------|-------------|
| `tree.newick` |  A Newick-formatted phylogenetic tree file which can visualized using your choice of tools. | |   

------------------------------------------------------------------------

## Self Assessment Questions

??? question "What kind of applications are supported in VICE?"
 
    **A** Applications with their own graphical interface

    **B** Open-source applications

    **C**  Applications that have interactive visualizations

    **D**  All of the above
    
    ??? Success "Answer" 
        
        Correct answer is **D**


??? question "Which of the following are restrictions on using VICE?"

    **A**  You must request access on the CyVerse user portal
    
    **B**  VICE applications have a 48-hour runtime limit
    
    **C**  You must install VICE applications yourself

    **D**  A and B

    **E**  C only

    ??? Success "Answer"

        Correct answer is **D**, you must request separate access to use VICE. 
        
        There is a default 48-hour run time but you can extend your time by requesting this in the Analysis view for the launched application.

-----------------------------------------------------------------------

**Fix or improve this documentation**

  - Search for an answer:
     [CyVerse Learning Center](https://learning.cyverse.org){target=_blank}
  - Send feedback: <tutorials@cyverse.org>
  
------------------------------------------------------------------------

[:material-rocket: Learning Center Home](http://learning.cyverse.org/)
