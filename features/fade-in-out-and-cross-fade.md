---
cover: >-
  https://images.unsplash.com/photo-1514241516423-6c0a5e031aa2?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxzdW5yaXNlfGVufDB8fHx8MTcwNDI3ODEyN3ww&ixlib=rb-4.0.3&q=85
coverY: -5.960294117647059
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

# Fade In/Out and Cross Fade

## Fade In/Out

淡出淡入是使播放體驗能夠更加平滑流暢的技術，你除了可以在LibraryManager為每一個AudioClip設置淡出淡入以外，還有包括SetVolume()及SetEffect()等API，都有提供float型態的fadeTime多載，讓這些效果能更自然的被enabled and disabled。

## Cross Fade

Crossfading in audio is the technique of smoothly transitioning from one sound to another by gradually decreasing the volume of the first sound while simultaneously increasing the volume of the second.
