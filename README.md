# Custom-Links
_Original plugin by [nushnush](https://github.com/nushnush/Custom-Links)_

Create custom links for players using MOTD! Extended with support for custom server page rendering.

[Original AlliedModders thread.](https://forums.alliedmods.net/showthread.php?t=328328) See below for updated configuration options.

## Configuration
In `links.cfg` in `sourcemod/configs`, the commands and their links can be set up. Each command must be set up with at least the required properties described below.

| Property | Required | Description |
|----------|----------|-------------|
| `command` | Yes | The name of the command to use. If it takes the `sm_<name>`, then it can be called with `!<name>` or `/<name>` in chat. |
| `link` | Yes | The URL you want to link to. It must begin with `http://` or `https://`. |
| `custom` | No | Set to `1` to use custom server page rendering<sup>1</sup>. |

<sup>1</sup>_When using custom server page rendering, TF2 will show the webpage in full screen and skip showing map information after pressing continue._

See [`sourcemod/configs/links.cfg`](sourcemod/configs/links.cfg) for an example.
