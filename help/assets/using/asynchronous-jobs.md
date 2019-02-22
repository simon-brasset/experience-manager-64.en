---
title: Asynchronous Operations
seo-title: Asynchronous Operations
description: Overview of asynchronous operations in AEM Assets.
seo-description: Know about asynchronous operations in AEM Assets.
uuid: bb9fe4b9-ba2c-4e99-8c3a-546ea4fb1d8d
contentOwner: cmajumda
discoiquuid: e94320df-f1e4-4879-ba73-36b883ac04f0
index: y
internal: n
snippet: y
---

# Asynchronous Operations{#asynchronous-operations}

Overview of asynchronous operations in AEM Assets.

To reduce adverse impact on performance, Adobe Experience Manger (AEM) Assets processes certain long-running and resource-intensive asset operations asynchronously.

These operations include:

* Deleting many assets
* Moving many assets or assets with many references 
* Exporting/importing asset metadata in bulk.

Asynchronous processing involves enqueuing multiple jobs and eventually running them in a serial manner subject to the availability of system resources.

You can view the status of asynchronous jobs from the **Async Job Status** page.

>[!NOTE]
>
>By default, jobs in AEM Assets run in parallel. If N is the number of CPU cores, N/2 jobs can run in parallel, by default. To use custom settings for the job queue, modify the **Async Operation Default Queue** configuration from the web console. For more information, see [Queue Configurations](https://sling.apache.org/documentation/bundles/apache-sling-eventing-and-job-handling.html#queue-configurations).

## Monitoring the status of asynchronous operations {#monitoring-the-status-of-asynchronous-operations}

Whenever AEM Assets processes an operation asynchronously, you receive a notification at your inbox and through email.

To view the status of the asynchronous operations in detail, navigate to the **Async Job Status** page.

1. Tap/click the AEM logo, and go **Assets** &gt; **Jobs**.
1. In the **Async Job Status** page, review the details of the operations.

   ![](assets/job_status.png)

   To ascertain the progress of a particular operation, see the value in the **Status** column. Depending upon the progress, one of the following statuses is displayed:

   **Active**: The operation is being processed

   **Success**: The operation is complete

   **Fail**: The operation could not be processed

   **Scheduled**: The operation is scheduled for processing a later time

1. To stop an active operation, select it from the list and tap/click the **Stop** icon from the toolbar.

   ![](assets/stop_icon.png)

1. To view extra details, for example description and logs, select the operation and tap/click the **Open** icon from the toolbar.

   ![](assets/open_icon.png)

   The job details page is displayed.

   ![](assets/job_details.png)

1. To delete the operation from the list, select **Delete** from the toolbar. To download the details in a CSV file, tap/click the **Download** icon.

   >[!NOTE]
   >
   >You cannot delete a job if its status is either active or queued.

## Purging completed jobs {#purging-completed-jobs}

AEM Assets runs a purge job everyday at 1:00 AM to delete completed asynchronous jobs that are more than a day old.

You can modify the schedule for the purge job and the duration for which details of completed jobs are retained before they are deleted. You can also configure the maximum number of completed jobs for which details are retained at any point of time.

1. Tap/click the AEM logo, and go to **Tools** &gt; **Operations** &gt; **Web Console**.
1. Open the **Adobe CQ DAM Async Jobs Purge Scheduled** job.
1. Specify the threshold number of days after which completed jobs are deleted and the maximum number of jobs for which details are retained in history.

   ![](assets/purge_job.png)

1. Save the changes.

## Configuring thresholds for asynchronous processing {#configuring-thresholds-for-asynchronous-processing}

You can configure the threshold number of assets or references for AEM Assets to process a particular operation asynchronously.

### Configuring thresholds for asynchronous delete operations {#configuring-thresholds-for-asynchronous-delete-operations}

If the number of assets or folders to be deleted exceed the threshold number, the delete operation is performed asynchronously.

1. Tap/click the AEM logo, and go to **Tools** &gt; **Operations** &gt; **Web Console**.
1. From the web console, open the** Async Delete Operation Job Processing** configuration.
1. In the **Threshold number of assets** box, specify the threshold number of assets/folders for asynchronous processing of delete operations.

   ![](assets/delete_threshold.png)

1. Save the changes.

### Configuring thresholds for asynchronous move operations {#configuring-thresholds-for-asynchronous-move-operations}

If the number of assets/folders or references to be moved exceed the threshold number, the move operation is performed asynchronously.

1. Tap/click the AEM logo, and go to **Tools** &gt; **Operations** &gt; **Web Console**.
1. From the web console, open the** Async Move Operation Job Processing** configuration.
1. In the **Threshold number of assets/references** box, specify the threshold number of assets/folders or references for asynchronous processing of move operations.

   ![](assets/move_threshold.png)

1. Save the changes.
