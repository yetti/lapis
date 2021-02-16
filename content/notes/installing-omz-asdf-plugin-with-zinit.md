---
title: Installing OMZ ASDF plugin with zinit
date: 2020-11-14T04:16:19.681Z
---
Installing OMZ asdf plugin with zinit requires loading bashcompinit before the plugin is loaded to avoid `command not found: complete` error. 

e.g.

```
autoload -Uz bashcompinit && bashcompinit
zinit snippet OMZ::plugins/asdf/asdf.plugin.zsh
```