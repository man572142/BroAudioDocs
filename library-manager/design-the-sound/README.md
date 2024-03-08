---
description: How a sound would be played and how it will behave is all set in Entity.
---

# Design The Sound

## Name

Click the text field to name the entity when it's unfolded.&#x20;

<mark style="background-color:orange;">The name will be used in the AudioID dropdown menu, so a meaningful name is recommended.</mark>

## AudioType

The AudioType of the entity, it could be utilized by the API such as SetVolume(AudioType) or SetEffect(AudioType) ...etc. Choose the type that suits your needs.

## Clips

### Clip List

The list that stores all the AudioClips. Each clip can have different parameter settings, and they will be picked by PlaybackMode. The parameters will be shown when one of the clips is selected.

### PlaybackMode

When an entity is played, it will follow the rule of the following options to pick an AudioClip.

1. **Single:** always play the first AudioClip.
2. **Sequence:** The first playback will be at index 0, the second will be at index 1, and so on. After playing the last AudioClip, the next playback will return to index 0.
3. **Random:** It will randomly select one AudioClip based on its weight. Probability is calculated as: _Weight/Total sum of all weights._

🔔 if there is only one AudioClip, the options won't show, and it will use **Single** mode



### Clip Parameters

#### Volume

The audio volume that the clip will be played. More details in [Volume Control](volume-control.md).

#### Playback Position (in seconds)

{% hint style="info" %}
The playback position can be controlled by dragging the icon on the waveform GUI, and the green guiding line could help you see the playback flow more clearly.
{% endhint %}

**Start:** The starting point of the clip.

**End:** The ending point of the clip.

**In:** The duration time of the fade-in process.

**Out:** The duration time of the fade-out process.

**Delay:** The duration time before the entity plays.



## Settings

### Master Volume

The audio volume that the entity will be played. It is useful when using multiple clips in an entity.

The final volume will be :\
<mark style="background-color:green;">clip volume \* master volume</mark> (normalized), or <mark style="background-color:blue;">clip volume + master volume</mark>(In dB).\
For example: the clip's volume is 0.5 (-6.02dB) and the master volume is 2 (+6.02dB), so the final volume is 1 (0dB).

{% hint style="info" %}
This setting supports randomization! click the \[RND] button to set its random range.
{% endhint %}

### Pitch

The pitch of the entity. Currently, it is the same as AudioSource's pitch, which is achieved through time stretching. The higher the pitch is set, the more it is shortened.

{% hint style="info" %}
This setting supports randomization! click the \[RND] button to set its random range.
{% endhint %}

### Priority

The same as AudioSource's priority. [see Unity's Doc](https://docs.unity3d.com/Manual/class-AudioSource.html)

### Looping

Let the entity automatically replay when it ends. More details in [Seamless Loop](seamless-loop.md).

### Spatial

All the settings that show in the popup window are the same as AudioSource. [see Unity's Doc](https://docs.unity3d.com/Manual/class-AudioSource.html)
