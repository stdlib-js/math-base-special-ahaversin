<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

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

# Archaversine

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [inverse half-value versed sine][archaversine].

<section class="intro">

The [inverse half-value versed sine][archaversine] is defined as

<!-- <equation class="equation" label="eq:archaversine" align="center" raw="\operatorname{ahaversin}(\theta) = 2 \cdot \arcsin(\sqrt{\theta})" alt="Inverse half-value versed sine."> -->

<div class="equation" align="center" data-raw-text="\operatorname{ahaversin}(\theta) = 2 \cdot \arcsin(\sqrt{\theta})" data-equation="eq:archaversine">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@bb29798906e119fcb2af99e94b60407a270c9b32/lib/node_modules/@stdlib/math/base/special/ahaversin/docs/img/equation_archaversine.svg" alt="Inverse half-value versed sine.">
    <br>
</div>

<!-- </equation> -->

</section>

<!-- /.intro -->



<section class="usage">

## Usage

To use in Observable,

```javascript
ahaversin = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-ahaversin@umd/bundle.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-ahaversin@umd/bundle.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.ahaversin;
})();
</script>
```

#### ahaversin( x )

Computes the [inverse half-value versed sine][archaversine].

```javascript
var v = ahaversin( 0.0 );
// returns 0.0

v = ahaversin( 1.0 );
// returns ~3.1416

v = ahaversin( 0.5 );
// returns ~1.5708
```

If `x < 0`, `x > 1`, or `x` is `NaN`, the function returns `NaN`.

```javascript
var v = ahaversin( 1.5 );
// returns NaN

v = ahaversin( -3.14 );
// returns NaN

v = ahaversin( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/array-base-linspace@umd/bundle.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-ahaversin@umd/bundle.js"></script>
<script type="text/javascript">
(function () {

var x = linspace( 0.0, 1.0, 100 );

var i;
for ( i = 0; i < x.length; i++ ) {
    console.log( ahaversin( x[ i ] ) );
}

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math/base/special/ahavercos`][@stdlib/math/base/special/ahavercos]</span><span class="delimiter">: </span><span class="description">compute the inverse half-value versed cosine.</span>
-   <span class="package-name">[`@stdlib/math/base/special/haversin`][@stdlib/math/base/special/haversin]</span><span class="delimiter">: </span><span class="description">compute the half-value versed sine.</span>
-   <span class="package-name">[`@stdlib/math/base/special/versin`][@stdlib/math/base/special/versin]</span><span class="delimiter">: </span><span class="description">compute the versed sine.</span>

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

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-ahaversin.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-ahaversin

[test-image]: https://github.com/stdlib-js/math-base-special-ahaversin/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-ahaversin/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-ahaversin/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-ahaversin?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-ahaversin.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-ahaversin/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-ahaversin/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-ahaversin/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-ahaversin/tree/esm

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-ahaversin/main/LICENSE

[archaversine]: https://en.wikipedia.org/wiki/Versine

<!-- <related-links> -->

[@stdlib/math/base/special/ahavercos]: https://github.com/stdlib-js/math-base-special-ahavercos/tree/umd

[@stdlib/math/base/special/haversin]: https://github.com/stdlib-js/math-base-special-haversin/tree/umd

[@stdlib/math/base/special/versin]: https://github.com/stdlib-js/math-base-special-versin/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
