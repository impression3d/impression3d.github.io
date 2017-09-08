---
layout: docs
title: Content Pipeline . Building
permalink: /docs/content-pipeline/building
---

### {{ page.title }}

***

#### Introduction
You need <code>ContentBuilder</code> to build a content project. If you haven't, please grab the development toolkit.

#### Target platform
Every target platform have some special behaviour, like texture compression. You should aware, so your game will be optimized. 

#### Run builder
1.  Open terminal or command prompt
2.  On Windows environment with target platform is Android

    ```bash
    > {path-to}\ContentBuilder.exe build YourProjectName.Content.xml -t Android
    ```

    On Mac/Linux environment with target platform is Android

    ```bash
    > mono {path-to}\ContentBuilder.exe build YourProjectName.Content.xml -t Android
    ```