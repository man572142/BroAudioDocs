---
cover: >-
  https://images.unsplash.com/photo-1516865674991-9bb4878e3476?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHx2b2x1bWV8ZW58MHx8fHwxNzA0Mjc3ODc2fDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# Volume Control

## Volume Range

In BroAudio, every sound plays through the [Audio Mixer](audio-mixer.md), with a volume range of 0 to 10 (-80dB to +20dB). This is **20dB more** than what [Audio Source](https://docs.unity3d.com/Manual/class-AudioSource.html) offers, meaning you can produce sounds louder than the original files. This feature helps you to easily adjust and balance the overall volume.

## Editor Slider

The volume slider is based on decibel value; it's a logarithmic slider instead of a linear slider like [Audio Source](https://docs.unity3d.com/Manual/class-AudioSource.html)'s volume. This matches human sound perception better and allows for easier fine-tuning.

To further ensure precision, most audio software, including [Unity Audio Mixer](https://docs.unity3d.com/Manual/AudioMixer.html), features custom scale settings. Below is a comparison of different slider types, with each measured in decibels(dB) :

<figure><img src="../.gitbook/assets/Slider difference.PNG" alt=""><figcaption></figcaption></figure>

* \-6dB ≒ 0.5 volume (half volume), -20dB ≒ 0.1 volume, [Decibel(dB) Wikipedia](https://en.wikipedia.org/wiki/Decibel)

