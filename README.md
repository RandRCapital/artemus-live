# artemus-live

Where The Artemus's online test server is right now. The game reads `server.json` when a player opens **Online**, so
nobody types a server address. It is updated whenever the test server starts or stops.

`server.json` holds only the public address players connect to (no credentials):

```json
{ "status": "online", "host": "xxxx.pr.edgegap.net", "port": 30881, "updated": "2026-10-22T00:00:00Z" }
```

When no server is running, `status` is `offline` and the game tells players to try again later.
