# Variables

## Problem

You are required to complete the code to declare and initialize variables of different types in Golang.

## Requirements

- Basic knowledge of Golang syntax
- Familiarity with variable declaration and initialization in Golang

## Example

```sh
$ go run variables.go
initial
1 2
true
0
apple
```

## Solution

```go
// In Go, _variables_ are explicitly declared and used by
// the compiler to e.g. check type-correctness of function
// calls.

package main

import "fmt"

func main() {

	// `var` declares 1 or more variables.
	var a = "initial"
	fmt.Println(a)

	// You can declare multiple variables at once.
	var b, c int = 1, 2
	fmt.Println(b, c)

	// Go will infer the type of initialized variables.
	var d = true
	fmt.Println(d)

	// Variables declared without a corresponding
	// initialization are _zero-valued_. For example, the
	// zero value for an `int` is `0`.
	var e int
	fmt.Println(e)

	// The `:=` syntax is shorthand for declaring and
	// initializing a variable, e.g. for
	// `var f string = "apple"` in this case.
	// This syntax is only available inside functions.
	f := "apple"
	fmt.Println(f)
}

```
