---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error message: SAML 2.0 error: Primary StatusCode"
description: You are unable to establish a successful connection to ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Error message: SAML 2.0 error: Primary StatusCode

## Problem

You are unable to establish a successful connection to ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>If you establish a successful test connection and you are still experiencing issues, you might have incorrect attribute mappings or issues with the federation IDs. Contact customer support with questions.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cause 1: Secure hash algorithm is set to SHA-256

### Solution

1. In Windows, click **Start** > **Administration** > **ADFS 2.0 Management**.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select **Trust Relationship** > **Relying Party Trusts** in the left-hand pane.

1. Right-click on the relying party trust related to Adobe Workfront, then select **Properties**.
1. Click on the **Advanced** tab, then select **SHA-1** from the **Secure hash algorithm** drop-down menu.  
   ![](assets/1-350x287.png)

## Cause 2: ADFS Signing Certificate is about to expire and has been replaced by a new Certificate with overlapping dates

### Solution

The Workfront SSO Setup Page lists the certificate expiration date. If the certificate is about to expire, you need to manually pull the New Signing Certificate from the ADFS Server:

1. In Windows, click **Start** > **Administration** > **ADFS 2.0 Management**.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select **Trust Relationship** > **Relying Party Trusts** in the left-hand pane.

1. Right-click on the relying party trust related to Workfront, and select **Properties**.
1. Click on the **Signature** tab.
1. Click on the name of the Signing Certificate, and click **View**.
1. Click Copy to **File**..., and select **Next**.

1. Select **Base-64 encoded x.509 (CER)**, and click **Next**.

1. Specify the file name, and click **Next**.
1. Click **Finish**.
1. In Workfront, navigate to **Setup** > **System** > **Single Sign-On (SSO)** and manually upload the Signing Certificate.

## Cause 3: Certificate revocation check is failing

The solution for this depends on the version of Microsoft ADFS that you are using. Consult Microsoft's documentation to obtain the appropriate commands for your version.
