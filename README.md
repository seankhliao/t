# t

[![pkg.go.dev](http://img.shields.io/badge/godoc-reference-blue.svg?style=flat-square)](https://pkg.go.dev/go.seankhliao.com/t)
![Version](https://img.shields.io/github/v/tag/seankhliao/t?sort=semver&style=flat-square)
[![License](https://img.shields.io/github/license/seankhliao/t.svg?style=flat-square)](LICENSE)

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

less portable, stripped down version of [tag](https://github.com/aykamko/tag),
also uses a larger (64MiB vs 64KiB) buffer for readline.

TODO: replace bufio.Reader with https://godoc.org/golang.org/x/text/transform
