A little RCON cli based on james4k's RCON library for golang.

## Building on Mac

```sh
brew install goreleaser
goreleaser
```

## Installation

1. Download the appropriate binary for your platform from the [latest releases](https://github.com/itzg/rcon-cli/releases/latest)

2. On UNIX-y platforms, set the binary to be executable

Done.

## Usage

```text
rcon-cli is a CLI for attaching to an RCON enabled game server, such as Minecraft.
Without any additional arguments, the CLI will start an interactive session with
the RCON server.

If arguments are passed into the CLI, then the arguments are sent
as a single command (joined by spaces), the response is displayed,
and the CLI will exit.

Usage:
  rcon-cli [flags] [RCON command ...]

Examples:

rcon-cli --host mc1 --port 25575
rcon-cli --port 25575 stop
RCON_PORT=25575 rcon-cli stop


Flags:
      --config string     config file (default is $HOME/.rcon-cli.yaml)
      --host string       RCON server's hostname (default "localhost")
      --password string   RCON server's password
      --port int          Server's RCON port (default 27015)
```
