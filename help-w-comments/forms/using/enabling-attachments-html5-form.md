---
title: Enabling attachments for an HTML5 form
seo-title: Enabling attachments for an HTML5 form
description: By default, the attachment support for HTML5 forms is disabled.
seo-description: By default, the attachment support for HTML5 forms is disabled.
uuid: 3ea14f67-272b-48e2-8602-46c7042cb586
content-type: reference
products: SG_EXPERIENCEMANAGER/6.4/FORMS
topic-tags: hTML5_forms
discoiquuid: 9b877c6f-0632-4162-a146-fe81a804cb99
index: y
internal: n
snippet: y
---

# Enabling attachments for an HTML5 form{#enabling-attachments-for-an-html-form}

You can upload, preview, and submit attachments with HTML5 forms. By default, the attachment support is disabled. To enable the attachment support:

1. Create a [custom profile](../../forms/using/custom-profile.md) with mutiselect string property `mfAttachmentOptions`.
1. In the custom profile, specify properties `fileSizeLimit`, `multiSelect`, and `buttonTex`t to configure options of the file attachment widget. As required, you can also specify more custom properties.   

1. In the custom profile, use the following configurations:

    * **multiSelect **-&gt; true or false (true by default)
    * **fileSizeLimit **-&gt; value_in_mb (say 5) (2 MBs by default)
    * **buttonText **-&gt; Button text for pop-up window ("Attach" by default) 
    * **accept **-&gt; file types to accept ("audio/&#42;, video/&#42;, image/&#42;, text/&#42;, .pdf" by default)

   >[!NOTE]
   >
   >In Microsoft Internet Explorer 9, users can attach files larger than the specified limit. It is a known issue.

1. Use the [metadata editor](../../forms/using/manage-form-metadata.md) to select the custom profile that you have created above for HTML 5 forms. 
1. Render your form template with custom profile and the attachments icon would appear on the forms toolbar.

   >[!NOTE]
   >
   >Out of the box, the forms portal provides a custom profile with drafts and attachments capability enabled. For more information about the **Save as Draft **profile, see [Saving HTML5 forms as a draft](../../forms/using/saving-html5-form-draft.md).

1. Click the attachment icon, an attachment selection dialog box appears. Browse and select the attachment and click **Attach**.

   >[!NOTE]
   >
   >To preview an attachment, click the attachment name.

   >[!NOTE]
   >
   >The file preview option is not available for anonymous users.

## Attachment submission format {#attachment-submission-format}

When attachments are enabled, HTML5 form submits multipart data. The mutii-part submission data has two parts **dataXml **and** attachments. **

>[!NOTE]
>
>For backward compatibility, if `mfAllowAttachments`option is turned off, then the HTML5 forms does not send the muti- ``part data. It sends simple data xml in **application/xml **format.

If the mfAllowAttachments flag is turned on, the [submit service proxy service](../../forms/using/service-proxy.md) also posts multipart data with dataXml and attachments.