# ScriptProcessorNode requires an output to call audioprocess event

## [Chromium Bug #349831](https://code.google.com/p/chromium/issues/detail?id=349831)

When using a ScriptProcessorNode, an output is required to be connected ultimately to the destination. This works on Firefox, fails in webkit implementations.

* **Works**: Firefox 26
* **Fails**: Chrome 33, 35
* **Fails**: Safari 6.1

Example prints to textarea on `onaudioprocess` call.
