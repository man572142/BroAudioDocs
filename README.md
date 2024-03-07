---
cover: >-
  https://images.unsplash.com/photo-1548504769-900b70ed122e?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw0fHxvcmFuZ2V8ZW58MHx8fHwxNzAzNDgwNjc1fDA&ixlib=rb-4.0.3&q=85
coverY: 0
layout:
  cover:
    visible: true
    size: full
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Introduction

## **What is BroAudio ?**

BroAudio is a **sound management** and **playback system** designed for Unity. It's unique in its focus on [sound quality](./#why-is-this-tool-related-to-sound-quality) and a [developer-friendly](./#what-does-developer-friendly-mean-in-this-tool) experience. You can create extensive and captivating audio systems without the need for mastering complex middleware like FMOD or Wwise. Whether you're part of a large team or a solo developer, achieving the goals becomes effortless and efficient with BroAudio.



### Why is this tool related to sound quality?

Indeed, apart from issues like noise and distortion that need to be repaired, there is no objective method to enhance sound quality. However, a playback system still holds significant impact over the quality of sound. This is because the loss of sound quality is relatively easy to occur and hard to avoid.

Here are some common issues listed along with how BroAudio addresses them:

| Issues                                                         | Bro's Solutions                                                                  |
| -------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| Distortion caused by playing multiple sounds simultaneously    | Well-designed mixer and auto-ducking on the master track                         |
| [Comb Filtering](bro-wiki/audio-terminology.md#comb-filtering) | Preventing rapid repetition of the same sound                                    |
| Unbalanced volume levels                                       | Full range (-80dB to +20dB) and highly adaptable real-time volume control system |
| Unnatural volume changes in Fade In, Fade Out and CrossFade    | Utilizing AudioMixer for volume control                                          |



### What does Developer-Friendly mean in this tool?

BroAudio aims to minimize the amount of information presented to developers. This means that by default, you will only see a few commonly used features, while other functions dynamically appear in the UI interface as you interact. You won't be overwhelmed by a large number of rarely used, or even completely unfamiliar settings and parameters.

What's even better is that BroAudio allows you to customize the GUI layout. You can set and select the parameters you want to display in _**Tools/BroAudio/Settings**_**.**



## Main Features

* Fade In/Out and Cross Fade with multiple ease function
* Seamless Loop
* Random Playback (with weight), Sequential Playback
* Clip Editor for permanent clip editing
* Dynamic audio effect
* Enhanced Volume Control Range (up to +20dB)
* Customizable GUI settings
* Visualized waveform and playback lines
* Write code in just one line
* and more…
