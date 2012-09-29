* Works in Chrome v21, fails in Safari 6/iOS6
* Fails in Safari 6
* Fails in iOS6

When using a [MediaElementAudioSource](https://dvcs.w3.org/hg/audio/raw-file/tip/webaudio/specification.html#MediaElementAudioSourceNode-section) node and connecting to a [JavaScriptAudioNode](https://dvcs.w3.org/hg/audio/raw-file/tip/webaudio/specification.html#JavaScriptAudioNode-section), all elements in a channel array are `0`.

This works fine when using a different source, such as an oscillator or an AudioBuffer.
