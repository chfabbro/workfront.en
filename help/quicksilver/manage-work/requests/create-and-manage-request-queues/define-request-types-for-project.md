---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Define Request Types for a project
description: You can organize the kind of issues or requests that are logged in Adobe Workfront by Request Types.
author: Alina
feature: Work Management
---

# Define Request Types for a project

You can organize the kind&nbsp;of issues or requests that are logged in Adobe Workfront by Request Types.

This organization is useful for reporting reasons and for helping users understand what kind&nbsp;of unexpected work&nbsp;might occur during the lifetime of a project.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront license</a>*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must

* Have or create a project

  For information about creating projects, see [Create a project](../../../manage-work/projects/create-projects/create-project.md).

## Considerations about Request Types

* You can specify the&nbsp;type of issues or requests that can be logged on a project when you configure the **Queue Details**&nbsp;area for the project.
* You don't have to enable the project to be a request queue to be able to define Request&nbsp;Types for a project. Any issues logged for a project can be labeled with a different Request&nbsp;Type. 
* If you add Queue Topics to your project, you must define Request&nbsp;Types on each queue topic to display it when adding a new issue or request. For more information, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Define the issue or request types for a project

1. Click **Projects** in the Main Menu. ![](assets/main-menu-icon.png)

1. Click the name of the project to open it.
1. In the left panel, click **Queue Details**. 
1. In the **Queue Properties** section, select the **Request Types** you want for the project.

   >[!NOTE]
   >
   >You must have at least one request type selected. You can select multiple request types.

   Select from the following types:

   * Bug Report
   * Change Order
   * Issue
   * Request

   >[!TIP]
   >
   >Your Workfront administrator might have renamed some of these options. For information, see [Configure request types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Click **Save**.

   The request types you specified&nbsp;will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project, if the project is enabled as a request queue.

