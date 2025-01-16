# ttf-subset

Golang ttf subset library

## Summary

- Written on pure Go
- Require Go version >= 1.14

## Install

```plaintext
go get github.com/taofei-pro/ttf-subset
```

## Usage

```golang
package main

import (
  "fmt"
  "os"

  "github.com/taofei-pro/ttf-subset"
)

func main() {
  in, err := ioutil.ReadFile("./data/font.ttf")
	if err != nil {
		panic(err)
	}
  words := "hello world"
	content := ttfsubset.UTF8CutFont(in, words)
}
```
