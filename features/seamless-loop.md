---
cover: >-
  https://images.unsplash.com/photo-1702360373665-af7bf9766ab4?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHJhbmRvbXx8fHx8fHx8fDE3MDQyNzc4MjR8&ixlib=rb-4.0.3&q=85
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

# Seamless Loop

Looping allows an [AudioClip](https://docs.unity3d.com/Manual/class-AudioClip.html) to be continuously replayed. It's a common technique used for playing sounds like **Music** and **Ambience** in games. However, if a sound is not specifically designed for looping, its beginning and end might not match seamlessly. Direct replay would result in a noticeable change.

This is where **SeamlessLoop** comes in. It enables an [AudioClip](https://docs.unity3d.com/Manual/class-AudioClip.html) to start playing again on a new audio track just before the current one finishes. By gradually [cross-fading](fade-in-out-and-cross-fade.md#crossfade) between the two tracks, it creates an illusion that the sound never stops at all.

### **How To Use?**

You can find the looping options in the "Settings" tab of an AudioEntity.

[<mark style="color:blue;"><p style="text-align: right;">Didn't see the option?</p></mark>](#user-content-fn-1)[^1]

&#x20;

<figure><img src="../.gitbook/assets/SeamlessLoop.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
If you can't see this option, it might be because the GUI setting of this AudioType is set to be invisible. Click here for more details.
{% endhint %}



\


[^1]: If you can't see this option, it might be because the GUI setting of this AudioType is set to be invisible. Click here for more details.
