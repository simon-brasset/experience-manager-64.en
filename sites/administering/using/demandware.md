---
title: Demandware
seo-title: Demandware
description: null
seo-description: Learn how to use AEM with Demandware.
uuid: c9152776-54b7-435a-b08f-09b1476315db
contentOwner: Guillaume Carlino
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: e-commerce
content-type: reference
discoiquuid: 77fba3c1-8d2e-4666-aca4-b802fcf637d7
disttype: dist5
gnavtheme: light
isreadyforlocalization: false
pagetitle: Administering Demandware
index: y
internal: n
snippet: y
---

# Demandware{#demandware}

## Product Data Import {#product-data-import}

Demandware products can be imported into AEM to be used by product pickers, components, creating product teasers, and so on.

1. Export the catalog and the product data using the Demandware Business Manager or via a scheduled job.
1. In AEM, navigate to Products: [http://localhost:4502/aem/products.html/etc/commerce/products](http://localhost:4502/aem/products.html/etc/commerce/products)
1. Click **Create** button and **Import Products**.

   ![](assets/chlimage_1-84.png)

1. Select **Demandware** as **Importer**.

   ![](assets/chlimage_1-85.png)

1. Select the exported xml as **Source** and enter a store name.

   >[!NOTE]
   >
   >It is recommended to use `demandware` for the **Demandware store name**. Other names can be used as well, but product properties scaffolding is linked to **demandware**. This can be customised within the project.

1. Click **Next**.

   >[!NOTE]
   >
   >Depending on the size of the catalog, the amount of products and associated images, this can take a few minutes. As a reference, the import of the SiteGenesis apparel catalog including product assets takes around 5 minutes.
