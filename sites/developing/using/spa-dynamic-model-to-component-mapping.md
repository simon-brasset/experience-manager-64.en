---
title: Dynamic Model to Component Mapping for SPAs
seo-title: Dynamic Model to Component Mapping for SPAs
description: null
seo-description: This article describes how the dynamic model to component mapping occurs in the Javascript SPA SDK for AEM.
uuid: f905692c-bff6-4acd-870a-8b8e2533e26d
contentOwner: bohnert
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: spa
content-type: reference
discoiquuid: fe3a2c9c-3cb2-472c-9fb0-b29ef8c3ee43
index: y
internal: n
snippet: y
---

# Dynamic Model to Component Mapping for SPAs{#dynamic-model-to-component-mapping-for-spas}

This document describes how the dynamic model to component mapping occurs in the Javascript SPA SDK for AEM.

## ComponentMapping Module {#componentmapping-module}

The `ComponentMapping` module is provided as an NPM package to the front-end project. It stores front-end components and provides a way for the Single Page Application to map front-end components to AEM resource types. This enables a dynamic resolution of components when parsing the JSON model of the application.

Each items present in the model contains a `:type` field that exposes an AEM resource type. When mounted, the front-end component can render itself using the fragment of model it has received from the underlying libraries.

Please refer to the [SPA Blueprint](../../developing/using/spa-blueprint.md) document for more information about model parsing and the front-end component access to the model.

Also see the npm package: [https://www.npmjs.com/package/@adobe/cq-spa-component-mapping](https://www.npmjs.com/package/@adobe/cq-spa-component-mapping)

## Model-Driven Single Page Application {#model-driven-single-page-application}

Single Page Applications leveraging the Javascript SPA SDK for AEM are model-driven:

1. Front-end components register themselves to the [Component Mapping Store](../../developing/using/spa-dynamic-model-to-component-mapping.md#main-pars-header-396526892).
1. Then the [Container](../../developing/using/spa-blueprint.md#main-pars-header-496071810), once provided with a model by the [Model Provider](../../developing/using/spa-blueprint.md#main-pars-header-451661207), iterates over its model content ( `:items`).

1. In the case of a page, its children ( `:children`) first get a component class from the [Component Mapping](../../developing/using/spa-blueprint.md#main-pars-header-906602219) and then instantiate it.

## App Initialization {#app-initialization}

Each component is extended with the capabilities of the [ `ModelProvider`](../../developing/using/spa-blueprint.md#main-pars-header-451661207). Initialization therefore take the following general form:

1. Each model provider initializes itself and listens for changes made to the piece of model that corresponds to its inner component. 
1. The [ `PageModelManager`](../../developing/using/spa-blueprint.md#main-pars-header-249430796) must be initialized as represented by the [initialization flow](../../developing/using/spa-blueprint.md#main-pars-text-1679624069). 

1. Once stored, the page model manager returns the complete model of the app. 
1. This model is then passed to the front-end root [Container](../../developing/using/spa-blueprint.md#main-pars-header-496071810) component of the application. 
1. Pieces of the model are finally propagated to each individual child component.

![](assets/app_model_initialization.png)
