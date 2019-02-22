---
title: Authoring - the Environment and Tools
seo-title: Authoring - the Environment and Tools
description: The authoring environment of AEM provides various mechanisms for organizing and editing your content
seo-description: The authoring environment of AEM provides various mechanisms for organizing and editing your content
uuid: 069c425a-1058-4c02-a2d0-0b04d9277038
contentOwner: Chris Bohnert
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: page-authoring
content-type: reference
discoiquuid: 2aafd551-901a-4564-8425-91053af976fe
index: y
internal: n
snippet: y
---

# Authoring - the Environment and Tools{#authoring-the-environment-and-tools}

The authoring environment of AEM provides various mechanisms for organizing and editing your content. The tools provided are accessed from the various consoles and page editors.

## Managing your Site {#managing-your-site}

The **Sites** console allows you to navigate and manage your website, using the header bar, toolbar, action icons (applicable for the selected resource), breadcrumbs and when selected, secondary rails (for example, timeline and references).

For example, card view:

![](assets/chlimage_1-386.png) 

## Editing Page Content {#editing-page-content}

You can edit a page with the page editor. For example:

`http://localhost:4502/editor.html/content/we-retail/us/en/equipment.html`

![](assets/screen_shot_2018-03-22at141536.png)

>[!NOTE]
>
>The first time you open a page for editing, a series of slides will provide you with a tour of the features.
>
>You can skip the tour if wanted and repeat it at any time by selecting from the **Page Information** menu.

## Accessing Help {#accessing-help}

When editing a page, **Help** can be accessed from:

* the [**Page Information**](../../../sites/authoring/using/editing-page-properties.md#main-pars-title-1005086348) selector; this will show the introductory slides (as shown the first time you access the editor).
* the [configuration](../../../sites/authoring/using/editing-content.md#main-pars-title-32) dialog for specific components (using the ? icon in the dialog toolbar); this will show context sensitive help.

Further [help-related resources are available from consoles](../../../sites/authoring/using/basic-handling.md#main-pars-title-24).

## Components Browser {#components-browser}

The components browser shows all components that are available for use on your current page. These can be dragged to the appropriate location, then edited to add your content.

The components browser is a tab within the side panel (together with the [assets browser](../../../sites/authoring/using/author-environment-tools.md#main-pars-title) and [content tree](../../../sites/authoring/using/author-environment-tools.md#main-pars-title-96d3)). To open (or close) the side panel use the icon at the top left of the toolbar:

![](assets/screen_shot_2018-03-22at141659.png)

When you open the side panel it will slide open from the left side (select the **Components** tab if necessary). When open you can browse through all the components available for your page.

The actual appearance and handling is dependent on the device type you are using:

>[!NOTE]
>
>A mobile device is detected when the width is less than 1024px. This can also be the case for a small desktop window.

* The component browser completely covers the page being edited.

  To add a component to your page touch-and-hold the required component and move it towards the right - the component browser will close to show the page again - where you can position the component.

  ![](assets/screen_shot_2018-03-22at141752.png)

* The component browser is opened at the left side of the window.

  To add a component to your page click on the required component and drag it to the required location.

  ![](assets/screen_shot_2018-03-22at141808.png)

  Components are represented by

    * Component name
    * Component group (in grey)
    * Icon or abbreviation

        * Standard components' icons are monochrome.
        * Abbreviations are always the first two charaters of the component name.

  From the top toolbar in the Components browser you can:

    * Filter components by name.  
    * Limit the display to a specific group using the drop down selection.

  For a more detailed description of the component, you can click or tap the information icon next to the component in the Components browser (if available).

  ![](assets/screen_shot_2018-03-22at141929.png)

  For even more information about the components available to you see the [Component Console](../../../sites/authoring/using/default-components-console.md).

## Assets Browser {#assets-browser}

The assets browser shows all [assets](/assets/using/author-assets) that are available for direct use on your current page.

The assets browser is a tab within the side panel along with the [components browse](../../../sites/authoring/using/author-environment-tools.md#main-pars-title-17)r and [content tree](../../../sites/authoring/using/author-environment-tools.md#main-pars-title-96d3). To open or close the side panel use the icon at the top left of the toolbar:

![](assets/screen_shot_2018-03-22at141659-1.png)

When you open the side panel it will slide open from the left side. Select the **Assets** tab if necessary.

![](assets/screen_shot_2018-03-22at142035.png)

When the assets browser is open you can browse through all the assets available for your page. Infinite scrolling is used to expand the list when required.

![](assets/chlimage_1-387.png)

To add an asset to your page, select and drag to the required location. This can be:

* An existing component of the appropriate type.

    * For example, you can drag an asset of type image onto an Image component.

* A [placeholder](../../../sites/authoring/using/editing-content.md#main-pars-title-3) in the paragraph system to create a new component of the appropriate type.

    * For example, you can drag an asset of type image onto the parargraph system to create an Image component.

>[!NOTE]
>
>This is available for specific assets and component types. See [Inserting a Component using the Assets Browser](../../../sites/authoring/using/editing-content.md#main-pars-title-18) for more details.

From the top toolbar of the assets browser you can filter the assets by:

* Name
* Path
* Asset type such as images, manuscripts, documents, videos, pages, paragraphs, and products  
* Asset characteristics such as Orientation (Portrait, Landscape, Square) and Style (Color, Monochrome, Grayscale)

    * Available only for certain asset types

The actual appearance and handling is dependent on the device type you are using:

>[!NOTE]
>
>A mobile device is detected when the width is less than 1024px; i.e. also on a small desktop window.

* The assets browser completely covers the page being edited.

  To add an asset to your page touch-and-hold the required asset, then move it towards the right - the assets browser will close to show the page again, where you can add the asset to the required component.

  ![](assets/screen_shot_2018-03-22at142223.png)

* The assets browser is opened at the left side of the window.

  To add an asset to your page click on the required asset and drag it to the required component or location.

  ![](assets/screen_shot_2018-03-22at142337.png)

If you need to quickly make a change to an asset, you can start the [asset editor](../../../assets/using/managing-assets-touch-ui.md) directly from the asset browser by clicking the edit icon shown next to the asset's name.

![](assets/screen_shot_2018-03-22at142448.png) 

## Content Tree {#content-tree}

The **Content Tree** gives an overview of all of the components on the page in a hierarchy so you can see at a glance how the page is composed.

The Content Tree is a tab within the side panel (together with the components and assets browser). To open (or close) the side panel use the icon at the top left of the toolbar:

![](assets/screen_shot_2018-03-22at142042.png)

When you open the side panel it will slide open (from the left side). Select the **Content Tree** tab if necessary. When open you can see a tree view representation of your page or template, so that it's easier to understand how its content is structured hierarchically. Additionally on a complex page, it makes it easier to jump between components of the page.

![](assets/screen_shot_2018-03-22at142526.png)

A page can easily be composed of many of the same type of components, so the component tree displays descriptive text (in grey) after the name of the component type (in black). The descriptive text comes from common properties of the component such as title or text.

Component types will be shown in the user language, whereas the component description text comes from the page language.

Clicking the chevron next to a component will collapse or expand that level.

![](assets/screen_shot_2018-03-22at142559.png)

Clicking on the component will highlight the component in the page editor.

![](assets/screen_shot_2018-03-22at142647.png)

If the component you click in the tree is editable a wrench icon will appear to the right of the name. Clicking on this icon will directly start the edit dialogue for the component.

![](assets/screen_shot_2018-03-22at142725.png)

>[!NOTE]
>
>The Content Tree is not available if you are editing a page on a mobile device (if the browser width is less than 1024px).

## Fragments - Associated Content Browser {#fragments-associated-content-browser}

If your page contains Content Fragments then you will also have access to the [browser for Associated Content](../../../sites/authoring/using/content-fragments.md#main-pars-title-2096066215).

## References {#references}

**References** shows connections to the selected page:

* Blueprints
* Launches
* Live copies
* Language copies
* Use of the reference component
* References to Product pages (from the Commerce - Products console)

Open the required console, then navigate to the required resource and open **References** using:

![](assets/screen_shot_2018-03-22at153653.png)

[Select your required resource](../../../sites/authoring/using/basic-handling.md#main-pars-title-14) to show a list of references types relevant to that resource:

![](assets/screen_shot_2018-03-22at153731.png)

Select the appropriate reference type for more information. In certain situations further actions are available when you select a specific reference, including:

* Instances of the Reference component (e.g. navigate to referencing/referenced page)  
* [References to Product pages](../../../sites/administering/using/generic.md#showingproductreferences) (available from the Commerce-Products console)
* [Launches](../../../sites/authoring/using/launches.md)
* [Live Copies](../../../sites/administering/using/msm.md) displays the paths of all live copies that are based on the selected resource.
* [Blueprint](../../../sites/administering/using/msm-best-practices.md)
* [Languages Copies](../../../sites/administering/using/tc-manage.md#creatingtranslationprojectsusingthereferencespanel)

For example, you can fix a broken reference within a Reference component:

![](assets/chlimage_1-388.png) 

## Events - Timeline {#events-timeline}

For appropriate resources (e.g. pages from the **Sites** console, or assets from the **Assets** console) the [timeline can be used to show the recent activity on any selected items](../../../sites/authoring/using/basic-handling.md#main-pars-title-281465694).

Open the required console, then navigate to the required resource and open **Timeline**, using:

![](assets/screen_shot_2018-03-22at153952.png)

[Select your required resource](../../../sites/authoring/using/basic-handling.md#main-pars-title-14), then either **Show All** or **Activities** to list any recent actions on the selected resources:

![](assets/screen_shot_2018-03-22at154130.png) 

## Page Information {#page-information}

The Page Information (equalizer icon) opens a menu that also provides details about the last edit and the last publication. Depending on the characteristics of the page (and its site) more or fewer options might be available:

![](assets/screen_shot_2018-03-22at154210.png)

* [Open Properties](../../../sites/authoring/using/editing-page-properties.md)
* [Rollout Page](../../../sites/administering/using/msm.md#main-pars-title-2120087243)
* [Start Workflow](../../../sites/authoring/using/workflows-applying.md#main-pars-title-4)
* [Lock Page](../../../sites/authoring/using/editing-content.md#main-pars-title-13)
* [Publish Page](../../../sites/authoring/using/publishing-pages.md#main-pars-title-10)
* [Unpublish Page](../../../sites/authoring/using/publishing-pages.md#main-pars-title-5)
* [View as Published](../../../sites/authoring/using/editing-content.md#main-pars-title-1534569976)
* [View in Admin](../../../sites/authoring/using/basic-handling.md#main-pars-title-14)
* [Help](../../../sites/authoring/using/basic-handling.md#main-pars-title-24)

For example, when appropriate, **Page Information** also has the options:

* [Promote Launch](../../../sites/authoring/using/launches-promoting.md) if the page is a launch.
* [Edit Template](../../../sites/authoring/using/templates.md) if the page is based on an [editable template](../../../sites/authoring/using/templates.md#main-pars-title-1120829965)

* [Open in Classic UI](../../../sites/authoring/using/select-ui.md#main-pars-title-5) if this options has been [enabled by an administrator](../../../sites/administering/using/enable-classic-ui-editor.md)

In addition, **Page Information** can provide access to analytics and recommendations, when appropriate.

## Page Modes {#page-modes}

There are various modes when editing a page allowing for different actions:

* [Edit](../../../sites/authoring/using/editing-content.md) - the mode to use when editing the page content.
* [Layout](../../../sites/authoring/using/responsive-layout.md) - allows you to create and edit your responsive layout dependent on device (if the page is based on a layout container)  

* [Scaffolding](../../../sites/authoring/using/scaffolding.md) - help you to create a large set of pages that share the same structure but have differing content.
* [Developer](../../../sites/developing/using/developer-mode.md) - allows you to perform various actions (requires privileges). These include inspecting the technical details of a page and its components.  

* [Design](../../../sites/authoring/using/default-components-designmode.md) - allows you to enable/disable components for use on a page and to configure the design of the component (if the page is based on a [static template](../../../sites/authoring/using/templates.md#main-pars-title-1120829965)).

* [Targeting](../../../sites/authoring/using/content-targeting-touch.md) - increase content relevance through targeting and measuring across all channels.
* [Activity Map](../../../sites/authoring/using/pa-using.md#analyticsvisiblefromthepageeditor) - shows Analytics data for the page.  

* [Timewarp](../../../sites/authoring/using/working-with-page-versions.md#main-pars-title-951f) - allows you to view a pages state at a particular point in time.
* [Live Copy Status](../../../sites/authoring/using/editing-content.md#main-pars-title-4) - allows a quick overview of the live copy status and which components are/are not inherited.
* [Preview](../../../sites/authoring/using/editing-content.md#main-pars-title-9) - used to view the page as it will be shown on the publish environment; or to navigate using links in the content.  

* [Annotate](../../../sites/authoring/using/annotations.md) - used to add or view annotations on the page.

You can access these using the icons in the top right corner. The actual icon will change to reflect the mode you are currently using:

![](assets/chlimage_1-389.png)

>[!NOTE]
>
>* Depending on the characteristics of the page, some modes my not be available.
>* Access to some modes require the appropriate permissions/privileges.
>* Developer mode is not available on mobile devices due to space restrictions.
>* There is a [keyboard shortcut](../../../sites/authoring/using/page-authoring-keyboard-shortcuts.md) ( `Ctrl-Shift-M`) to toggle between **Preview** and the currently selected mode (e.g. **Edit**, **Layout**, etc).
>

## Path Selection {#path-selection}

Often when authoring it is necessary to select another resource such as when defining a link to another page or resource or selecting an image. To easily select a path, [path fields](../../../sites/authoring/using/author-environment-tools.md#main-pars-title-7c8e) offer auto-complete and the [path browser](../../../sites/authoring/using/author-environment-tools.md#main-pars-title-b097) allows for more robust selection.

### Path Fields {#path-fields}

The example used here to illustrate is the image component. For more information about using and editing components see [Components for Page Authoring](../../../sites/authoring/using/default-components.md).

Path fields have auto-complete and look-ahead funtionality now to make locating a resource easier. Simply start typing in the path field and the AEM will offer matching paths as you type.

![](assets/screen_shot_2018-03-22at154403.png)

Clicking the **Open Selection Dialog** button in the path field opens the [path browser](../../../sites/authoring/using/author-environment-tools.md#main-pars-title-b097) dialog to allow for more detailed selection options.

![](assets/screen_shot_2018-03-22at154427.png) 

### Path Browser {#path-browser}

The path browser is organized like the [column view](../../../sites/authoring/using/basic-handling.md#main-pars-title-1571169225) of the sites console, allowing for more detailed selection of resources.

![](assets/screen_shot_2018-03-22at154521.png)

Once a resource is selected, the **Select** button at the upper-right of the dialogue becomes active. Click or tap to confirm the selection or **Cancel** to abort.

If the context allows for the selection of multiple resources, selecting a resource also activates the Select button, but also adds a count of the number of selected resources to the upper-right of the window. Click the X next to the number to deselect all.

![](assets/chlimage_1-390.png)

The breadcrumbs can be used to quickly jump within the resource hierarchy.

![](assets/chlimage_1-391.png)

At any time you can use the search field at the top of the dialogue.

![](assets/chlimage_1-392.png)

Click the X in the search field to clear the search.

To narrow your search, you can reveal the filter options and filter your results based on a certain path.

![](assets/chlimage_1-393.png) 

## Keyboard Shortcuts {#keyboard-shortcuts}

Various [keyboard shortcuts](../../../sites/authoring/using/page-authoring-keyboard-shortcuts.md) are available.