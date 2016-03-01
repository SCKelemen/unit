# About

[![Travis-CI](https://api.travis-ci.org/martinlindhe/unit.svg)](https://travis-ci.org/martinlindhe/unit)
[![GoDoc](https://godoc.org/github.com/martinlindhe/unit?status.svg)](https://godoc.org/github.com/martinlindhe/unit)

Conversion of unit library for golang

Uses float64 math, so is fast but not so accurate


# Installation

```
go get -u github.com/martinlindhe/unit
```


# General use

```go
ft := 1 * unit.Feet

fmt.Println("in meters", ft.Meters())
```


# Temperature

Cannot be used to scale directly like the other units, instead, use the From* functions:

```go
c := unit.FromFahrenheit(100).Celsius())
```


# License

Under [MIT](LICENSE)