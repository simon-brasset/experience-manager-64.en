---
title: eCommerce
seo-title: eCommerce
description: AEM eCommerce helps marketers deliver branded, personalized shopping experiences across web, mobile, and social touchpoints. 
seo-description: AEM eCommerce helps marketers deliver branded, personalized shopping experiences across web, mobile, and social touchpoints. 
uuid: 14af7a3a-7211-4a56-aeef-1603128d5d8a
contentOwner: Guillaume Carlino
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: e-commerce
content-type: reference
discoiquuid: 68799110-8183-40fe-be4f-2a7c7a7b3018
---

# eCommerce{#ecommerce}

* [Concepts](/help/sites-administering/concepts.md)
* [Administering (generic)](/help/sites-administering/generic.md)
* [hybris](/help/sites-administering/hybris.md)
* [Elastic Path](/help/sites-administering/elasticpath.md)
* [Intershop](/help/sites-administering/intershop.md)
* [IBM Websphere Commerce](/help/sites-administering/ibm-websphere.md)
* [Demandware](/help/sites-administering/demandware.md)
* [Magento](/help/sites-administering/magento.md)
* [Digital River](/help/sites-administering/digital-river.md)

>[!NOTE]
>
>The connectors for AEM 6.4 are still under development.

eCommerce, together with Product Information Management (PIM), handles the activities of a website focused on selling products via an online store:

* Creation, lifetime, and obsolescence of a product
* Price management
* Transaction management
* Management of entire catalogs  
* Live and centralized storage records
* Web interfaces

AEM eCommerce helps marketers deliver branded, personalized shopping experiences across web, mobile, and social touchpoints. The AEM authoring environment allows you to customize pages and components based on target visitor context and merchandising strategies; for example:

* Product pages
* Shopping cart components
* Checkout components

The implementation allows real-time access to product information. This can be used to enforce:

* Product information integrity
* Pricing
* Stock-keeping inventory
* Variations in state of a shopping cart

>[!NOTE]
>
>To use the integration framework with external eCommerce providers, you first need to install the required packages. For more information, see [Deploying eCommerce](/help/sites-deploying/ecommerce.md).
>
>For information about extending eCommerce capabilities, see [Developing eCommerce](/help/sites-developing/ecommerce.md).

## Main Features {#main-features}

AEM eCommerce provides:

* A number of **out-of-the-box AEM components** to illustrate what can be achieved for your project:

    * Product display  
    * Shopping cart  
    * Check-out  
    * Recently viewed products
    * Vouchers
    * and others

  ![](assets/chlimage_1-150.png)

  >[!NOTE]
  >
  >The integration framework provided by AEM also allows you to build additional AEM components for commerce capabilities independent of your specific eCommerce engine.

* **Search** - using either:

    * the AEM search
    * the search of the eCommerce system
    * a third party search (such as Search&Promote)   
    * or a combination thereof.

  ![](assets/chlimage_1-151.png)

* Uses the AEM ability to **present your content on multiple channels**, be that full browser window or mobile device. This delivers your content in the format needed by your visitors.

  ![](assets/chlimage_1-152.png)

* The ability to **develop your own integration implementation based on the [AEM eCommerce framework](#the-framework)**.

  The two implementations currently available are both built on the same basis - on top of the general API (the framework). Implementing a new integration only involves implementing the feature(s) that your integration needs. Front end components can be used by any new implementation as they use interfaces (so are independent from the implementation).

* The possibility to develop **experience-driven commerce based on shopper data and activity**. This allows you to realize many scenarios:

    * One example might be providing reductions in shipping costs when the total order exceeds a specific amount.  
    * Another might allow you to provide seasonal offers that use profile data (e.g. location). These can then be highlighted, again depending on other factors when necessary.

  In the example below one teaser is shown as the contents of the cart are less than $75:

  ![](assets/chlimage_1-153.png)

  This can be changed when the contents of the cart exceed $75:

  ![](assets/chlimage_1-154.png)

* And other features including:

    * Shopping cart contents retained across sessions
    * Full order history  
    * Express catalog update

## The Framework {#the-framework}

The [Concepts](/help/sites-administering/concepts.md) section covers the framework in more detail, but the following provides a high-level, high-speed view of the framework:

### What? {#what}

* The integration framework provides the API, a range of components to illustrate functionality and several extensions to provide examples of connection methods.
* The framework provides the basic structure needed for a project implementation.
* The framework is extensible.  
* The framework does not provide an out-of-the-box, ready-to-use site. A certain amount of development work is always needed to adapt the framework to your specifications.

### Why? {#why}

* To provide the basic mechanisms needed to quickly realise a customized eCommerce site.
* Tp provide the flexibility needed for developing a real-life eCommerce site.
* Illustrate best practices.
