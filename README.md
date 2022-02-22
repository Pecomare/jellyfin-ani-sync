<h1>Ani-Sync Jellyfin Plugin</h1>

## About

Ani-Sync lets you synchorinze your Jellyfin Anime watch progress to popular services (currently only MyAnimeList is supported, please [create an issue](https://github.com/vosmiic/jellyfin-ani-sync/issues/new) if you have a different provider you would like to be supported).

## Installation

[See the official Jellyfin documentation for install instructions](https://jellyfin.org/docs/general/server/plugins/index.html#installing).

1. Download a version from the [releases tab](https://github.com/vosmiic/jellyfin-ani-sync/releases) that matches your Jellyfin version.
2. Copy the `meta.json` and `jellyfin-ani-sync.dll` files into `plugins/ani-sync` (see above official documentation on where to find the `plugins` folder).
3. Restart your Jellyfin instance.
4. Navigate to Plugins in Jellyfin (Settings > Admin Dashboard > Plugins).
5. Adjust the settings accordingly. I would advise following the detailed instructions on the [wiki page](https://github.com/vosmiic/jellyfin-ani-sync/wiki).

## Build

1. To build this plugin you will need [.Net 6.x](https://dotnet.microsoft.com/download/dotnet/6.0).

2. Build plugin with following command
  ```
  dotnet publish --configuration Release --output bin
  ```

3. Place the dll-file in the `plugins/ani-sync` folder (you might need to create the folders) of your JF install

## Services/providers
### Currently supported
1. MyAnimeList
### In-progress
1. Kitsu
2. [Your suggestion](https://github.com/vosmiic/jellyfin-ani-sync/issues/new)

## In progress

The current list of unsupported features (that are being worked on):
1. OVAs. Attempting to find them via the API is mildly difficult and unreliable, so they are currently not supported.
2. Other providers/services. Any suggestions as to which providers the plugin should be extended to support is appreciated (click [here](https://github.com/vosmiic/jellyfin-ani-sync/issues/new) to request a new provider). 