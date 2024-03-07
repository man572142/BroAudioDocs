---
description: Know the terminologies of Audio
---

# BroAudio

## Asset&#x20;

A collection of multiple entities, it's a Unity ScriptableObject that saves as an .asset file. You create and name it by scenes, characters, weapons, or any other category. (see the example pic)

## Entity

A sound or a group of sounds, containing specified AudioClips along with various playback parameters. It is the primary entity used for playback.

## AudioID

A unique ID for an entity. Use \[SerializedField] to show a dropdown menu on the inspector to address the entity that you want to play.

## AudioType

A tag to help you organize the sounds. it could be used for APIs like: SetEffect(), SetVolume() ...etc

the list of all AudioType shown below

* Music
* Sfx
* UI
* Ambience
* VoiceOver
* All

### The Volume Slider Design

