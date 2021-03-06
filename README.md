[![Go Reference](https://pkg.go.dev/badge/github.com/iwdgo/htmlutils.svg)](https://pkg.go.dev/github.com/iwdgo/htmlutils)
[![Go Report Card](https://goreportcard.com/badge/github.com/iwdgo/htmlutils)](https://goreportcard.com/report/github.com/iwdgo/htmlutils)
[![codecov](https://codecov.io/gh/iWdGo/htmlutils/branch/master/graph/badge.svg)](https://codecov.io/gh/iWdGo/htmlutils)

[![Build Status](https://travis-ci.com/iWdGo/htmlutils.svg?branch=master)](https://travis-ci.com/iWdGo/htmlutils)
[![Build Status](https://api.cirrus-ci.com/github/iWdGo/htmlutils.svg)](https://cirrus-ci.com/github/iWdGo/htmlutils)
[![Build status](https://ci.appveyor.com/api/projects/status/v6ce70t0jmqgehpw?svg=true)](https://ci.appveyor.com/project/iWdGo/htmlutils)
![Build status](https://github.com/iwdgo/htmlutils/workflows/Go/badge.svg)

# Exploring html.Node trees

html.Node trees as parsed using [golang.org/x/net/html](https://godoc.org/golang.org/x/net/html).

The module provides basic functionality to compare HTML tags or html.Node and their trees.
The search of an HTML tag using a *node.HTML type ignores pointers.
It always returns the first match. By ignoring some properties, tags `<button>` are easy to count.
Text value of a tag (title, error message,...) can be checked.

# Good to know

Parsing is not a complete syntax checker of HTML.
For instance, tags that may be omitted like `<p>` would fail a comparison.

Siblings must always have the same order or comparison fails.
Order of attributes is treated as irrelevant.

# How to start

Detailed [documentation](https://pkg.go.dev/github.com/iwdgo/htmlutils) includes examples.
