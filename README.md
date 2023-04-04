![dogo logo](assets/Dogo.png)
[![Go Reference](https://pkg.go.dev/badge/github.com/XotoX1337/dogo.svg)](https://pkg.go.dev/github.com/XotoX1337/dogo)
[![Go Report Card](https://goreportcard.com/badge/github.com/XotoX1337/dogo)](https://goreportcard.com/report/github.com/XotoX1337/dogo)

docker (compose) command line helper with autocomplete written in [go](https://go.dev/) and [cobra](https://github.com/spf13/cobra)

## Install

```shell
go install github.com/XotoX1337/dogo@latest
```

## Usage 
```shell
Usage:
  dogo [command]

Available Commands:
  completion  Generate completion script
  exec        execute a command in a running container
  help        Help about any command
  list        list all containers & services
  remove      remove one or many containers
  shell       connect to a running container
  start       start one or many containers
  stop        stop one or many containers
```
## Examples
    dogo shell yourContainer
    dogo start firstContainer secondContainer ...

## Completion

To generate a completion file simply run 

```shell
dogo completion bash -f
```


this will store the completion script in `$HOME/.bash_completion.d/dogo-completion.sh`.

After that you only need to source this file in your profile

