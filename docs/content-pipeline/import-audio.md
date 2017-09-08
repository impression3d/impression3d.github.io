---
layout: docs
title: Content Pipeline . Import Audio
permalink: /docs/content-pipeline/import-audio
---

### {{ page.title }}

***

#### Introduction
Currently, supported audio formats are <code>.wav</code> for sound effect (sampling audio) and <code>.mp3</code> or <code>.ogg</code> for song (streaming audio).

#### Add sound effect content to project
Just set <code>Importer</code> name to <code>AudioImporter</code> and <code>Processor</code> name to <code>SoundEffectProcessor</code>, like below.

```xml
<Item Include="\Audio\Electrical-Tone.wav">
  <Name>Electrical-Tone</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="AudioImporter" />
  <Processor Name="SoundEffectProcessor"/>
</Item>
```

#### Add song content to project
Just set <code>Importer</code> name to <code>AudioImporter</code> and <code>Processor</code> name to <code>SongProcessor</code>, like below.

```xml
<Item Include="\Audio\Srengenge.mp3">
  <Name>Srengenge</Name>
  <BuildAction>Compile</BuildAction>
  <Importer Name="AudioImporter" />
  <Processor Name="SongProcessor"/>
</Item>
```