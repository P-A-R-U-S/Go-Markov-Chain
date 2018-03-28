# Go-Markov-Chain [![License](https://img.shields.io/dub/l/vibe-d.svg)](https://opensource.org/licenses/MIT) [![Go Report Card](https://goreportcard.com/badge/github.com/P-A-R-U-S/Go-Markov-Chain)](https://goreportcard.com/report/github.com/P-A-R-U-S/Go-Markov-Chain) [![Travis-CI](https://travis-ci.org/P-A-R-U-S/Go-Markov-Chain.svg?branch=master)](https://travis-ci.org/P-A-R-U-S/Go-Markov-Chain)
A Markov chain algorithm generates text by creating a statistical model of potential textual suffixes for a given prefix.

# Example

``
    c := NewChain(2) // Words in Links
	c.Build(strings.NewReader("One fish two fish red fish blue fish))
	text := c.Generate(250) // Generate text.
	fmt.Println(text) 
``