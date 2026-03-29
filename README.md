# KunalMavenAnalyticsDataPlayground

## Data Table

|Name|Key|Data Type|Notes|
|--|--|--|--|
|Name|name|string||
|Description|description|string||
|File Types|fileTypes|string[]||
|Tags|tags|string[]||
|Data Structure|dataStructure|string||
|# of Records|numRecords|number||
|# of Fields|numFields|number||
|Date Added|dateAdded|string||
|Download Link|downloadLink|string||
|Analysis Completed?|analysisCompleted|boolean||
|Logo|logo|string||
|Github Link|githubLink|string||
|NbViewer Link|nbviewerLink|string|This could be programmatically created|

## Data Model

```
// Jupyter Analysis Data Model
export interface jupyterAnalysis {
    name: string;
    description: string;
    fileTypes: string[];
    tags: string[];
    dataStructure: string;
    numRecords: number;
    numFields: number;
    dateAdded: string;
    downloadLink: string;
    analysisCompleted: boolean;
    logo: string;
    githubLink: string;
}

// Jupyter Analysis View Model
export interface jupyterAnalysisView extends jupyterAnalysis {
    nbViewerLink: string;
}
```