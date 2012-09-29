# AudioNodes do not alter audio from MediaElementAudioSource
## Apple Problem ID #12400564

* Works in Chrome v21, fails in Safari 6/iOS6
* Fails in Safari 6
* Fails in iOS6

When using a [MediaElementAudioSource](https://dvcs.w3.org/hg/audio/raw-file/tip/webaudio/specification.html#MediaElementAudioSourceNode-section) node and connecting to an AudioNode, there is no change in audio, as if the AudioNode is being circumvented.

As per the [spec for createMediaElementSource](https://dvcs.w3.org/hg/audio/raw-file/tip/webaudio/specification.html#methodsandparams-AudioContext):

_As a consequence of calling this method, audio playback from the HTMLMediaElement will be re-routed into the processing graph of the AudioContext._

This works fine when using a different source, such as an oscillator or an AudioBuffer.
