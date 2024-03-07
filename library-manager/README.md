---
description: Library Manager 是你建立並發揮創意的起點，你可以在這裡放入需要的AudioClip，定義播放時的行為與表現。
cover: ../.gitbook/assets/LibraryManager.png
coverY: 331.33953834698434
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Library Manager

BroAudio聲音資料庫主要由兩個資料結構所構成，他們分別是Asset以及Entity，兩者的關係如下圖：

<figure><img src="../.gitbook/assets/DataStructure.png" alt=""><figcaption></figcaption></figure>

**Asset**代表一系列Entity的集合，你可以將較常被一起使用的聲音都放在同一個Asset裡，如上圖你可以看到，所有Player相關的聲音都被存放在Player這個Asset之中。

目前各個Asset之間僅有名字的差異，所以區分方式並沒有任何的限制。不過未來將會有針對記憶體優化的更新，聲音資源的載入將會使用Asset來區分，詳見：



**Entity**就代表一個聲音，當他被指定播放時，只會播放在ClipList當中的其中一個AudioClip。我們將在這裡設置他該播放哪一個AudioClip、如何被播放、以及播放時會有什麼樣的表現。

#### AudioID

當entity在LibraryManager被建立時，會自動產生一組AudioID，你可以在任何需要使用這個Entity的script，使用\[SerializedField]來將AudioID顯示在Inspector，再使用dropdown menu來指定他。

[see how to do this in action](../getting-started.md#declare-an-audioid-and-use-broaudio.play-to-play-it)

###



##
