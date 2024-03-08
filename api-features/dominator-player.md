---
coverY: 0
---

# Dominator Player

Dominator allows you to 'dominate' other sounds while playing it, meaning Dominator will play in a normal way, while other sounds will be affected by the effects you specify until the Dominator is finished.

## Common use cases and API examples:

#### When an explosion occurs nearby, other sounds become temporarily unclear, but the tinnitus, heartbeat, or breathing remain clear.

```csharp
BroAudio.Play(_explosion).AsDominator().LowPassOthers(_lowPassFrequency); 
BroAudio.Play(_tinnitus).AsDominator(); // dominators share the same effect, we don't need to set in this line again
```

#### When the theme song plays,  lower the volume of all other sounds.

```csharp
BroAudio.Play(_deathStrandingAwesomeMusic).AsDominator().QuietOthers(othersVol);
```

#### When a character is speaking, lower the volume of the background music.

```csharp
BroAudio.Play(_talking).AsDominator(BroAudioType.Music).QuietOthers(othersVol);
```

### Side Note:

Even though this feature is straightforward and effective, it might not cover all complex situations. For these, you can individually apply the SetEffect to specific sounds or sound categories. Essentially, this feature is built upon using SetEffect.
