---
layout: docs
title: Content Pipeline . Import Meshes
permalink: /docs/content-pipeline/import-meshes
---

### {{ page.title }}

***

#### Introduction
Importing mesh is powered by [Assimp](https://github.com/assimp/assimp/blob/master/port/AssimpNET/Readme.md). Assimp support many mesh format, nevertheless we recommend <code>.fbx</code> or <code>.obj</code>.

#### Add mesh content to project
Just set <code>Importer</code> name to <code>OpenAssetImporter</code> and <code>Processor</code> name to <code>ModelProcessor</code>, like below.

```xml
<Item Include="\Models\Tank\Tank.fbx">
  <Name>Tank</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="OpenAssetImporter" />
  <Processor Name="ModelProcessor">
    <TextureFormat>Compressed</TextureFormat>
  </Processor>
</Item>
```

#### Add skinned mesh content to project
Just set <code>Importer</code> name to <code>OpenAssetImporter</code>, <code>Processor</code> name to <code>SkinnedModelProcessor</code>, and <code>StockEffect</code> value to <code>SkinnedEffect</code>, like below.

```xml
<Item Include="\Models\Karakter\Karakter.fbx">
  <Name>Karakter</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="OpenAssetImporter" />
  <Processor Name="SkinnedModelProcessor">
    <StockEffect>SkinnedEffect</StockEffect>
    <TextureFormat>Compressed</TextureFormat>
  </Processor>
</Item>
```

Defaultly, <code>TextureFormat</code> is <code>Compressed</code> for best performance when rendering. You can create custom <code>Importer</code> library <code>.dll</code> to support other mesh format.