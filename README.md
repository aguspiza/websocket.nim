# websocket.nim

A websocket library for nim, providing both client and server support.

This is a pre-release and not final software. There might be bugs,
unintended side-effects, the API might change without warning between releases,
and features are missing - namely:

 * A robust RNG for the client data masking

See [the API docs](http://niv.github.io/websocket.nim/docs/0.3.0/websocket.html) for usage instructions.

You will get an error about masking server data if you do not define websocketUnmaskedByDefault.

```nim
nim  c --define:websocketUnmaskedByDefault myserverapp.nim
```
