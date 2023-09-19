[de]: assets/de/logos/deIcon.svg
[home]: assets/de/menu_items/homeIcon.svg
[data]: assets/de/menu_items/dataIcon.svg
[apps]: assets/de/menu_items/appsIcon.svg
[analysis]: assets/de/menu_items/analysisIcon.svg
[shell]: assets/de/menu_items/webshellIcon.svg
[team]: assets/de/menu_items/teamsIcon.svg
[bank]: assets/de/menu_items/bank.svg
[help]: assets/de/menu_items/helpIcon.svg

# Data Management III

!!! tip "Learning Objectives"

    - Apply metadata in the Discovery Environment interface
    - Share data with other CyVerse users

**Description:**

In this module, we introduce how to apply metadata in the Discovery Environment and demonstrate how to share data with other CyVerse users.

---
> <div class="video-container">
> <iframe width="560" height="315" src="https://www.youtube.com/embed/shqShSoTOW8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
> </div>

------------------------------------------------------------------------

## Input Data:

| Location | Files | Example |
|--------|-------------|---------|
| On CyVerse | `README.md` `ept2copc.json` | View the [example folder](https://data.cyverse.org/dav-anon/iplant/home/shared/usda/usfs/r3/coconino/training_data/mahan/){target=_blank} |                    

---------------------------------------------------------------

## Editing Metadata on Single Files in the Discovery Environment

1.  If necessary, log into the CyVerse .
2.  Click the (Data Icon) to browse your collection of files in the CyVerse Data Store.
3.  Navigate to the `raw_data` folder inside `tutorial_folder` and select (checkbox) the `ept2copc.json` file uploaded previously.
4.  Under the **More Actions** menu, click on the **Metadata** choice.

You will see existing metadata for the file/folder in the Attribute, Value, Unit (AVU) format.

### Adding metadata

1.  Click the "+ Add Metadata" button to add a new entry. Then follow the directions for editing metadata below.

### Editing or deleting metadata

1.  Use the "pencil" icon to edit an existing entry or the "trash can" icon to delete an entry.
2.  After you have made any edits or deletion, click 'Save' (on the top right of the screen) to save all entries and apply the metadata.

### Apply metadata on multiple files in the Discovery Environment

It is possible to add or edit metadata on multiple files in the Discovery Environment by uploading a spreadsheet with this metadata. 

The spreadsheet can be designed to follow a metadata format or standard, or contain whatever metadata entries you want associated with a set of files. See the for more details.

## Output/Results

Although the file itself has not been edited, viewing the metadata in the Discovery Environment lets you view all annotations you have made to the file. View with metadata applied (you will need to view the file in the Discovery Environment to view the associated metadata; select the file and click **More Actions** and then **Metadata**).

## Data Sharing in the Discovery Environment

1.  If necessary, log into the [![][de]{width=25}](https://de.cyverse.org){target=_blank} [Discovery Environment](https://de.cyverse.org){target=_blank}.
2.  Click the [![][data]{width=25}](https://de.cyverse.org/data/){target=_blank} [Data Icon](https://de.cyverse.org/data){target=_blank} to browse your collection of files in the CyVerse Data Store.
3.  Navigate to the `tutorial_folder/` created previously and select (checkbox) the folder. Click the **Share** button.
4.  In the 'search for users' field search for the CyVerse user you wish to share with by searching for their username or email address.
5.  Next, under 'Permissions' choose what permission you want to grant the person you are sharing this file with.
6.  Once you are finished, click Done to begin sharing. The user will be notified that a file has been shared with them.

!!! Tip "See more on in the [Data Store Guide](https://learning.cyverse.org/ds/share/#share-a-filefolder-in-the-discovery-environment-with-another-cyverse-user-or-group){target=_blank}."

------------------------------------------------------------------------

### Self Assessment Questions

??? Question "Use the `README.md` file from [Data Management I](step4.md) and apply the metadata correctly to your file using the DE"

    ??? Success "Answer"

        Click to see how it should look and compare your results; click the **More Actions** menu, then **Metadata**.

??? Question "Which of the following are true about metadata in the CyVerse Data Store?"

    **A**  Are structured in Attribute-Value-Unit in CyVerse

    **B**  Contain information about the corresponding data file

    **C** Are discoverable in CyVerse through ElasticSearch

    **D**  Contain results of experiments

    ??? Success "Answer"
      
        Correct answer are **A, B, & C**.


??? Question "Select the correct statement: Sharing of research data in CyVerse..."

    **A**  Will be sent to collaboration partners automatically
  
    **B**  Will transfer of ownership to a collaborator

    **C**  Enables cross-institutional collaboration

    **D**  Ensures that data stays in a single accessible location you control access to.

    ??? Success "Answer"

        Correct answer are **C & D**.

-----------------------------------------------------------------------

**Fix or improve this documentation**

  - Search for an answer:
     [CyVerse Learning Center](https://learning.cyverse.org){target=_blank}
  - Send feedback: <tutorials@cyverse.org>
  
------------------------------------------------------------------------

[:material-rocket: Learning Center Home](http://learning.cyverse.org/)
