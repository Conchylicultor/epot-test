# Changelog

## [Unreleased]

* `epath`:
  * Add `epath.testing.mock_epath` to mock GCS calls.
* `epy.testing`:
  * Add `epy.testing.subtest` for better subtests support.
  * Add `epy.testing.non_hermetic` to mark non-hermetic tests.

## [0.5.1] - 2022-05-04

* `array_utils`:
  * Now has a `__all__` to allow `from etils.array_types import *`
  * `FloatArray` and `IntArray` have dtype to `np.float32` and `np.int32`
* `ecolab`:
  * Add `with ecolab.adhoc():`contextmanager for dynamic code import.
  * More `ecolab.lazy_imports`
* `enp`:
  * Add `enp.linalg` alias of `enp.compat`
  * `enp.testing.parametrize_xnp` now has a `restrict` kwarg
* `epy`:
  * `StrEnum` is now case-insensitive

### Other

* asdasd

## [0.5.0] - 2022-03-23

* `enp`:
  * Expose `enp.lazy` to the public API to help design code compatible
  with `jax`, `np`, `tf`
  * Add `enp.compat` for ops compatibles with both TF, Jax, Np
  * Add `enp.tau` [constant](https://tauday.com/)
  * Add `enp.testing.parametrize_xnp` fixture to test a function with both
    `jax`, `tf`, `np`
  * Add `enp.testing.set_tnp` fixture to activate tf numpy mode.
* `ecolab`:
  * Add `from etils.ecolab.lazy_imports import *` to lazy-import common
  Python modules
  * Rename `ecolab.display_array_as_img` -> `ecolab.auto_plot_array`
  * `ecolab.auto_plot_array` now supports multi-images & video.
* `etree`: Add `assert_same_structure` on the backend
* `epy`: Add `epy.zip_dict`

## [0.4.0] - 2022-02-03

* `edc`: Dataclasses utils
* `etree`:
  * `etree.spec_like`: Inspect a nested structure
* `enp`:
  * `enp.interp`: Scale arrays
  * `enp.normalize_bytes2str`: Normalize `str` arrays
* `ecolab`:
    * Replace `ecolab.collapse_xyz()` by unified `ecolab.collapse()`

## [0.3.3] - 2021-01-07

* Add text utils:
  * `epy.Lines`
  * `epy.dedent`

## [0.3.2] - 2022-01-04

* Automated github release

[Unreleased]: https://github.com/google/etils/compare/v0.5.1...HEAD
[0.5.1]: https://github.com/google/etils/compare/v0.5.0...v0.5.1
[0.5.0]: https://github.com/google/etils/compare/v0.4.0...v0.5.0
[0.4.0]: https://github.com/google/etils/compare/v0.3.3...0.4.0
[0.3.3]: https://github.com/google/etils/compare/v0.3.2...v0.3.3
[0.3.2]: https://github.com/google/etils/releases/tag/v0.3.2
