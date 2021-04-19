# t

less portable, stripped down version of [tag](https://github.com/aykamko/tag),
also uses a larger (64MiB vs 64KiB) buffer for readline.

[![License](https://img.shields.io/github/license/seankhliao/t.svg?style=flat-square)](LICENSE)
![Version](https://img.shields.io/github/v/tag/seankhliao/t?sort=semver&style=flat-square)
[![Go Reference](https://pkg.go.dev/badge/go.seankhliao.com/fin.svg)](https://pkg.go.dev/go.seankhliao.com/t)

## install

```go
go install go.seankhliao.com/t@latest
```

requires ripgrep

```zsh
function t() {
    command t -i "$@"
    source /tmp/t_aliases 2>/dev/null
}
```

## usage

```sh
$ t func
main.go
[1] 18:1:func main() {

README.md
[2] 14:1:function t() {

# opens first link with nvim
$ e1
```

## todo

- [ ] replace `bufio.Reader` with https://godoc.org/golang.org/x/text/transform
