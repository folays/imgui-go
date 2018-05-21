# Dear ImGui for Go

This library is a [Go](https://www.golang.org) wrapper for [Dear ImGui](https://github.com/ocornut/imgui).

At the moment, this wrapper is a special-purpose wrapper for use within InkyBlackness.
However, it is self-contained and can be used for other purposes as well.

This wrapper is
* hand-crafted, for Go
* documented
* versioned
* with a ported example using [GLFW3](https://github.com/go-gl/glfw) and [OpenGL3](https://github.com/go-gl/gl).

## Version philosophy
This library does not mirror the versions of the wrapped ImGui. The semantic versioning of this wrapper is defined as:
* Major changes: (Breaking) changes in API or behaviour. Typically done through changes in ImGui.
* Minor changes: Extensions in API. Typically done through small version increments of ImGui and/or exposing further features in a compatible way.
* Patch changes: Bug fixes - either in the wrapper or the wrapped ImGui, given that the API & behaviour remains the same.

At the moment, this library uses version [1.61](https://github.com/ocornut/imgui/releases/tag/v1.61) of ImGui.

## Alternatives

Before this project was created, the following alternatives were considered - and ignored:
* [kdrag0n/go-imgui](https://github.com/kdrag0n/go-imgui). Reasons for dismissal:
  * Auto-generated bloat, which doesn't help
  * Old API (1.5x)
  * Does not compile (Issues [1](https://github.com/kdrag0n/go-imgui/issues/1) and [3](https://github.com/kdrag0n/go-imgui/issues/3))
  * Project appears to be abandoned
* [Extrawurst/cimgui](https://github.com/Extrawurst/cimgui). Reasons for dismissal:
  * Old API (1.5x), 1.6x attempted, in-progress, could not be used
  * Appears to still semi-expose the C++ API, especially through the structures
  * Adding this adds another dependency


## License

The project is available under the terms of the **New BSD License** (see LICENSE file).
The licenses of included sources are stored in the **_licenses** folder.
