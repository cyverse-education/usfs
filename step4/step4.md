[de]: assets/de/logos/deIcon.svg
[home]: assets/de/menu_items/homeIcon.svg
[data]: assets/de/menu_items/dataIcon.svg
[apps]: assets/de/menu_items/appsIcon.svg
[analysis]: assets/de/menu_items/analysisIcon.svg
[shell]: assets/de/menu_items/webshellIcon.svg
[team]: assets/de/menu_items/teamsIcon.svg
[bank]: assets/de/menu_items/bank.svg
[help]: assets/de/menu_items/helpIcon.svg

# Data Management I

!!! tip "Learning Objectives"

    - Create private directories in the Data Store using the Discovery Environment (DE) User Interface (UI)
    - Create, upload & download data from DE UI
    - Understand file permissions in the DE UI
    - Download data from the Data Store


**Description:**

In this module, we introduce the Data Store and its management in the Discovery Environment

---

> <div class="video-container">
> <iframe width="560" height="315" src="https://www.youtube.com/embed/yDptqWLfxXk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
> </div>

------------------------------------------------------------------------

## Create a Directory in your personal account space

In your :material-home: home create a folder named `tutorial_folder` by clicking on the :fontawesome-solid-folder-plus: folder with a + icon. 

Inside that folder create two additional folders: `raw_data/` and `results/`

------------------------------------------------------------------------

**Output/Results**

| Output | Description |
|--------|-------------|
| `/tutorial folder/` <br> `tutorial_folder/raw_data` <br> `tutorial_folder/results` | - We will cover in detail how to create and share folders in the next steps of the course. <br> - These will contain example data from future steps in the tutorial |

## Downloading data from the Discovery Environment

??? Tip "Dropdown Menu"

    The dropdown menu (:material-home: `username`)allows you to navigate between your home directory in the Data Store (i.e. your username), and other CyVerse data collections such as files shared with you (i.e. :material-folder-account: "Shared with Me"), and files shared by the CyVerse community (i.e.:octicons-people-16: "Community Data"). You may also access files located in your :fontawesome-solid-trash: "Trash" folder.

1. If necessary, log into the [![][de]{width=25}](https://de.cyverse.org){target=_blank} [Discovery Environment](https://de.cyverse.org){target=_blank}.

2. Click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} to browse your collection of files in the Data Store.

3. In the top left of the page, you should see your username with a dropdown arrow next to it; Click on your username, then click Community Data in the dropdown menu.

4. From the **Community Data** directory, scroll down until you find `usda/` folder, and click on it. Then navigate to the `/usda/usfs/r3/coconino/training_data/` folder, then `mahan/`, which contains the sample data. 

??? Info "Access points for data in the Data Store"

    Path to the iRODS data store via [`iCommands`](https://learning.cyverse.org/ds/icommands/){target=_blank} or [`GoCommands`](https://learning.cyverse.org/ds/gocommands/){target=_blank}

    ```
    /iplant/home/shared/usda/usfs/r3/coconino/training_data/mahan/
    ```

    `https://de.cyverse.org` - Discovery Environment

    [https://de.cyverse.org/data/ds/iplant/home/shared/usda/usfs/r3/coconino/training_data/mahan](https://de.cyverse.org/data/ds/iplant/home/shared/usda/usfs/r3/coconino/training_data/mahan){target=_blank}

    `https://data.cyverse.org` - WebDav Interface

    [https://data.cyverse.org/dav-anon/iplant/projects/usda/usfs/r3/coconino/training_data/mahan/](https://data.cyverse.org/dav-anon/iplant/projects/usda/usfs/r3/coconino/training_data/mahan/){target=_blank}

1.  Click (Select) the checkbox next to the `ept2copc.json` file to select it.

2.  Click on the **More Actions** button on the upper right and select the **Download** option to download the file to your local computer.

3. Check your Downloads directory on your personal computer.

??? Tip "Downloads in the browser"

    We don't recommend downloading many (>10) files or large (>2GB) files directly from the Discovery Environment. 
    
    Because files transferred in this way make use of `https://` protocols these are slower and more often subject to failure for larger data sets. 
    
    [CyVerse Cyberduck Profile](https://learning.cyverse.org/ds/cyberduck/){target=_blank}, [GoCommands](https://learning.cyverse.org/ds/gocommands/){target=_blank} or [iCommands](https://docs.irods.org/master/icommands/user/){target=_blank} (discussed below and in the next section) are recommended for these uses.

## Uploading Files to the Data Store via Discovery Environment

1. On your local computer, use any text editor to create a file called `README.md`. You may wish to save it in the same place you have the `ept2copc.json` file (i.e. your Desktop, Downloads Folder, etc.).

2. In the `README.md` file, add several pieces of information about the `ept2copc.json` file you just downloaded:

``` 
   Name of file: `ept2copc.json`
   Type of file: `JSON` file containing PDAL pipeline scripts
   Type of data: lidar .las or .laz
```
Adding a simple README with this sort of information can quickly make your data more [FAIR](https://www.go-fair.org/fair-principles/){target=_blank}.
    
??? Note "Discovery Environment file"

    Make sure you save this as a markdown text file (`.md`), other file formats (e.g. `.docx`) may not be rendered in the Discovery Environment's file editor.

3.  In the Discovery Environment, click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} to access your home folder; you can access this from the same dropdown menu where you previously selected **Community Data**.

4.  Navigate to the `tutorial_folder` directory you created earlier.

5.  Click the **Upload** icon in the upper right, then select **Browse Local**. Then navigate to your `README.md` file and select it.

6.  It may take a moment, but your `README.md` file should now be
    uploaded to your `tutorial_folder` on the Data Store; you may
    need to refresh your web browser to see the update.

------------------------------------------------------------------------

## Output/Results

| Location | File | Example |
|--------|-------------|---------|
| On CyVerse | `README.md` | View the [example folder](https://datacommons.cyverse.org/browse/iplant/home/shared/usda/usfs/r3/coconino/training_data/mahan/){target=_blank} |
| On your Computer | `ept2copc.json`, `README.md` | ||                      

### Self Assessment Questions

??? Question "What do the letters in **FAIR** refer to?"

    **A**  Fixable, Assessable, Interpretable, Recyclable
    
    **B**  Fast Access In Repetition
    
    **C**  Findable, Accessible, Interoperable, Reusable
    
    **D**  Fixable, Automated, Intersectional, Reducible

    ??? Success "Answer"

        The correct answer is **C**.

??? Question "**True or False** is FAIR data is the same as Open data?"

    ??? Success "Answer"
    
        **False.** Open data must be free for use and distribution by anyone, whereas data can be limited in access while still being FAIR.
        
        Likewise, Open data are not necessarily easily findable,interoperable, or reusable.


??? Question "Which of the following are NOT true of the process of making your data FAIR?"

    **A**  It will be the same regardless of discipline

    **B**  It may require some technical skills
    
    **C**  It can be easier with CyVerse
    
    **D**  It happens on a continuum, not a binary FAIR/not FAIR

    ??? Success "Answer"

        The correct answer is **A** Making your data FAIR **can** vary widely by discipline. 
        
        For example, human health data may be subject to stricter security and more limited sharing, which must be accounted for when attempting to make data FAIR.

??? Question "**True or False** is adding a README file a quick way to make your data more FAIR?"

    ??? Success "Answer"

        **True**, a README can provide quick access to metadata and is easily discovered within a given directory.

-----------------------------------------------------------------------

**Fix or improve this documentation**

  - Search for an answer:
     [CyVerse Learning Center](https://learning.cyverse.org){target=_blank}
  - Send feedback: <tutorials@cyverse.org>
  
------------------------------------------------------------------------

[:material-rocket: Learning Center Home](http://learning.cyverse.org/)
