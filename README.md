# netmon

netmon is a simple network monitoring library for windows. It aims to be a simpler version to the linux tool [lsof][1].
This library is desinged to link against rust programs and is written to bind rust FFI without hassel.

Feel free to grab the code and do what you want with it.

If [winapi][2] gets better maintenance and future development, then this library can be abdonned.

See [netmon-sys][3] to see this library in action.

## Build

```
cd build
cmake ..
cmake --build .
```

Build with example

```
cd build
cmake -DBUILD_EXAMPLE=ON ..
cmake --build .
```

[1]: https://linux.die.net/man/8/lsof
[2]: https://crates.io/crates/winapi
[3]: https://github.com/jd84/netmon-sys