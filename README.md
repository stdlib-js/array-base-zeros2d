<!--

@license Apache-2.0

Copyright (c) 2023 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# zeros2d

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Create a zero-filled two-dimensional nested array.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->

<section class="installation">

## Installation

```bash
npm install @stdlib/array-base-zeros2d
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var zeros2d = require( '@stdlib/array-base-zeros2d' );
```

#### zeros2d( shape )

Returns a zero-filled two-dimensional nested array.

```javascript
var out = zeros2d( [ 2, 3 ] );
// returns [ [ 0.0, 0.0, 0.0 ], [ 0.0, 0.0, 0.0 ] ]
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var gfill = require( '@stdlib/blas-ext-base-gfill' );
var zeros2d = require( '@stdlib/array-base-zeros2d' );

// Create a zero-filled array:
var arr = zeros2d( [ 5, 10 ] );

// Fill nested arrays with the same value...
gfill( arr[ 0 ].length, 1.0, arr[ 0 ], 1 );
gfill( arr[ 1 ].length, 2.0, arr[ 1 ], 1 );
gfill( arr[ 2 ].length, 3.0, arr[ 2 ], 1 );
gfill( arr[ 3 ].length, 4.0, arr[ 3 ], 1 );
gfill( arr[ 4 ].length, 5.0, arr[ 4 ], 1 );

console.log( arr );
// => [ [ 1.0, 1.0, ... ], [ 2.0, 2.0, ... ], [ 3.0, 3.0, ... ], [ 4.0, 4.0, ... ], [ 5.0, 5.0, ... ] ]
```

</section>

<!-- /.examples -->

<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/array-base/zeros`][@stdlib/array/base/zeros]</span><span class="delimiter">: </span><span class="description">create a zero-filled generic array.</span>
-   <span class="package-name">[`@stdlib/array-base/ones2d`][@stdlib/array/base/ones2d]</span><span class="delimiter">: </span><span class="description">create a two-dimensional nested array filled with ones.</span>
-   <span class="package-name">[`@stdlib/array-base/zeros3d`][@stdlib/array/base/zeros3d]</span><span class="delimiter">: </span><span class="description">create a zero-filled three-dimensional nested array.</span>
-   <span class="package-name">[`@stdlib/array-base/zeros4d`][@stdlib/array/base/zeros4d]</span><span class="delimiter">: </span><span class="description">create a zero-filled four-dimensional nested array.</span>
-   <span class="package-name">[`@stdlib/array-base/zeros5d`][@stdlib/array/base/zeros5d]</span><span class="delimiter">: </span><span class="description">create a zero-filled five-dimensional nested array.</span>
-   <span class="package-name">[`@stdlib/array-base/zerosnd`][@stdlib/array/base/zerosnd]</span><span class="delimiter">: </span><span class="description">create a zero-filled n-dimensional nested array.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2025. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/array-base-zeros2d.svg
[npm-url]: https://npmjs.org/package/@stdlib/array-base-zeros2d

[test-image]: https://github.com/stdlib-js/array-base-zeros2d/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/array-base-zeros2d/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/array-base-zeros2d/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/array-base-zeros2d?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/array-base-zeros2d.svg
[dependencies-url]: https://david-dm.org/stdlib-js/array-base-zeros2d/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/array-base-zeros2d/tree/deno
[deno-readme]: https://github.com/stdlib-js/array-base-zeros2d/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/array-base-zeros2d/tree/umd
[umd-readme]: https://github.com/stdlib-js/array-base-zeros2d/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/array-base-zeros2d/tree/esm
[esm-readme]: https://github.com/stdlib-js/array-base-zeros2d/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/array-base-zeros2d/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/array-base-zeros2d/main/LICENSE

<!-- <related-links> -->

[@stdlib/array/base/zeros]: https://github.com/stdlib-js/array-base-zeros

[@stdlib/array/base/ones2d]: https://github.com/stdlib-js/array-base-ones2d

[@stdlib/array/base/zeros3d]: https://github.com/stdlib-js/array-base-zeros3d

[@stdlib/array/base/zeros4d]: https://github.com/stdlib-js/array-base-zeros4d

[@stdlib/array/base/zeros5d]: https://github.com/stdlib-js/array-base-zeros5d

[@stdlib/array/base/zerosnd]: https://github.com/stdlib-js/array-base-zerosnd

<!-- </related-links> -->

</section>

<!-- /.links -->
