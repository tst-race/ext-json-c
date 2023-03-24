# JSON-C for RACE

This repo provides scripts to custom-build the
[JSON-C library](https://github.com/json-c/json-c) for RACE.

## License

The JSON-C library is licensed under the MIT license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

JSON-C has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build JSON-C.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-json-c.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-json-c
```

## Platforms

JSON-C is built for the following platforms:

* `android-x86_64`
* `android-arm64-v8a`

It is also used on Linux but can be installed via `apt`.

## How It Is Used

JSON-C is used by slothy.
