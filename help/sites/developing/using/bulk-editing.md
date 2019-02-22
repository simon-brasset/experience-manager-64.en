---
title: Configuring your Page for Bulk Editing of Page Properties
seo-title: Configuring your Page for Bulk Editing of Page Properties
description: Bulk editing of page properties allows you to edit the properties of multiple pages at once
seo-description: Bulk editing of page properties allows you to edit the properties of multiple pages at once
uuid: c179d4fc-becd-4519-84af-e1dc8fb9bb69
contentOwner: User
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: extending-aem
content-type: reference
discoiquuid: 0ba98cef-9782-441f-a1c4-1e10f88894e4
index: y
internal: n
snippet: y
---

# Configuring your Page for Bulk Editing of Page Properties{#configuring-your-page-for-bulk-editing-of-page-properties}

[Bulk editing of page properties](../../../sites/authoring/using/editing-page-properties.md#fromthesitesconsolemultiplepages) allows you to edit the properties of multiple pages at once.

Due to the possibility of different values, page properties are not enabled for bulk editing as default. They must be explicitily whitelisted (enabled). When defining the page properties to be available for bulk editing you need to consider certain implications, such as:

* Certain fields are usually unique; for example a page title. You must decide whether it is meaningful to enable such fields for bulk editing, when one value will be applied.  
* Certain fields might have multiple values - this needs meaningful representation when rendering.  
  For example, a check-box indicating "Ready for Publication". This might have several values before bulk-editing (e.g. ready, in-review, in-progress).

>[!CAUTION]
>
>Bulk editing of page properties is:
>
>* Not available in the classic UI.
>* Not available for pages within a live copy.
>* Only available for pages with the same resource type. 
>

>[!NOTE]
>
>Bulk editing is also available for Assets. It is very similar, but differs in a few points. See [Editing Properties of Multiple Assets](../../../assets/using/managing-multiple-assets.md) for full information. You can customize the fields in the Bulk Metadata editor for Assets using the [Schema editor](../../../assets/using/metadata-schemas.md).

### Enabling a Field {#enabling-a-field}

>[!NOTE]
>
>Certain fields might have multiple values - this needs meaningful representation when rendering. For this reason you should only enable the following field types: 
>
>* `/libs/granite/ui/components/foundation/form/textfield`
>* `/libs/granite/ui/components/foundation/form/textarea`
>* `/libs/granite/ui/components/foundation/form/tagspicker`
>* `/libs/granite/ui/components/foundation/form/datepicker`
>* `/libs/granite/ui/components/foundation/form/pathbrowser`
>* `/libs/granite/ui/components/foundation/form/checkbox`
>

Fields are enabled on the page component (*not* on the template):

1. Using CRXDE Lite (or an equivalent method) open your page component.

   For example: `/apps/core/wcm/components/page/v1/page`

   >[!NOTE]
   >
   >This example assumes that the Core Components have been installed on the instance, which is the case if the instance is running with We.Retail sample content. See the [Core Components documentation](/content/help/en/experience-manager/core-components/user-guide) for more information.

1. Navigate to the required field within the `cq:dialog` definition.
1. Define the following property on the field node:

    * **Name**: `allowBulkEdit`  
    
    * **Type**: `Boolean`  
    
    * **Value**: `true`

   For example, for the standard page [foundation component](../../../sites/authoring/using/default-components-foundation.md):

   The property would be defined on:

   >[!CAUTION]
   >
   >You ***must*** not change anything in the `/libs` path.
   >
   >
   >This is because the content of `/libs` is overwritten the next time you upgrade your instance (and may well be overwritten when you apply either a hotfix or feature pack).
   >
   >
   >The recommended method for configuration and other changes is:
   >
   >    
   >    
   >    1. Recreate the required item (i.e. as it exists in `/libs`) under `/apps`  
   >    
   >    1. Make any changes within `/apps`
   >    
   >

1. Select **Save All** to persist your updates.
