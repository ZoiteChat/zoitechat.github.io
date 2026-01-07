---
layout: post
title: "Flatpak known issue: Python plugin freeze"
---

If ZoiteChat appears to “hang” right after you select a network and press **Connect**, and you’re using the Flatpak build, it’s very likely the Python plugin.

### Workarounds

- Run without any plugins:

  ```
  zoitechat --no-plugins
  ```

- Or disable just the Python plugin (when the UI is available), then restart.

### Status

This is a known packaging/runtime bug we’re tracking and plan to fix.

If you want to help debug it, grab a log:

```
G_MESSAGES_DEBUG=all flatpak run io.github.Zoitechat
```
