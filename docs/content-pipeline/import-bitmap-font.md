---
layout: docs
title: Content Pipeline . Import Bitmap Font
permalink: /docs/content-pipeline/import-bitmap-font
---

### {{ page.title }}

***

#### Introduction
Currently, supported bitmap font format is <code>.fnt</code>. 

#### Add bitmap font content to project
Just set <code>Importer</code> name to <code>BitmapFontImporter</code> and <code>Processor</code> name to <code>SpriteFontProcessor</code>, like below.

```xml
<Item Include="\Fonts\petangue-42.fnt">
  <Name>petangue-42</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="BitmapFontImporter" />
  <Processor Name="SpriteFontProcessor" />
</Item>
```

You can create custom <code>Importer</code> library <code>.dll</code> to support <code>.xml</code> bitmap font format.