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
| On CyVerse | `ortho.tif` | View the [example folder](https://data.cyverse.org/dav-anon/iplant/commons/cyverse_curated/Gillan_Ecosphere_2021/raster_products/Sept_2019/){target=_blank} |

## Launch an Executable Analysis

[de]: assets/de/logos/deIcon.svg
[home]: assets/de/menu_items/homeIcon.svg
[data]: assets/de/menu_items/dataIcon.svg
[apps]: assets/de/menu_items/appsIcon.svg
[analysis]: assets/de/menu_items/analysisIcon.svg

1. If necessary, log into the [![][de]{width=25}](https://de.cyverse.org){target=_blank} [Discovery Environment](https://de.cyverse.org){target=_blank}.

2. Click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} and navigate to your `tutorial_folder/`; click the (Add Folder button) and create a new folder called `gdal_output/` inside your `tutorial_output` folder.

3.  Click [![][apps]{width=20}](https://de.cyverse.org/apps){target=_blank} [Apps](https://de.cyverse.org/apps){target=_blank} - Applications (including VICE interactive applications); You will begin in the **Featured Apps** section; Click on the application name in the search bar. Type "`gdal`" and hit Return. There should be an app with this name in the search results.

4.  Under "Analysis Info", for **Output Folder** click **Browse** and navigate to and select the **tutorial_folder/gdal_output** created above. No other changes are needed at this step, but you may edit the analysis name or comments (optional)

5. Click "Next :material-arrow-right:" or click on icon :material-numeric-2-circle: number "2" in the **Advanced Settings (optional).**. Set the "Minimum CPU Cores" to 8, and "Minimum Memory" to 64 GiB. Leave "Minimum Disk Space" open. Note: the "**Select Maximums**" cannot be changed - this tool can use up to 128 cores, which is the average size of our newer compute nodes in the Discovery Environment.
6.  Under "Select input data" click Browse, then navigate to the `raw_data/` folder in the `tutorial_folder` and select a valid geotiff .tif file.

7.  Under the optional "Advanced Settings", make no changes. If required, some analyses may be launched with requests for more minimum Resource Requirements, but this may cause those analyses to sit longer in the submission queue until a node matching those minimum requirements becomes available; click **Next**.

8.  Click **Launch Analysis**.

9.  You will receive a notification and be redirected to the [![][analysis]{width=20}](https://de.cyverse.org/analyses){target=_blank} [Analyses](https://de.cyverse.org/analyses){target=_blank} page.

10. When the analysis has the status **Completed**, you may click the folder icon next to the analysis name, to navigate to and browse the outputs for this analysis. You may need to refresh your web browser to see the updated status.

!!! Danger "Setting minimums"

    As a general rule of thumb, the "**Advanced Settings (optional)**" tab can be passed over when starting an analysis. The Kubernetes scheduler provides everyone with at least 4 CPUs and 16 GiB of memory.

    By asking for the "minimum" you're locking in that amount for your analysis. If the system is busy and there are many users on the VICE cluster, asking for an entire 128 CPU node may leave you in a queue, waiting minutes or hours for a free resource to become available. 

    Its a good rule of thumb, and a neighborly courtesy to other users not to ask for maximum CPU and RAM unless absolutely necessary. 

    More importantly, asking for larger minimums will result in a faster burn rate for your CPU hours, 1 allocation unit = 1 CPU core / hour.

------------------------------------------------------------------------

## Output/Results

| Location | File | Example |
|----------|------|---------|
| `pdal_outputs/`  | output folder | [View the example `pdal_outputs/`](https://data.cyverse.org/dav-anon/iplant/home/shared/usda/usfs/r3/coconino/training_data/mahan){target=_blank} |
| `ept2copc.json` | PDAL pipeline `.json` | the input for the app |
| `mahan.copc.laz` | `.laz` format with COPC |
| `mahan_dem.tif` | `.tif` file from GDAL | 

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
  - Send feedback: <tutorials@cyverse.org>
  
------------------------------------------------------------------------

[:material-rocket: Learning Center Home](http://learning.cyverse.org/)
