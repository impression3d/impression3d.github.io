---
layout: docs
title: Getting Started . Basic Usage
permalink: /docs/getting-started/basic-usage
---

### {{ page.title }}

***

#### Introduction
Shortenly, you need <code>ProjectBuilder</code> to generate a game project. If you haven't it, please grab the development toolkit.

#### Let's generate a game project
1.  Open terminal or command prompt
2.  On Windows environment

    ```bash
    > {path-to}\ProjectBuilder.exe new YourProjectName
    ```

    On Mac/Linux environment

    ```bash
    > mono {path-to}\ProjectBuilder.exe new YourProjectName
    ```

#### Project structure
If you are succesfully creating new project, your project structure will be like below:

```bash
    YourProjectName
    .. YourProjectName.Content
    .. YourProjectName.Shared
    .... YourProjectNameGame.cs
    .. YourProjectName.Android
    .. YourProjectName.iOS
    .. YourProjectName.Linux
    .. YourProjectName.Mac
    .. YourProjectName.UniversalWindows
    .. YourProjectName.Windows
    .. YourProjectName.Platform
    .. YourProjectName.sln
    .. YourProjectName.Content.xml
```

#### Code the game
1. Open your favourite C# IDE
2. Open <code>YourProjectName.sln</code> solution

Ideally, you will code at <code>YourProjectName.Shared</code> project and <code>YourProjectNameGame.cs</code> is main entry of your game.

#### Run or debug the game
Just <code>run</code> or <code>debug</code> like other C# project. At first time, building need internet connection to download some dependencies. If successfully, you will see an empty <code class="badge badge-feature">burlywood color</code> game window.