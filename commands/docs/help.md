---
title: help
categories: |
  core
version: 0.84.0
core: |
  Display help information about different parts of Nushell.
usage: |
  Display help information about different parts of Nushell.
---

# <code>{{ $frontmatter.title }}</code> for core

<div class='command-title'>{{ $frontmatter.core }}</div>

## Signature

```> help ...rest --find```

## Parameters

 -  `...rest`: the name of command, alias or module to get help on
 -  `--find {string}`: string to find in command names, usage, and search terms


## Input/output types:

| input   | output |
| ------- | ------ |
| nothing | string |

## Examples

show help for single command, alias, or module
```shell
> help match

```

show help for single sub-command, alias, or module
```shell
> help str lpad

```

search for string in command names, usage and search terms
```shell
> help --find char

```

## Notes
`help word` searches for "word" in commands, aliases and modules, in that order.

## Subcommands:

| name                                                 | type    | usage                           |
| ---------------------------------------------------- | ------- | ------------------------------- |
| [`help aliases`](/commands/docs/help_aliases.md)     | Builtin | Show help on nushell aliases.   |
| [`help commands`](/commands/docs/help_commands.md)   | Builtin | Show help on nushell commands.  |
| [`help externs`](/commands/docs/help_externs.md)     | Builtin | Show help on nushell externs.   |
| [`help modules`](/commands/docs/help_modules.md)     | Builtin | Show help on nushell modules.   |
| [`help operators`](/commands/docs/help_operators.md) | Builtin | Show help on nushell operators. |