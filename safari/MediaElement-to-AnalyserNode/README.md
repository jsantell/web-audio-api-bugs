# All Analyser Node methods do not update when using Media Element source in Safari 6
## Apple Problem ID #12400561

* Works in Chrome v21, fails in Safari 6/iOS6
* Fails in Safari 6
* Fails in iOS6

When using a [MediaElementAudioSource](https://dvcs.w3.org/hg/audio/raw-file/tip/webaudio/specification.html#MediaElementAudioSourceNode-section) node and connecting to a [RealtimeAnalyserNode](https://dvcs.w3.org/hg/audio/raw-file/tip/webaudio/specification.html#RealtimeAnalyserNode), the analyser node's methods `getByteFrequencyData`, `getFloatFrequencyData` and `getByteTimeDomainData` do not change as the audio progresses.

This works as intended when using a different source, such as an oscillator or AudioBuffer.
