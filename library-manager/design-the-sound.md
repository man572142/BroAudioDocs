# Design The Sound

How a sound would be played and how it will behave is all recorded in Entity.

#### Name

Click the text field to name the entity when it's unfolded.&#x20;

The name will be used in the AudioID dropdown menu, so a meaningful name is recommended.

#### AudioType

The AudioType of the entity, it could be utilized by the API such as SetVolume(AudioType) or SetEffect(AudioType) ...etc. Choose the type that suits your needs.

## Clips

#### PlaybackMode

When an entity is played, it will follow the rule of this setting to pick an AudioClip for it.

If there is more than one AudioClip, the PlaybackMode options will appear in the header of the clip list

1. **Single:** always play the first AudioClip.
2. **Sequence:** The first playback will be at index 0, the second will be at index 1, and so on. After playing the last AudioClip, the next playback will return to index 0.
3. **Random:** It will randomly select one AudioClip based on its weight. Probability is calculated as: _Weight/Total sum of all weights._

if there is only one AudioClip, the options won't show, and it will use **Single** mode

####

#### Clips

The list that stores all the AudioClips. Each clip can have different parameter settings, and they will be picked by PlaybackMode. The parameters will be shown when one of the clips is selected.

### Clip Parameters

#### Volume

the max audio volume that the clip will be played.

#### Playback Position (in seconds)

{% hint style="info" %}
Playback position can be controlled by draging the icon on the waveform GUI, and the green guiding line could help you see the playback flow more clearly.
{% endhint %}

**Start:** The starting point of the clip.

**End:** The ending point of the clip.

**In:** The duration time of the fade in process.

**Out:** The duration time of the fade out process.

**Delay:** The duration time before the entity play.



## Settings

#### Master Volume



#### Pitch

#### Priority

#### Spatial
