# tantalizing-client

Client builds for the Tantalizing server. Players don't need anything from this page except the launcher.

## Players
1. Download **TantalizingLauncher-windows.zip** from the [latest release](https://github.com/bcoll1493/tantalizing-client/releases/latest) and unzip it anywhere.
2. Run **TantalizingLauncher.exe**. Java is built in. Windows may show a SmartScreen warning because the launcher isn't code-signed yet: click "More info", then "Run anyway".

The launcher downloads the client, checks its SHA-256, and starts it.

## Publishing a new client (staff)
Every release has `client.jar` and `client.properties`:
```
url=https://github.com/bcoll1493/tantalizing-client/releases/download/<tag>/client.jar
sha256=<sha256 of client.jar>
host=<server address>
```
The launcher always reads `client.properties` from the **latest** release. A new release with a new jar and manifest updates every player on their next launch. Old releases can stay.
