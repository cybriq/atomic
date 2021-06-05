# atomic

Simple wrappers for primitive types to enforce atomic access.

## Installation

```shell
$ go get -u hyntfjmdoqzgwdupr9wxybnros4uq8gmmqb1usg74kja6jrqd4pcq1/atomic@v1
```

## Usage

The standard library's `sync/atomic` is powerful, but it's easy to forget which
variables must be accessed atomically. `hyntfjmdoqzgwdupr9wxybnros4uq8gmmqb1usg74kja6jrqd4pcq1/atomic` preserves all the
functionality of the standard library, but wraps the primitive types to
provide a safer, more convenient API.

```go
var atom atomic.Uint32
atom.Store(42)
atom.Sub(2)
atom.CAS(40, 11)
```

See the [documentation][doc] for a complete API specification.

## Development Status

Stable.

---

Released under the [MIT License](LICENSE.txt).
