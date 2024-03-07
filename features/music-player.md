---
cover: >-
  https://images.unsplash.com/photo-1534224039826-c7a0eda0e6b3?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw2fHx0cmFuc2l0aW9ufGVufDB8fHx8MTcwNDI3ODA4OHww&ixlib=rb-4.0.3&q=85
coverY: 0
---

# Music Player

MusicPlayer讓你可以輕易地在不同BGM之間切換並自然過渡，每當玩家到了新的場景，或者觸發了特定的劇情，你可以使用`BroAudio.Play().AsBGM()`讓音樂以MusicPlayer的方式播放。

MusicPlayer與一般播放器的不同之處在於

1\. 同一時間只會播放一個ID的聲音 (除了過渡期間以外)

2\. 當你呼叫BroAudio.Play().AsBGM()時，他將會自動從前一個使用這個API的音樂，以指定的Transition設定過渡



### SetTransition(TimeTransition, fadeTime)

你可以指定Transition類型以及過渡的時間長度。當你沒有指定FadeTime的時候，系統將會採用該聲音(Entity)在LibraryManager中的FadeIn及FadeOut設定；反之，則會忽略(或者說複寫)。

Transition類型分別有

* Default: 先FadeOut再FadeIn
* Immediate: 立即停止現在的聲音，並馬上播放新的，不做任何過渡。
* OnlyFadeIn : 立即停止現在的聲音，但使用新的聲音在LibraryManager中設置的FadeIn
* OnlyFadeOut : 使用現在聲音的LibraryManager設定FadeOut，完成後馬上播放新的聲音
* CorssFade : 在前段聲音開始FadeOut時就播放下一段聲音並進行FadeIn

FadeTime, Transiton以及Entity在LibraryManager的設定是會互相影響的，其規則是:\
除非使用Transition.Immediate(ignore all fadeTime)，否則FadeTime的優先度最高，若沒有設置則採用Entity上的FadeIn/Out，最後再看Transition的模式。

#### 以下表格的配置其結果都等同於Transition.Immediate，也就是無任何過渡

| Entity FadeIn | Entity FadeOut | Transition  | FadeTime |
| ------------- | -------------- | ----------- | -------- |
| 0             | 0              | Default     | Not set  |
| 2             | 2              | CrossFade   | 0        |
| 2             | 2              | Immediate   | 2        |
| 0             | 2              | OnlyFadeIn  | Not Set  |
| 2             | 0              | OnlyFadeOut | NotSet   |

