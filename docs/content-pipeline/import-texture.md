---
layout: docs
title: Content Pipeline . Import Texture
permalink: /docs/content-pipeline/import-texture
---

### {{ page.title }}

***

#### Introduction
Currently, supported texture formats are <code>.png</code>, <code>.jpg</code>, and <code>.bmp</code>.

#### Add texture content to project
Just set <code>Importer</code> name to <code>TextureImporter</code> and <code>Processor</code> name to <code>TextureProcessor</code>, like below.

```xml
<Item Include="\Textures\Impression.png">
  <Name>Impression</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="TextureImporter" />
  <Processor Name="TextureProcessor">
    <TextureFormat>Compressed</TextureFormat>
  </Processor>
</Item>
```

Defaultly, <code>TextureFormat</code> is <code>Color</code> and to get best performance when rendering should be set to <code>Compressed</code>. You can create custom <code>Importer</code> library <code>.dll</code> to support other texture format.