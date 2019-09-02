---
title: "Using the SharePoint Migration Tool Reports"
ms.reviewer: 
ms.author: jhendr
author: JoanneHendrickson
manager: pamgreen
audience: ITPro
ms.topic: article
ms.prod: sharepoint-server-itpro
localization_priority: Normal
mscollection:
- SPMigration
- M365-collaboration
search.appverid: MET150
---

# Using the SharePoint Migration Tool Reports


The SharePoint Migration Tool generates log files, summary and task level reports to help you manage, audit and troubleshoot your migration process.
  
## How to view the reports

These reports can be viewed while the migration is taking place or after the jobs are complete.
  
 **Viewing task level reports:**
  
1. After the migration has begun, click **View reports**.
    
2. A file folder will open listing the task level reports that have been generated for that specific task.
    
 **Viewing summary reports:**
  
1. After migration completes, click **Migration details**.
     
2. A folder with the summary reports opens.
    
## Summary Reports

Two types of summary reports are generated. The second type of summary report generated only if there is failures.
  
- **SummaryReport.csv.** This report contains a single row of data that gives the total picture total size, number of files migrated, duration. 
    
- **FailureSummary.csv.** This report is created only when failures or errors happen during the migration process. 
    
When assessing your migration jobs, we recommend that you first look at these summary reports. If a FailureSummary.csv file was not created, then no failures occurred during the job run.
  
### Summary Report

|**Column**|**Description**|
|:-----|:-----|
|Source  <br/> |File path or URL of the location of the data being migrated.  <br/> |
|Destination  <br/> |The URL of the Site and library to where the data will be migrated.  <br/> |
|Status  <br/> |Status of each task (success, failure, in progress, not started)  <br/> |
|Total bytes  <br/> |Total number of bytes scanned in source destination..  <br/> |
|Total GB  <br/> |Total number of gigabytes scanned in source destination.  <br/> |
|Count of files  <br/> |Total number of scanned items  <br/> |
|Migrated bytes  <br/> |The total number of bytes of data migrated.  <br/> |
|Migrated GB in current round  <br/> |The total size of the files migrated, expressed in gigabytes.  <br/> |
|GB not migrated in current round  <br/> |The total size of the files not migrated, expressed in gigabytes.  <br/> |
|Total scanned items  <br/> |Total number of files and list items, including those that will be filtered out because of settings or potential scan issues.  <br/> |
|Total to be migrated in current round  <br/> |The total number of files that were expected to migrate excluding those filtered out based on settings or potential scan issues.  <br/> |
|Migrated items in current round  <br/> |The total number of files migrated.  <br/> |
|Items not migrated in current round  <br/> |Number of files that did not migrate.  <br/> |
|Warning count in current round  <br/> |Number of warnings generated.  <br/> |
|Start time  <br/> |The time the migration task began.  <br/> |
|End time  <br/> |The time the migration task ended.  <br/> |
|Duration  <br/> |Length of time in minutes that the migration task took to complete.  <br/> |
|GB/hour  <br/> |How many GB per migrated per hour.  <br/> |
|Round number  <br/> |The round number is the incremental number of times the report has been generated based on the multiple passes the tool made to get all the content it could into the destination.  <br/> |
|Workflow ID  <br/> |The ID number of the migration workflow. Many tasks can be in a single workflow.  <br/> |
|Task ID  <br/> |The individual task number.  <br/> |
|Log Path  <br/> |The location of the log files for each task.  <br/> |
   
### Failure Summary Report

This report is only generated if a failure occurs during the job run.
  
|**Column**|**Description**|
|:-----|:-----|
|Source  <br/> |File path or URL of the location of the data being migrated.  <br/> |
|Destination  <br/> |The URL of the Site and library to where the data will be migrated.  <br/> |
|File name  <br/> |Failed file or folder name or list items  <br/> |
|Extension  <br/> |If it is a folder, then the extension is empty, else if it is a file, then extension is file extension.  <br/> |
|File size  <br/> |Failed file or folder size or item size  <br/> |
|Content type  <br/> |Folder or file.  <br/> |
|Status  <br/> |Status of the file or folder that shows as "Failed" in this report.  <br/> |
|Result category  <br/> |Failed reason category based on the job process.  <br/> |
|Message  <br/> |Failed reason detail description.  <br/> |
|Error code  <br/> |Failed reason errorcode.  <br/> |
|Package number  <br/> |The package number for the package includes the failed item .  <br/> |
|Migration job ID  <br/> |The job id for the package includes the failed item.  <br/> |
|Incremental round  <br/> |The last incremental round number that item failed.  <br/> |
|Task ID  <br/> |The individual task number.  <br/> |
|Device name  <br/> |The name of the device or computer that is running the migration job.  <br/> |
   
## Task Reports

When you need to do deeper investigation or a thorough verification of your migration task, the task level reports help you drill down into the specific details. The four recommended task level reports to use are:
  
- **FileSummary.csv:** This is similar to the overall summary report except that it aggregates the data just for a single task. 
    
- **FilesFailureReport.csv:** This is the failure report at the item level. This is a filtered version of the filese report, showing only failures. 
    
- **FilesReport.csv:**  A list of all the items this task attempted to do 
    
- **ScanSummary.csv:** This report gives statistical totals. 
    
- **StructureReport.csv:**  Structure report at the task level.
    
- **StructureFailureReport.csv:**  Structure failure report at the task level.
    
- **StructureFailureSummary.csv:**  This is an aggregate of all the structural task failure reports. This will only be generated if there are failures.
    
### Files Summary

The **FilesSummary.csv** report is a summary report at the task level. 
  
|**Column**|**Description**|
|:-----|:-----|
|Incremental round  <br/> |The round number added to the end of the report name (RO, R1, etc.) indicates if the scan or job has been rerun.  <br/> |
|Scanned  <br/> |Total number of files scanned before migration.  <br/> |
|Item scan failures  <br/> |Number of files that failed the scan and doesn't qualify for the migration.  <br/> |
|Filtered out items  <br/> |Number of files not included in migration.  <br/> |
|Expected migrated file count  <br/> |The total number of files that were expected to migrate excluding those filtered out based settings or scanned potential issues. The total number of files that were expected to migrate.  <br/> |
|Read  <br/> |Total number of files read.  <br/> |
|Packaged  <br/> |Total number of files packaged and ready to upload to the destination.  <br/> |
|Uploaded  <br/> |Total number of files attempted to upload.  <br/> |
|ReUploaded  <br/> |The total number of files that were re-uploaded.  <br/> |
|Submitted  <br/> |Total number of files submitted.  <br/> |
|ReSubmitted  <br/> |Total number of files resubmitted.  <br/> |
|Migrated  <br/> |Total number of files migrated.  <br/> |
|Failed reading  <br/> |Number of files that encountered an error or failure while being read.  <br/> |
|Failed packing  <br/> |Number of files that encountered an error or failure while being packaged.  <br/> |
|Failed uploading  <br/> |Number of files that encountered an error or failure while being uploaded.  <br/> |
|Failed submitting  <br/> |Number of files that encountered an error or failure while being submitted.  <br/> |
|Failed querying  <br/> |Number of files that encountered an error or failure while being queried.  <br/> |
|Device name  <br/> |Name of the device or computer that is running the migration job.  <br/> |
   
### File Failure Report

The **FilesFailureReport.csv**, is only generated if an error resulting in a file being unable or failing to migrate. 
  
|**Column**|**Description**|
|:-----|:-----|
|Source  <br/> |File path or URL of the location of the data being migrated.  <br/> |
|Destination  <br/> |the URL of the tenant and library to where the data will be migrated.  <br/> |
|Item name  <br/> |The name of the file migrated.  <br/> |
|Extension  <br/> |The extension, indicating the file type.  <br/> |
|Item size  <br/> |The size of the individual file.  <br/> |
|Content type  <br/> |The file type.  <br/> |
|Status  <br/> |Status indicating at what stage the file is.  <br/> |
|Result category  <br/> |General code associated with the item to indicate what happened with that item.  <br/> |
|Message  <br/> |Detailed error or informational message .  <br/> |
|Error code  <br/> |Failed reason error code.  <br/> |
|Source item ID  <br/> |ID of the item at the source.  <br/> |
|Destination item ID  <br/> |ID ofthe item at the destination.  <br/> |
|Package number  <br/> |ID generated for the package number during the transition.  <br/> |
|Migration job ID  <br/> |The ID number of the job (which could contain one or more tasks).  <br/> |
|Incremental Round  <br/> |The round number added to the end of the report name (RO, R1, etc.) indicates if the scan or job has been rerun.  <br/> |
|Task ID  <br/> |The ID number of the Task.  <br/> |
|Device name  <br/> |Name of the device or computer that is running the migration job.  <br/> |
   
### Files Report

The **FilesReport.csv** is a detailed report that provides data on each file within the task. 
  
|**Column**|**Description**|
|:-----|:-----|
|Source  <br/> |File path or URL of the location of the data being migrated.  <br/> |
|Destination  <br/> |the URL of the tenant and library to where the data will be migrated.  <br/> |
|File name  <br/> |The name of the file migrated.  <br/> |
|Extension  <br/> |The extension, indicating the file type.  <br/> |
|File size  <br/> |The size of the individual file.  <br/> |
|Content type  <br/> |The file type.  <br/> |
|Status  <br/> |Status indicating at what stage the file is.  <br/> |
|Result category  <br/> |General code associated with the item to indicate what happened with that item.  <br/> |
|Message  <br/> |more detailed Error or informational message generated.  <br/> |
|Source item ID  <br/> |ID of the item at the source.  <br/> |
|Destination item ID  <br/> |ID ofthe item at the destination.  <br/> |
|Package number  <br/> |ID generated for the package number during the transition.  <br/> |
|Migration job ID  <br/> |The ID number of the job (which could contain one or more tasks).  <br/> |
|Incremental round  <br/> |The round number added to the end of the report name (RO, R1, etc.) indicates if the scan or job has been rerun.  <br/> |
|Task ID  <br/> |The ID number of the Task.  <br/> |
|Device name  <br/> |Name of the device or computer that is running the migration job.  <br/> |
   
### Scan Summary

The **ScanSummary.csv** report provides the total stats for the scan -- a process that takes place before the actual migration begins. 
  
|**Column**|**Description**|
|:-----|:-----|
|Incremental round  <br/> |The round number added to the end of the report name (RO, R1, etc.) indicates if the scan or job has been rerun.  <br/> |
|Total scanned items  <br/> |Total number of folders, list items and files that have been scanned.  <br/> |
|Total scanned folders  <br/> |Total number of folders scanned.  <br/> |
|Total scanned list items  <br/> |Total number of list items scanned.  <br/> |
|Total scanned files  <br/> |Total number of files scanned.  <br/> |
|Folders with issues  <br/> |The number of folders with potential issues for the migration.  <br/> |
|Items with issues  <br/> |The number of files with potential issues for migration.  <br/> |
|Items filtered out  <br/> |Number of files that where filtered out based on settings in the tool.  <br/> |
|Folders to be migrated  <br/> |Number of folders that will be migrated.  <br/> |
|Items to be migrated  <br/> |Number of files that will be migrated.  <br/> |
|Total items to be migrated  <br/> |Total number of folder and files that will be migrated.  <br/> |
|Device name  <br/> |Name of the device or computer that is running the migration job.  <br/> |
   
### Structure report

Structure report at the task level.
  
|**Column**|**Description**|
|:-----|:-----|
|Structure type  <br/> |Site collection, site, list, field, content type, view  <br/> |
|Structure title  <br/> |Display name of the object  <br/> |
|Operation  <br/> |Skipped, created or updated.  <br/> |
|Status  <br/> |Success, partial success, failure  <br/> |
|Details  <br/> |Reason for failure.  <br/> |
|Source structure URL  <br/> |Display the source URL. Site collection, site, and list will list the URL. Fields, content type. and view will display its container's URL.  <br/> |
|Destination structure URL  <br/> |Display the source URL. Site collection, site, and list will list the URL. Fields, content type, and view will display its container's URL.  <br/> |
|Source structure ID  <br/> |ID when available.  <br/> |
|Destination structure ID  <br/> |ID when available.  <br/> |
|Time stamp  <br/> |The time at which the action occurred.  <br/> |
   
### Structure failure report

This is a failure report at the task level. This report will only be generated if there is a failure.
  
|**Column**|**Description**|
|:-----|:-----|
|Structure type  <br/> |Site collection, site, list, field, content type, view  <br/> |
|Structure title  <br/> |Display name of the object  <br/> |
|Operation  <br/> |Skipped, created or updated.  <br/> |
|Status  <br/> |Success, partial success, failure  <br/> |
|Details  <br/> |Reason for failure.  <br/> |
|Source structure URL  <br/> |Display the source URL. Site collection, site, and list will list the URL. Fields, content type. and view will display its container's URL.  <br/> |
|Destination structure URL  <br/> |Display the source URL. Site collection, site, and list will list the URL. Fields, content type, and view will display its container's URL.  <br/> |
|Source structure ID  <br/> |ID when available.  <br/> |
|Destination structure ID  <br/> |ID when available.  <br/> |
|Time stamp  <br/> |The time at which the action occurred.  <br/> |
   
### Structure failure summary

This is an aggregate of all the task failure reports. This will only be generated if there are failures.
  
|**Column**|**Description**|
|:-----|:-----|
|Structure type  <br/> |Site collection, site, list, field, content type, view  <br/> |
|Structure title  <br/> |Display name of the object  <br/> |
|Operation  <br/> |Skipped, created or updated.  <br/> |
|Status  <br/> |Success, partial success, failure  <br/> |
|Details  <br/> |Reason for failure.  <br/> |
|Source structure URL  <br/> |Display the source URL. Site collection, site, and list will list the URL. Fields, content type. and view will display its container's URL.  <br/> |
|Destination structure URL  <br/> |Display the source URL. Site collection, site, and list will list the URL. Fields, content type, and view will display its container's URL.  <br/> |
|Source structure ID  <br/> |ID when available.  <br/> |
|Destination structure ID  <br/> |ID when available.  <br/> |
|Time stamp  <br/> |The time at which the action occurred.  <br/> |
   

