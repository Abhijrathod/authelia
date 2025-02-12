---
title: "authelia config template"
description: "Reference for the authelia config template command."
lead: ""
date: 2023-09-20T05:30:57+10:00
draft: false
images: []
menu:
  reference:
    parent: "cli-authelia"
weight: 905
toc: true
---

## authelia config template

Template a configuration file or files with enabled filters

### Synopsis

Template a configuration file or files with enabled filters.

This subcommand allows debugging the filtered YAML files with any of the available filters. It should be noted this
command needs to be executed with the same environment variables and working path as when normally running Authelia to
be useful.

```
authelia config template [flags]
```

### Examples

```
authelia config template --fitlers.experimental.template
authelia config template --fitlers.experimental.expand-env --config config.yml
```

### Options

```
  -h, --help   help for template
```

### Options inherited from parent commands

```
  -c, --config strings                        configuration files or directories to load, for more information run 'authelia -h authelia config' (default [configuration.yml])
      --config.experimental.filters strings   list of filters to apply to all configuration files, for more information run 'authelia -h authelia filters'
```

### SEE ALSO

* [authelia config](authelia_config.md)	 - Perform config related actions

