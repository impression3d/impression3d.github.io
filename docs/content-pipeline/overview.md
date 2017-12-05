---
layout: docs
title: Content Pipeline . Overview
permalink: /docs/content-pipeline/overview
---

### {{ page.title }}

***

#### Introduction

Content pipeline is process to convert any native content format like <code>.png</code> and <code>.obj</code> to general content format <code>.bin</code>, or steadfastly use native content format. Content building should be carried out when development phase. So loading and reading content get best performance on runtime.

#### Project structure
Usually, project file name is <code>YourProjectName.Content.xml</code> in under <code>YourProjectName</code> folder.

```xml
<?xml version="1.0" encoding="utf-8"?>
<ContentProject>
  <Name>YourProjectName.Content</Name>
  <InputDirectory>YourProjectName.Content</InputDirectory>
  <OutputDirectory>bin</OutputDirectory>
  <ContentRootDirectory></ContentRootDirectory>
  <Configuration>Release</Configuration>
  <TargetPlatform>Windows</TargetPlatform>
  <References>
  </References>
  <Items>
  </Items>
</ContentProject>
```

#### Add content
All content like meshes, images, audio, font, and effects is done on <code>Items</code> markup.

```xml
<Item Include="\Textures\Impression.png">
  <Name>Impression</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="TextureImporter">
  </Importer>
  <Processor Name="TextureProcessor">
  </Processor>
</Item>
```

Include path is relative by content project folder and detail of Importer and Processor see next section. We recommend naming convention of <code>filename</code> on <code>Include</code> and <code>Name</code> is equal. <code>BuildAction</code> can be <code>None</code>, <code>Compile</code>, or <code>Copy</code>.

1. <code>Compile</code>, content will be compiled as <code>.bin</code> and copy it to <code>OutputDirectory</code>
2. <code>Copy</code>, content will not be compiled as <code>.bin</code>, but steadfastly use native content format. Actually only copy the content to <code>OutputDirectory</code>
3. <code>None</code>, content will not be <code>Compiled</code> or <code>Copy</code>

#### Add custom content pipeline importer or processor
Add your library <code>.dll</code> path to <code>References</code> markup. See code below.

```xml
....
<References>
  <Reference>{path-to}\LevelImporter.dll</Reference>
</References>
....
```

Reference path must be absolute.




