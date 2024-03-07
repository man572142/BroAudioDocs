---
description: The main entry of BroAudio, all Api starts from here !
---

# BroAudio

#### <mark style="color:blue;">NameSpace</mark>

Ami.BroAudio

#### <mark style="color:blue;">Accessibility</mark>

public static

## Public Methods

<table data-full-width="true"><thead><tr><th width="173">Method</th><th>Parameters</th><th>Description</th></tr></thead><tbody><tr><td><mark style="color:orange;"><strong>Play</strong></mark></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id</td><td>Play an audio</td></tr><tr><td></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id, <mark style="color:green;">Vector3</mark> position</td><td>Play an audio at the given position <br>(SpatialBlend will be set to 3D automatically)</td></tr><tr><td></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id, <mark style="color:green;">Transform</mark> followTarget</td><td>Play an audio and keep following a target  <br>(SpatialBlend will be set to 3D automatically)</td></tr><tr><td><mark style="color:orange;"><strong>Stop</strong></mark></td><td><a href="../enums/broaudiotype.md"><mark style="color:green;">BroAudioType</mark></a> audioType</td><td>Stop playing all audio that matches the given audio type</td></tr><tr><td></td><td><a href="../enums/broaudiotype.md"><mark style="color:green;">BroAudioType</mark></a> audioType, <mark style="color:green;">float</mark> fadeOut</td><td>Stop playing all audio that matches the given audio type with the given fadeOut time</td></tr><tr><td></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id</td><td>Stop playing an audio</td></tr><tr><td></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id, <mark style="color:green;">float</mark> fadeOut</td><td>Stop playing an audio with the given fadeOut time</td></tr><tr><td><mark style="color:orange;"><strong>Pause</strong></mark></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id</td><td>Pause an audio</td></tr><tr><td></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id, <mark style="color:green;">float</mark> fadeOut</td><td>Pause with the given fadeOut time</td></tr><tr><td><mark style="color:orange;"><strong>SetVolume</strong></mark></td><td><mark style="color:green;">float</mark> volume</td><td>Set the master volume Immediately</td></tr><tr><td></td><td><mark style="color:green;">float</mark> volume, <a href="../enums/broaudiotype.md"><mark style="color:green;">BroAudioType</mark></a> audioType</td><td>Set the volume of the given audio type Immediately</td></tr><tr><td></td><td><mark style="color:green;">float</mark> volume, <a href="../enums/broaudiotype.md"><mark style="color:green;">BroAudioType</mark></a> audioType, <mark style="color:green;">float</mark> fadeTime</td><td>Set the volume of the given audio type with the given fading time</td></tr><tr><td></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id, <mark style="color:green;">float</mark> volume</td><td>Set the volume of an audio</td></tr><tr><td></td><td><a href="../struct/audioid.md"><mark style="color:green;">AudioID</mark></a> id, <mark style="color:green;">float</mark> volume, <mark style="color:green;">float</mark> fadeTime</td><td>Set the volume of an audio with the given fading time</td></tr><tr><td><a data-footnote-ref href="#user-content-fn-1"><mark style="color:orange;"><strong>SetEffect</strong></mark></a></td><td><a href="../struct/effect.md"><mark style="color:green;">Effect</mark></a> effect</td><td>Set effect for all audio</td></tr><tr><td></td><td><a href="../struct/effect.md"><mark style="color:green;">Effect</mark></a> effect, <a href="../enums/broaudiotype.md"><mark style="color:green;">BroAudioType</mark></a> audioType</td><td>Set effect for all audio that matches the given audio type.</td></tr><tr><td></td><td>*Use the static factory method for Effect such as Effect.LowPass()</td><td></td></tr></tbody></table>



[^1]: WebGL is not supported
