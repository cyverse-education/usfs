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

    -   Describe the components of FAIR data
    -   Describe the Data Lifecycle
    -   Download data from the Data Store
    -   Create a README file and upload it to the Data Store

**Description:**

In this module, we introduce the concepts of FAIR data and the Data Lifecycle and demonstrate how to move data between your computer and the CyVerse Data Store.

---

> <div class="video-container">
> <iframe width="560" height="315" src="https://www.youtube.com/embed/yDptqWLfxXk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
> </div>

Here is a link to the [FAIR Data assessment tool](https://ardc.edu.au/resources/working-with-data/fair-data/fair-self-assessment-tool/){target=_blank} mentioned in the video.


------------------------------------------------------------------------

## Downloading data from the Discovery Environment

??? Tip "Dropdown Menu"

    The dropdown menu (:material-home: `username`)allows you to navigate between your home directory in the Data Store (i.e. your username), and other CyVerse data collections such as files shared with you (i.e. :material-folder-account: "Shared with Me"), and files shared by the CyVerse community (i.e.:octicons-people-16: "Community Data"). You may also access files located in your :fontawesome-solid-trash: "Trash" folder.

1. If necessary, log into the [![][de]{width=25}](https://de.cyverse.org){target=_blank} [Discovery Environment](https://de.cyverse.org){target=_blank}.

2. Click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} to browse your collection of files in the Data Store.

3. In the top left of the page, you should see your username with a dropdown arrow next to it; Click on your username, then click Community Data in the dropdown menu.

4. From the **Community Data** directory, scroll down until you find `cyverse_training/` folder, and click on it. Then navigate to the `cyverse_mooc/` folder, then `muscle_3_8_31/01_muscle_input/`, which contains example data. This is the full file path, which should show up as part of your URL:

```
/iplant/home/shared/cyverse_training/cyverse_mooc/muscle_3_8_31/01_muscle_input/
```

5.  Click (Select) the checkbox next to the `DE_sample_plants.fas` file to select it.

6.  Click on the **More Actions** button on the upper right and select the **Download** option to download the file to your local computer.

??? Tip "Downloads in the browser"
    We don't recommend downloading many (more than 10) or large (more than 2GB) files directly from the Discovery Environment at one time. 
    
    Since files transferred in this way make use of HTML protocols these are slower and more often subject to failure for larger data sets. 
    
    [Cyberduck](https://cyberduck.io){target=_blank} or [iCommands](https://docs.irods.org/master/icommands/user/){target=_blank} (discussed below and in the next section) are recommended for these uses.

## Uploading a File to the Discovery Environment

1. On your computer, use any text editor to create a file called `README.txt`. You may wish to save it in the same place you have the `DE_sample_plants.fas` file (i.e. your Desktop, Downloads, etc.).

2. In the `README.txt` file, add several pieces of information about the `DE_sample_plants.fas` file you just downloaded:

``` 
   Name of file: `DE_sample_plants.fas`
   Type of file: `FASTA` file containing DNA sequences
   Type of organism: plants
```
Adding a simple README with this sort of information can quickly make your data more [FAIR](https://www.go-fair.org/fair-principles/){target=_blank}.
    
??? Note "Setting file type"

    Make sure you save this as a plain text file (`.txt`), other file formats (e.g. `.docx`) may not be rendered in the Discovery Environment editor.

3.  In the Discovery Environment, click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} to access your home folder; you can access this from the same dropdown menu where you previously selected **Community Data**.

4.  Navigate to the `tutorial_folder` directory you created earlier.

5.  Click the **Upload** icon in the upper right, then select **Browse Local**. Then navigate to your `README.txt` file and select it.

6.  It may take a moment, but your `README.txt` file should now be
    uploaded to your `tutorial_folder` on the Data Store; you may
    need to refresh your web browser to see the update.

------------------------------------------------------------------------

## Output/Results

| Location | File | Example |
|--------|-------------|---------|
| On CyVerse | `README.txt` | View the [example folder](https://datacommons.cyverse.org/browse/iplant/home/shared/cyverse_training/cyverse_mooc){target=_blank} |
| On your Computer | `DE_sample_plants.fas` | ||                      

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
     [CyVerse Learning Center](https://learning.cyverse.org)
  - Ask us for help:
    click the Intercom icon ![Intercom](assets/intercom.png){ width="25" } on the lower right-hand side of the page
  - Report an issue or submit a change:
    [Github Repo Link](https://github.com/cyverse-learning-materials/)
  - Send feedback: <Tutorials@CyVerse.org>
  
------------------------------------------------------------------------

[:material-rocket: Learning Center Home](http://learning.cyverse.org/)