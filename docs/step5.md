# Data Management II


!!! Tip "Learning Objectives"

    - Properly configure Cyberduck
    - Understand how Cyberduck works
    - Upload a dataset using Cyberduck to CyVerse

**Description:** In this module, we discuss how you can upload and download your dataset(s) in the Discovery Environment. This is done using Cyberduck, a 3rd party software that connects your local computer to the Data Store to enable drag-and-drop download and upload of data.

---
<div class="video-container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/RjvoF3i7zNE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
---

## Input Data

| Location | File | Example |
|--------|-------------|---------|
| On CyVerse | `README.txt` | View the [example folder](https://datacommons.cyverse.org/browse/iplant/home/shared/cyverse_training/cyverse_mooc){target=_blank} |
| On your Computer | `DE_sample_plants.fas` | ||                      

## Setting up Cyberduck

[bookmark]: assets/cyberduck/cyberduck_bookmark.png
[config]: assets/cyberduck/cyberduck_config.png
[window]: assets/cyberduck/cyberduck_window.png

1.  Download and install [CyberDuck](https://cyberduck.io){target=_blank} for your operating system.

2. Download the [CyVerse Cyberduck connection profile](https://cyverse.atlassian.net/wiki/download/attachments/241869843/CyVerseDataStore.cyberduckprofile?version=1&modificationDate=1568640173000&cacheVersion=1&api=v2) Double-click on the downloaded file (should be in your browser downloads)- this should open the now installed Cyberduck software.

3. In the Cyberduck configuration window, enter your CyVerse username in the field `iPlant username`.

4. Under **Advanced Options** ensure ‘Transfer Files’ option is set to ‘Open Multiple Connections’. Close this window - your entries will be automatically saved.

<figure markdown> 
  <a>![][config]{width=500}
    <figcaption>Username & multiple connections</figcaption>
  </a>
</figure>

Double-click on the Data Store bookmark in the window.

<figure markdown> 
  <a>![][bookmark]{width=500}
    <figcaption>Set the bookmark</figcaption>
  </a>
</figure>

You should now be connected to the Data Store and viewing the contents of your home directory.

<figure markdown> 
  <a>![][window]{width=500}
    <figcaption>your home path is: `/iplant/home/<username>`</figcaption>
  </a>
</figure>

## Upload data to the Data Store with CyberDuck

1.  Locate the `raw_data` folder inside your `tutorial_folder` in the Cyberduck display of your home
    directory.

2. Upload the file `DE_sample_plants.fas` to the `raw_data` folder inside the `tutorial_folder` by dragging and droping.

3. Back in the Discovery Environment, click the (Data Icon) to access your home folder.

4. Navigate to the `raw_data` folder inside your `tutorial_folder` in your browser to verify the upload was successful.

## Output/Results


| Location | File | Example |
|--------|-------------|---------|
| On CyVerse | `README.txt` & `DE_sample_plants.fas` | View the [example folder](https://datacommons.cyverse.org/browse/iplant/home/shared/cyverse_training/cyverse_mooc){target=_blank} |


------------------------------------------------------------------------

## Self Assessment Questions

??? Question "Why do you need Cyberduck?"

    **A** To conveniently chat with CyVerse support

    **B** To conveniently download and upload files from your local computer
    
    **C** To conveniently create teams on the Discovery Environment

    **D** To view apps and tools on the Discovery Environment

    ??? Success "Answer"
        
        Correst answer is **B**.


??? Question "Which of these will you need to configure and access the datastore using Cyberduck? Select all that apply:"

    **A**  SSH access

    **B**  CyVerse account

    **C**  CyVerse Cyberduck connection profile

    **D**  Discovery Environment

    ??? Success "Answer"

        Correct answer are **B & C**.

        Download the [CyVerse Cyberduck connection profile](https://cyverse.atlassian.net/wiki/download/attachments/241869843/CyVerseDataStore.cyberduckprofile?version=1&modificationDate=1568640173000&cacheVersion=1&api=v2) 

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