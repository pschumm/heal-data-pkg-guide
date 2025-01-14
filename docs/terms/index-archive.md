## Tabular data file
A data file that is organized in a table with rows and columns.

## Multi-result file
A file that contains multiple results from your study. Some examples of multi-results files include manuscripts, posters, and presentations.

## Study resources
All data and non-data supporting files/documents/resources generated by and associated with your study, regardless of whether you are planning to share them.

## Standard data package metadata files

<div markdown="1" style="background-color:rgba(0, 0, 0, 0.0470588); text-align:left; vertical-align: top; padding:10px 10px;">

Standard metadata file types that, altogether, provide essential usability and context information about the study as a whole and about the data files your study has produced/collected. These metadata files should be included in all data packages. 

**NOTE**: All standard data package metadata files have a standardized csv format in which they should be completed and provided. See here for [csv templates] and [field definitions] to aid you in completing the templates. 



### Standard data package metadata - Study-level 


* #### **Experiment Tracker**
     one per study; an inventory of experiments or activities included in the study; for a clinical trial, this may be simply one experiment equal to the registered clinical trial activity; for a basic biology study, this may be a listing of several orthogonal experiments used altogether to address and advance the study aims, 
* #### **Resource Tracker**
     one per study; an inventory of all data and non-data supporting files produced during the course of the study (or, in some cases, only those which will be shared in a public data repository), including a description of what is in the file or what the file represents, file relationships and dependencies, and whether/how each file is shareable in a public repository or not  

### Standard data package metadata - File-level 

* #### **Data Dictionary**
     one per tabular data file; an inventory of variables included in a tabular data file 
* #### **Results Tracker**
     one per multi-result file (e.g. manuscript); an inventory of figure, table, and text results included in a multi-result file 

</div>

## Experiment Tracker
The experiment tracker provides contextual information on the experiments that are involved in the study. Complete one per study.

The tracker is a csv file, where each row of the experiment tracker corresponds to one component experiment or activity included in the study. Information about the experiment includes research questions(s), approach, and hypotheses.

For detailed information on the name and definition of each field in the experiment tracker, please refer to the [experiment tracker schema].

**NOTE**: For a clinical trial, this may be simply a listing of one experiment equal to the registered clinical trial activity; For a basic biology study, this may be a listing of several orthogonal experiments used altogether to address and advance the study aims. 

## Study-level Metadata: Resource Tracker
The resource tracker is an inventory and annotate list of all data and supporting/non-date files for the study. Each row of the resource tracker corresponds to one data or non-data resource. Informaiton in the tracker about each resource includes file path, description, access restrictions, format, corresponding software, and dependencies. The resource tracker is where you will also list and annotate any associated any associated results trackers docummenting multi-result files.

See [Resource Tracker: Associated Files/Dependencies] for more information on how you should document your dependencies, depending on the type and amount of data you are sharing.

For detailed information on the name and definition of each field in the resource tracker, please refer to the [resource tracker schema].

## File-level Metadata: Data Dictionary

## File-level Metadata: Results Tracker
The results tracker provides detailed information and annotation for multi-result files (e.g., manuscript, presentation). Each multi-result file will have a corresponding results tracker. The purpose of this tracker is to track and annotate each single result (e.g., a figure or textual statement) within each multiresult file as well as all the data and supporting files upon which each single result depends. Within the results tracker, each row corresponds to one result from the multi-result file. Information about each result includes type of result (figure or text), description, and supported claims. 

!!! note
    Each results tracker should be additionally listed and annotated as its own row in the resource tracker.

For detailed information on the name and defiition of each field in the results tracker, please refer to the [results tracker schema].

## Wholistic annotation of study artefacts
Wholistic annotation involves creating and maintaining documentation that catalogues and annotates all files and non-data/supporting documents generated by and associated with your study regardless of whether you are planning to share them. Files that will not be shared are documented as permanent-private. This type of annotation works best paired with ['add as you go' annotation], as it easier an less time consuming to annotate wholistically, retrospectively, as part of ['top-down' annotation].

Although this mode of annotation is more time consuming, it maximizes transparency and allows investigators interested in the data to understand the full scope of the project when accessing study documentation on the Platform. This structure also allows for documentation of the existence and disposition of files that are too sensitive to share but are important for reproducibility and can perhaps be requested directly from the study team by an investigator.

<details>
<summary> Who may choose to share this way</summary>
    <ul>
    <li> Study groups that have not started collecting data or are very early in the data collection process.</li> 
    <li> Study groups that are earlier in the process and are interested in understanding and implementing a file and folder structure that facilitates data sharing in the future.</li>
    <li> Study groups that want to maximise the amount of information that they share about their study.</li>

</details>

<details>
<summary> Pros to sharing this way</summary>
    <ul>
    <li> You get the benefit of full local annotation, which not only maximizes the usefulness of your data for other investigators but also can be helpful internally, especially in preserving knowledge about the data even as team members may change over the course of the study.</li>
    <li> Although more time consuming at the beginning, integration of this process into your workflows allows for documentation and annotation in parts as you move through the study, so that you do not need to compile all that information at the end of the study, retrospectively.</li>
    <li> Documenting and sharing all metadata associated with your study can increase the discoverability of your study.</li>

</details>

<details>
<summary> Cons to sharing this way</summary>
    <ul>
    <li> More time consuming, because it requires you to set up the structures to fully catalogue all data and non-data/supporting files that are relevant to your study.</li>

</details>

**Notes about wholistic annotation**

If you are early in your study and choose to pursue wholistic annotation, we recommend you consider reviewing and implementing [HEAL recommendations for organizing and naming of study artefacts]. This will ease the process of annotation as well as future data sharing.

If you are annotating wholistically, you will also document dependencies 'one-layer-deep'. For more information, see [Resource Tracker: Associated Files/Dependencies] and ['One Layer Deep' Dependencies].


## Minimal annotation of study artefacts
Minimal annotation starts with the main file you are focused on sharing, whether that is a multi-result file, such as a publication or presentation, or a dataset, and works backwards. Rather than documenting all files, you document only the data and non-data file dependencies required to reproduce the final results or dataset. This is likely more ideal for studies that may be close to data collection completion and are not focused on meeting data sharing requirements but do not have adequate funding or time to devote the complete documentation of the data. This type of annotation pairs well with ‘top-down’ annotation, which retrospectively annotates study artefacts.

<details>
<summary> Who may choose to share this way</summary>
    <ul>
    <li> Study groups that may be finished or close to finished collecting data and have already produced results files (e.g., figures, draft publications/NIH reports, etc.) </li>
    <li> Study groups that want to meet minimal data sharing requirements of sharing data underlying published results</li>
</details>

<details>
<summary> Pros to sharing this way</summary>
    <ul>
    <li> You only catalog the data and non-data/supporting files that you will share/submit to a repository.</li>
    <li> This is less work than fully cataloguing all data and non-data/supporting files relevant to a study (including files you will not share/submit to a repository), especially if the study is well underway or complete/nearing completion and/or does not have resources or time set aside for a complete file inventory.</li>
    <li>This approach allows you to fulfill the minimal data sharing requirements of sharing data underlying published results.</li>
</details>

<details>
<summary> Cons to sharing this way</summary>
    <ul>
    <li> You don’t get the full local annotation benefit that would come with fully cataloguing all data and non-data/supporting files relevant to a study (including files you will not share/submit to a repository), and how they relate to each other and to published results – these benefits include <i>facilitating continuity and passed-down knowledge within study groups</i>, and discovery, sharing, and re-use of the data and knowledge produced by the study outside of the original study group.</li>
    <li>You don’t get the full benefit of the added discoverability that data-package level metadata can provide.</li>
</details>


**Notes about minimal annotation**

Even if you are not early in your study and are pursuing minimal annotation, we do not recommend reorganizing all your files or folder structures. However, we do recommend you consider reviewing and implementing naming conventions for like files, detailed in [HEAL recommendations for organizing and naming study artefacts]. This will ease the process of annotation.

If you are annotating minimally, you will document dependences 'liberally'. For more information, see [Resource Tracker: Associated Files/Dependencies] adn ['Liberal' Dependencies].

