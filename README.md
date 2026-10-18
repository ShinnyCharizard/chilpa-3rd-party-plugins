# Chilpa 3rd-party plugins

This catalog, maintained by [vicrodh](https://github.com/vicrodh), lists
independently published plugins that use Chilpa's native plugin API. It is
separate from [Chilpa's official catalog](https://github.com/vicrodh/chilpa-plugins).
Listed plugins are **third-party, with Chilpa verification and validation**.
Inclusion here does not make them official plugins or imply affiliation with a
service provider. Validation evidence accompanies each listed release.

## Install

Add this URL in **Settings > Plugins** using **Add**:

```text
https://raw.githubusercontent.com/vicrodh/chilpa-3rd-party-plugins/main/index.json
```

Chilpa reads the catalog alongside the official one. Select **Install**, review
the requested permissions and enable the plugin. Adding a catalog does not
automatically install or enable its plugins. Each download has a SHA-256 checksum.

## Plugins

| Plugin | Author | Source and downloads | Platform | Requirements |
| --- | --- | --- | --- | --- |
| Tidal | [vicrodh](https://github.com/vicrodh) | [chilpa-pg-tidal](https://github.com/vicrodh/chilpa-pg-tidal) | Linux x86_64 | Chilpa 0.1.0-beta; a Tidal account with a subscription for full playback. |
| Spotify | [vicrodh](https://github.com/vicrodh) | [chilpa-pg-spotify](https://github.com/vicrodh/chilpa-pg-spotify) | Linux x86_64 / macOS Apple Silicon | A host with native process support; Premium for playback; personal Client ID recommended. |

The Tidal plugin is independent of the service provider and retains its
GPL-3.0-or-later license.
It provides library browsing, search, discovery, playlists and playback through
its own account connection. Account credentials remain in the plugin's private
data; its README describes storage, permissions and playback limits.

The Spotify plugin is independently published under MIT. Its README and
bundled licenses credit Carmine Paolino's Spotifast. It is also a working example in the SDK's
[native process guide](https://github.com/vicrodh/chilpa-plugins-sdk/blob/main/wiki/Native-Plugins.md#native-source-example).
Its separate Web and playback approvals, quotas, account storage and tested
platform limits are documented in the plugin repository.

## Catalog format

The native version-1 JSON catalog records a plugin ID, author, repository,
version, API range, immutable versioned release URL and SHA-256. A package
can be listed only after that exact archive is published and checked. The catalog itself is MIT
licensed; individual plugins keep their own licenses.

## Independent repositories

Plugin authors can
host a version-1 `index.json` in a separate repository and distribute its URL
directly. Chilpa can add that URL alongside this catalog and the official one.
Those releases do not carry this catalog's Chilpa validation. They still need
valid SDK manifests, supported runtimes and permissions, compatible API versions
and matching package checksums to install and run.

The public [SDK and authoring documentation](https://github.com/vicrodh/chilpa-plugins-sdk)
defines the plugin contract. Submission rules and a detailed independent-repository
guide are not yet available.
