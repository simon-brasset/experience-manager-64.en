---
title: Code pitfalls
seo-title: Code pitfalls
description: null
seo-description: Common coding pitfalls to avoid when developing for AEM
uuid: 8c5417e8-83be-4173-95c6-eb1aabeec77a
contentOwner: User
products: SG_EXPERIENCEMANAGER/6.4/SITES
content-type: reference
topic-tags: best-practices
discoiquuid: a91c0e5d-b8e5-40ed-b328-2c743daf5439
isreadyforlocalization: false
index: y
internal: n
snippet: y
---

# Code pitfalls{#code-pitfalls}

### Avoid Sling Bindings in Java code {#avoid-sling-bindings-in-java-code}

Sling Bindings are an inappropriate way to get access to a service in 90% of cases. Instead, you should use *@Reference* or *@Inject* annotations.

### Avoid Thread.interfupt in Java code {#avoid-thread-interfupt-in-java-code}

*Thread.interrupt* is dangerous because it can close files, including Lucene files and persistent cache files, when called at the wrong time.

### Avoid mixing Java synchronization with ReadWriteLocks {#avoid-mixing-java-synchronization-with-readwritelocks}

This can lead to a race condition in which the code will eventually deadlock. 