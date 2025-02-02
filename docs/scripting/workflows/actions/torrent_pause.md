# `TorrentPause`

The `TorrentPause` action pauses a torrent. It waits until libtorrent has
actually paused the torrent before continuing.

:::info
If the torrent is auto managed by libtorrent, it will most likely be resumed
soon after pausing due to how queueing in libtorrent works.

This action makes the most sense if you use the `TorrentFlag` action and unset
`auto_managed` before pausing.
:::

## Inputs

_This action has no inputs_.

## Usage

```lua
local TorrentPause = require "porla.actions.TorrentPause"
```

### Example

```lua
TorrentPause:new{}
```
