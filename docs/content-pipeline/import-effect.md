---
layout: docs
title: Content Pipeline . Import Effect
permalink: /docs/content-pipeline/import-effect
---

### {{ page.title }}

***

#### Introduction
Importing effect is powered by [Sylabs](https://github.com/pratamabayu/Sylabs) with <code>.fx</code> extension. The syntax is like HLSL, but with custom rules. The effects for all windows platforms can only be built in windows environment.

See [stock effect](http://github.com/impression3d/Impression.StockEffect) samples to explore built-in effects.

#### Add mesh content to project
Just set <code>Importer</code> name to <code>EffectImporter</code> and <code>Processor</code> name to <code>EffectProcessor</code>, like below.

```xml
<Item Include="\Effect\Blur.fx">
  <Name>Blur</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="EffectImporter" />
  <Processor Name="EffectProcessor">
    <HiDef>true</HiDef>
    <Log>true</Log>
  </Processor>
</Item>
```

Defaultly, <code>HiDef</code> and <code>Log</code> are <code>false</code>. Currently, <code>HiDef</code> is only available on Windows target platform that support Shader Model 4.