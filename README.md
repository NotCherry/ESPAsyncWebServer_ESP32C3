# ESPAsyncWebServer

This is fork of [me-no-dev/ESP Async WebServer](https://registry.platformio.org/libraries/me-no-dev/ESP%20Async%20WebServer)

Changing exactly one line in `AsyncWebSocket.cpp:832`

from:

```cpp
return IPAddress(0U);
```

to:

```cpp
return IPAddress((uint32_t) 0u);
```

Fixing compile error.
