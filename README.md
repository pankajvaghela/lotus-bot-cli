# Lotus-bot-cli (LotBot)

LotusBot CLI

<!-- toc -->

- [Usage](#usage)
- [Commands](#commands)
<!-- tocstop -->

# Usage

<!-- usage -->

```sh-session
$ npm install -g lotus-bot-cli
$ lotbot COMMAND
running command...
$ lotbot (--version)
lotus-bot-cli/0.0.0 darwin-arm64 node-v16.15.0
$ lotbot --help [COMMAND]
USAGE
  $ lotbot COMMAND
...
```

<!-- usagestop -->

# Commands

<!-- commands -->

- [`lotbot help [COMMAND]`](#lotbot-help-command)
- [`lotbot plugins`](#lotbot-plugins)
- [`lotbot plugins:install PLUGIN...`](#lotbot-pluginsinstall-plugin)
- [`lotbot plugins:inspect PLUGIN...`](#lotbot-pluginsinspect-plugin)
- [`lotbot plugins:install PLUGIN...`](#lotbot-pluginsinstall-plugin-1)
- [`lotbot plugins:link PLUGIN`](#lotbot-pluginslink-plugin)
- [`lotbot plugins:uninstall PLUGIN...`](#lotbot-pluginsuninstall-plugin)
- [`lotbot plugins:uninstall PLUGIN...`](#lotbot-pluginsuninstall-plugin-1)
- [`lotbot plugins:uninstall PLUGIN...`](#lotbot-pluginsuninstall-plugin-2)
- [`lotbot plugins update`](#lotbot-plugins-update)

## `lotbot help [COMMAND]`

Display help for lotbot.

```
USAGE
  $ lotbot help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for lotbot.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.10/src/commands/help.ts)_

## `lotbot plugins`

List installed plugins.

```
USAGE
  $ lotbot plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ lotbot plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `lotbot plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ lotbot plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ lotbot plugins add

EXAMPLES
  $ lotbot plugins:install myplugin

  $ lotbot plugins:install https://github.com/someuser/someplugin

  $ lotbot plugins:install someuser/someplugin
```

## `lotbot plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ lotbot plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ lotbot plugins:inspect myplugin
```

## `lotbot plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ lotbot plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ lotbot plugins add

EXAMPLES
  $ lotbot plugins:install myplugin

  $ lotbot plugins:install https://github.com/someuser/someplugin

  $ lotbot plugins:install someuser/someplugin
```

## `lotbot plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ lotbot plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ lotbot plugins:link myplugin
```

## `lotbot plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ lotbot plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ lotbot plugins unlink
  $ lotbot plugins remove
```

## `lotbot plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ lotbot plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ lotbot plugins unlink
  $ lotbot plugins remove
```

## `lotbot plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ lotbot plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ lotbot plugins unlink
  $ lotbot plugins remove
```

## `lotbot plugins update`

Update installed plugins.

```
USAGE
  $ lotbot plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

<!-- commandsstop -->
