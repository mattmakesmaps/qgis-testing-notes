# QGIS Unit Tests

## Building QGIS

See [INSTALL docs](https://htmlpreview.github.io/?https://raw.github.com/qgis/QGIS/master/doc/INSTALL.html#toc3).

Additional ccmake flags set were:

```
CMAKE_BUILD_TYPE=Debug
CMAKE_INSTALL_PREFIX=/home/matt/Projects/apps
BUILD_TESTING=ON
ENABLE_COVERAGE=ON
ENABLE_TESTS=ON
```

After running `ccmake -G Ninja ..`, ran `ninja` to build.

## Executing Tests

See [/tests/README.md](https://github.com/qgis/QGIS/blob/master/tests/README.md)

- List all tests: from `build-master`: `ctest --show-only`

- Execute a specific test, verbose output: `ctest -V -R qgsgeometrycheckstest`
