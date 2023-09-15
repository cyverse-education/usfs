# Analysis with the Discovery Environment

!!! tip "Learning Objectives"

    - Understand basic analysis capabilities of the Discovery Environment

    - Find an app and launch an analysis
    
    - Monitor analysis results
    
    - Access analysis results

**Description:**

In this module, we introduce executable analyses in the CyVerse Discovery Environment and demonstrate how to launch and view their output.

> <div class="video-container">
> <iframe width="560" height="315" src="https://www.youtube.com/embed/LBtyt5bG2VY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
> </div>

------------------------------------------------------------------------

### Input Data:

| Location | File | Example |
|----------|------|---------|
| On CyVerse | `DE_sample_plants.fas` | View the [example folder](https://datacommons.cyverse.org/browse/iplant/home/shared/cyverse_training/cyverse_mooc){target=_blank} |

## Find a Tool and Launch an Analysis

[de]: assets/de/logos/deIcon.svg
[home]: assets/de/menu_items/homeIcon.svg
[data]: assets/de/menu_items/dataIcon.svg
[apps]: assets/de/menu_items/appsIcon.svg
[analysis]: assets/de/menu_items/analysisIcon.svg

1. If necessary, log into the [![][de]{width=25}](https://de.cyverse.org){target=_blank} [Discovery Environment](https://de.cyverse.org){target=_blank}.

2. Click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} and navigate to your `results/` folder in the` tutorial_folder/`; click the (Add Folder button) and create a new folder called `muscle_output/` inside your tutorial folder.

3.  Click [![][apps]{width=20}](https://de.cyverse.org/apps){target=_blank} [Apps](https://de.cyverse.org/apps){target=_blank} - Applications (including VICE interactive applications); search for "**Muscle-3.8.31**" with the search bar at top; Click on the application name to open the application.

4.  Under "Analysis Info", for **Output Folder** click **Browse** and
    navigate to and select the **muscle\_output** created above. No
    other changes are needed at this step, but you may edit the analysis
    name or comments (optional).
5.  Under "Select input data" click Browse, then navigate to the `raw_data/` folder in the `tutorial_folder` and select (checkbox) the `DE_sample_plants.fas` previously uploaded.

6.  Under "Sequence Type", select **DNA**.

7.  Under the optional "Advanced Settings", make no changes. If required, some analyses may be launched with requests for more minimum Resource Requirements, but this may cause those analyses to sit longer in the submission queue until a node matching those minimum requirements becomes available; click **Next**.

8.  Click **Launch Analysis**.

9.  You will receive a notification and be redirected to the [![][analysis]{width=20}](https://de.cyverse.org/analyses){target=_blank} [Analyses](https://de.cyverse.org/analyses){target=_blank} page.

10. When Muscle analysis has the status **Completed**, you may click the folder icon next to the analysis name, to navigate to and browse the outputs for this analysis. You may need to refresh your web browser    to see the updated status.

------------------------------------------------------------------------

## Output/Results

| Location | File | Example |
|----------|------|---------|
| `muscle_output/`  | logs folder | [View the example `muscle_output/`](https://datacommons.cyverse.org/browse/iplant/home/shared/cyverse_training/cyverse_mooc/tutorial_folder/results/muscle_output){target=_blank} |
| `clstalw.aln` | `.aln` are multi-alignment files |
| `fasta.aln` | | 
| `phylip_interleaved.aln` | | 
| `phylip_sequential.aln` | |

------------------------------------------------------------------------

### Self Assessment Questions

??? Question "Which of the following are **true** about Docker containers?"

    **A** They share the host OS
    
    **B** They have process-level isolation.
    
    **C** They are are heavyweight.

    **D** They have a startup time in the minutes range.

    ??? Success "Answer"

        Correct answer are **A** & **B**.

??? Question "Which of the following are incorrect about Docker containers?"
    
    **A** Dockerfiles are a recipe for creating Docker images.
    
    **B** Docker containers are a collection of Dockerfiles.
    
    **C** Docker images get built by running a Docker command which uses the Dockerfile.

    **D** Docker containers are running instances of a Docker image.

    ??? Success "Answer"
    
        The incorrect statement is **B**.

-----------------------------------------------------------------------

**Fix or improve this documentation**

  - Search for an answer:
     [CyVerse Learning Center](https://learning.cyverse.org){target=_blank}
  - Ask us for help:
    click the Intercom icon ![Intercom](assets/intercom.png){ width="25" } on the lower right-hand side of the page
  - Report an issue or submit a change:
    [Github Repo Link](https://github.com/cyverse-learning-materials/){target=_blank}
  - Send feedback: <tutorials@cyverse.org>
  
------------------------------------------------------------------------

[:material-rocket: Learning Center Home](http://learning.cyverse.org/)