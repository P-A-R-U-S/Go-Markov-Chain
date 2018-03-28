# Markov Chain Algorithm [![License](https://img.shields.io/dub/l/vibe-d.svg)](https://opensource.org/licenses/MIT) [![Go Report Card](https://goreportcard.com/badge/github.com/P-A-R-U-S/Go-Markov-Chain)](https://goreportcard.com/report/github.com/P-A-R-U-S/Go-Markov-Chain) [![Travis-CI](https://travis-ci.org/P-A-R-U-S/Go-Markov-Chain.svg?branch=master)](https://travis-ci.org/P-A-R-U-S/Go-Markov-Chain) [![Get help on Codementor](https://cdn.codementor.io/badges/get_help_github.svg)](https://www.codementor.io/parus) 

A Markov chain algorithm optimized by memory consumption generates text by creating a statistical model of potential textual Suffixes for a given Links.

# Example

```GO
    c := NewChain(2) // Words per Links 
    c.Build(strings.NewReader("One fish two fish red fish blue fish))"
    text := c.Generate(250) // Generate text. 
    fmt.Println(text) 
```