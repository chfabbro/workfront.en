---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: System project statuses
description: Workfront has 9 built-in system project statuses. The first 3 in the table below are required, which means that you can unlock, rename, and reorder them, but you cannot hide or delete them. Changing a project status is typically a manual process. However, sometimes a project status is changed automatically, depending on other factors that are happening in the system.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# System project statuses

Workfront has 9 built-in system project statuses.

The first 3 in the table below are required, which means that you can unlock, rename, and reorder them, but you cannot hide or delete them.

Changing a project status is typically a manual process. However, there are some scenarios outlined in the following list when a project status is changed automatically, depending on other factors that are happening in the system.

The following project statuses are provided with your Workfront instance:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>System project status</th> 
   <th>This project status occurs when</th> 
   <th>What happens in this status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planning (required status)</td> 
   <td> <p>The project manager is planning the timeline of the project, the assignment of the tasks, and the approvals. The project manager sets this status on a project manually.</p> <p>Tip: We recommend that you set the default status for new projects in Workfront to Planning. As a Workfront administrator, you can change the default status for all your new projects in the Projects area of Project Preferences.</p> </td> 
   <td> <p>Users on the project team can see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project do not populate their Work List. Only approvals and accepted work items display in the Home Work List.</p> <p>No notifications are sent while a project has this status.</p> <p>We recommend that all the changes that can trigger an update to the timeline of the project, or any changes to tasks and issue assignments, are made while the project is in the Planning status. This minimizes the amount of notifications users receive.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
  <tr> 
   <td>Current (required status)</td> 
   <td> <p>Users are working on it. The project manager should turn a project to Current to signal that it has started.</p> <p>This is the default status for new projects in Workfront.</p> <p>Tip: As a Workfront administrator, you can change the default status for new projects in the Projects area of Project Preferences. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
   <td> <p>Users on the project team can see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project populate their Work List. They can start accepting work on tasks and issues and move them to their Working On list.</p> <p>Also, on a Current project, all notifications about timeline changes, assignments, actions needed, and approvals are sent to users on the project team.</p> <p>And the timeline of the project is calculated automatically by the system, if the Update Type of the project is set to Automatic, On Change, or Automatic and On Change.</p> <p>Tip: It's a good idea to keep project plan adjustments to a minimum when a project is in this status so that users don't receive too many notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Complete (required status)</td> 
   <td> <p> The project is completed:</p> 
    <ul> 
     <li> <p>If the Completion Mode of the project is set to Manual, the project manager chooses this status manually to inform users on the project team to stop working on the project.</p> </li> 
    </ul> 
    <ul> 
     <li>If the Completion Mode of the project is set to Automatic, Workfront automatically marks a project as Complete when all the tasks and issues in the project are marked as Complete. </li> 
    </ul> <p><b>IMPORTANT</b>: You can mark a project as Complete only when all the tasks, issues, and approvals on the project are resolved.</p> </td> 
   <td>
    <ul>
     <li>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project do not populate their Work Requests or Working On lists.</li>
     <li>All the notifications related to the project, except for a status change notification, stop being sent to the users on the project team. </li>
     <li>The timeline of the project is not calculated anymore by the system.</li>
     <li>The project cannot be copied.</li>
    </ul><p>You can prevent users from performing additional actions when a project is marked as Complete. </p><p>For more information about how to restrict actions on projects that are marked as Complete, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Dead</td> 
   <td>The project has not finished yet, but due to roadblocks, or scope change, the project cannot continue to be worked on and has been abandoned. The project manager changes the status to Dead to alert the users on the project team that this project will never finish and they should not be working on it anymore.</td> 
   <td> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project disappear from their Work List.</p> <p>Approval decisions cannot be granted to tasks or issues.</p> <p>Notifications about timeline changes, assignments, actions needed, approvals are not sent to users on the project team.</p> <p>The timeline of the project is not calculated automatically by the system, as the project is perceived as being completed.</p> <p>You can prevent users from performing certain actions when a project is marked as Dead. For more information about how to restrict actions on Dead projects, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>On Hold</td> 
   <td>The project has not finished yet, but due to some delays, the project needs to be temporarily suspended. The project manager chooses to use this status to alert users in the project team to stop working on the project, at the current time.</td> 
   <td> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project disappear from their Work List. </p> <p>Approval decisions cannot be granted to tasks or issues.</p> <p>Notifications about timeline changes, assignments, actions needed, approvals are not sent to users on the project team.</p> <p> <p><b>NOTE</b>:  When you place a project On Hold, the timeline of the project does not stop. The project can still show as At Risk or In Trouble even if no one is actively working on the project. Some manual adjustments of the dates of the remaining open tasks might be needed when turning the project back to Current again, so that the project can show updated progress.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Requested</td> 
   <td>The project status is automatically marked as Requested by the system, when the business case on a project request has been completed and submitted for approval. For more information about requesting a project using a business case, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues on the project that are assigned to them do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
  <tr> 
   <td>Approved</td> 
   <td>The project status is automatically marked as Approved, when the business case on a project request has been approved. For more information about requesting a project using a business case, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td> <p>Users on the project team can see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system. </p> </td> 
  </tr> 
  <tr> 
   <td>Rejected</td> 
   <td>The project status is automatically marked as Rejected, when the business case on a project request has been rejected. For more information about requesting a project using a business case, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
  <tr> 
   <td>Idea</td> 
   <td>The project status is automatically marked as Idea when you submit a project request. For more information about requesting a project using a business case, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Review Requested Projects</a>.</td> 
   <td> <p>Users on the project team cannot see the project on their Projects lists by default, in the Projects area of Workfront. The tasks and issues that are assigned to them on the project do not populate their Work List.</p> <p>All the notifications related to the project, except for a status change notification are not sent to any users.</p> <p>The timeline of the project is not calculated automatically by the system.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The following project statuses cannot be changed to a Dead, On Hold, or Complete status:
>
>* Requested
>* Idea
>* Approved
>* Rejected (or its equivalent)
>

