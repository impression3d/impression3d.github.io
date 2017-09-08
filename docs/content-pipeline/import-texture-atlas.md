---
layout: docs
title: Content Pipeline . Import Texture Atlas
permalink: /docs/content-pipeline/import-texture-atlas
---

### {{ page.title }}

***

#### Introduction
Currently, supported texture atlas formats are <code>.json</code> and <code>.xml</code>.

#### Json format sample

```json
{
    "SubTexture": [
        {
            "y": 60,
            "height": 53,
            "x": 135,
            "name": "lowerbody",
            "width": 44
        },
        {
            "y": 0,
            "height": 99,
            "x": 0,
            "name": "upperbody",
            "width": 60
        }
    ],
    "imagePath": "Robot.png",
    "name": "Robot"
}
```

#### Xml format sample

```xml
<TextureAtlas name="Warrior" imagePath="Warrior.png">
  <SubTexture name="outerarm_upper" x="312" y="130" width="71" height="110"/>
  <SubTexture name="outerarm_lower" x="385" y="227" width="61" height="81"/>
</TextureAtlas>
```

#### Add texture atlas content to project
Just set <code>Importer</code> name to <code>TextureAtlasImporter</code> and <code>Processor</code> name to <code>SpriteSheetProcessor</code>, like below.

```xml
<Item Include="\Atlases\Warrior\Warrior.xml">
  <Name>Warrior</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="TextureAtlasImporter" />
  <Processor Name="SpriteSheetProcessor">
    <TextureFormat>Compressed</TextureFormat>
  </Processor>
</Item>
```

Defaultly, <code>TextureFormat</code> is <code>Color</code> and to get best performance when rendering should be set to <code>Compressed</code>. You can create custom <code>Importer</code> library <code>.dll</code> to support other texture atlas format.