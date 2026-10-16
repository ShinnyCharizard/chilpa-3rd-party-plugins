# Chilpa 3rd-party plugins

I maintain this catalog as [vicrodh](https://github.com/vicrodh) for independently
published plugins that use Chilpa's native plugin API. I keep it separate from
[Chilpa's official catalog](https://github.com/vicrodh/chilpa-plugins).
I list these plugins as **third-party, with Chilpa verification and validation**.
Inclusion here does not make them official plugins or imply affiliation with a
service provider. I publish the validation evidence with each listed release.

## Install

I add this URL in **Settings > Plugins** using **Add**:

```text
https://raw.githubusercontent.com/vicrodh/chilpa-3rd-party-plugins/main/index.json
```

Chilpa reads the catalog alongside the official one. I select **Install**, review
the requested permissions and enable the plugin. Adding a catalog does not
automatically install or enable its plugins. Each download has a SHA-256 checksum.

## Plugins

| Plugin | Author | Source and downloads | Platform | Requirements |
| --- | --- | --- | --- | --- |
| Tidal | [vicrodh](https://github.com/vicrodh) | [chilpa-pg-tidal](https://github.com/vicrodh/chilpa-pg-tidal) | Linux x86_64 | Chilpa 0.1.0-beta; a Tidal account with a subscription for full playback. |

I publish Tidal independently of Tidal and retain its GPL-3.0-or-later license.
It provides library browsing, search, discovery, playlists and playback through
its own account connection. Account credentials remain in the plugin's private
data; its README describes storage, permissions and playback limits.

## Catalog format

I use the native version-1 JSON catalog: a plugin ID, author, repository, version,
API range, immutable versioned release URL and SHA-256. I list a package only
after publishing and checking that exact archive. The catalog itself is MIT
licensed; individual plugins keep their own licenses.

## Independent repositories

I do not require plugin authors to publish through this catalog. An author can
host a version-1 `index.json` in a separate repository and distribute its URL
directly. Chilpa can add that URL alongside this catalog and the official one.
Those releases do not carry this catalog's Chilpa validation. They still need
valid SDK manifests, supported runtimes and permissions, compatible API versions
and matching package checksums to install and run.

I use the public [SDK and authoring documentation](https://github.com/vicrodh/chilpa-plugins-sdk)
for the plugin contract. Submission rules and the detailed independent-repository
guide are being prepared separately.
