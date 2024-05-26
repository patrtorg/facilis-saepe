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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# ndarray

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Multidimensional arrays.

<section class="installation">

## Installation

```bash
npm install @patrtorg/facilis-saepe
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
var ns = require( '@patrtorg/facilis-saepe' );
```

#### ns

ndarray namespace.

```javascript
var o = ns;
// returns {...}
```

The namespace exports the following functions to create multidimensional arrays:

<!-- <toc pattern="+(array|ctor)"> -->

<div class="namespace-toc">

-   <span class="signature">[`array( [buffer,] [options] )`][@patrtorg/facilis-saepe/array]</span><span class="delimiter">: </span><span class="description">create a multidimensional array.</span>
-   <span class="signature">[`ndarray( dtype, buffer, shape, strides, offset, order[, options] )`][@patrtorg/facilis-saepe/ctor]</span><span class="delimiter">: </span><span class="description">multidimensional array constructor.</span>

</div>

<!-- </toc> -->

The namespace contains the following sub-namespaces:

<!-- <toc pattern="+(base|iter)"> -->

<div class="namespace-toc">

-   <span class="signature">[`base`][@patrtorg/facilis-saepe/base]</span><span class="delimiter">: </span><span class="description">base ndarray.</span>
-   <span class="signature">[`iter`][@patrtorg/facilis-saepe/iter]</span><span class="delimiter">: </span><span class="description">multidimensional array iterators.</span>

</div>

<!-- </toc> -->

In addition, the namespace contains the following multidimensional array utility functions:

<!-- <toc pattern="*" > -->

<div class="namespace-toc">

-   <span class="signature">[`at( x[, ...indices] )`][@patrtorg/facilis-saepe/at]</span><span class="delimiter">: </span><span class="description">return an `ndarray` element.</span>
-   <span class="signature">[`broadcastArray( x, shape )`][@patrtorg/facilis-saepe/broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape.</span>
-   <span class="signature">[`broadcastArrays( ...arrays )`][@patrtorg/facilis-saepe/broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`castingModes()`][@patrtorg/facilis-saepe/casting-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray casting modes.</span>
-   <span class="signature">[`dataBuffer( x )`][@patrtorg/facilis-saepe/data-buffer]</span><span class="delimiter">: </span><span class="description">return the underlying data buffer of a provided ndarray.</span>
-   <span class="signature">[`defaults()`][@patrtorg/facilis-saepe/defaults]</span><span class="delimiter">: </span><span class="description">default ndarray settings.</span>
-   <span class="signature">[`dispatch( fcns, types, data, nargs, nin, nout )`][@patrtorg/facilis-saepe/dispatch]</span><span class="delimiter">: </span><span class="description">create an ndarray function interface which performs multiple dispatch.</span>
-   <span class="signature">[`dtype( x )`][@patrtorg/facilis-saepe/dtype]</span><span class="delimiter">: </span><span class="description">return the data type of a provided ndarray.</span>
-   <span class="signature">[`dtypes( [kind] )`][@patrtorg/facilis-saepe/dtypes]</span><span class="delimiter">: </span><span class="description">list of ndarray data types.</span>
-   <span class="signature">[`emptyLike( x[, options] )`][@patrtorg/facilis-saepe/empty-like]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`empty( shape[, options] )`][@patrtorg/facilis-saepe/empty]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having a specified shape and data type.</span>
-   <span class="signature">[`FancyArray( dtype, buffer, shape, strides, offset, order[, options] )`][@patrtorg/facilis-saepe/fancy]</span><span class="delimiter">: </span><span class="description">fancy multidimensional array constructor.</span>
-   <span class="signature">[`flag( x, name )`][@patrtorg/facilis-saepe/flag]</span><span class="delimiter">: </span><span class="description">return a specified flag for a provided ndarray.</span>
-   <span class="signature">[`flags( x )`][@patrtorg/facilis-saepe/flags]</span><span class="delimiter">: </span><span class="description">return the flags of a provided ndarray.</span>
-   <span class="signature">[`scalar2ndarray( value[, options] )`][@patrtorg/facilis-saepe/from-scalar]</span><span class="delimiter">: </span><span class="description">convert a scalar value to a zero-dimensional ndarray.</span>
-   <span class="signature">[`ind2sub( shape, idx[, options] )`][@patrtorg/facilis-saepe/ind2sub]</span><span class="delimiter">: </span><span class="description">convert a linear index to an array of subscripts.</span>
-   <span class="signature">[`indexModes()`][@patrtorg/facilis-saepe/index-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray index modes.</span>
-   <span class="signature">[`maybeBroadcastArray( x, shape )`][@patrtorg/facilis-saepe/maybe-broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape if and only if the specified shape differs from the provided ndarray's shape.</span>
-   <span class="signature">[`maybeBroadcastArrays( arrays )`][@patrtorg/facilis-saepe/maybe-broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`minDataType( value )`][@patrtorg/facilis-saepe/min-dtype]</span><span class="delimiter">: </span><span class="description">determine the minimum ndarray data type of the closest "kind" necessary for storing a provided scalar value.</span>
-   <span class="signature">[`mostlySafeCasts( [dtype] )`][@patrtorg/facilis-saepe/mostly-safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast and, for floating-point data types, can be downcast.</span>
-   <span class="signature">[`ndims( x )`][@patrtorg/facilis-saepe/ndims]</span><span class="delimiter">: </span><span class="description">return the number of ndarray dimensions.</span>
-   <span class="signature">[`nextDataType( [dtype] )`][@patrtorg/facilis-saepe/next-dtype]</span><span class="delimiter">: </span><span class="description">return the next larger ndarray data type of the same kind.</span>
-   <span class="signature">[`numelDimension( x, dim )`][@patrtorg/facilis-saepe/numel-dimension]</span><span class="delimiter">: </span><span class="description">return the size (i.e., number of elements) of a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`numel( x )`][@patrtorg/facilis-saepe/numel]</span><span class="delimiter">: </span><span class="description">return the number of elements in an ndarray.</span>
-   <span class="signature">[`offset( x )`][@patrtorg/facilis-saepe/offset]</span><span class="delimiter">: </span><span class="description">return the index offset specifying the underlying buffer index of the first iterated ndarray element.</span>
-   <span class="signature">[`order( x )`][@patrtorg/facilis-saepe/order]</span><span class="delimiter">: </span><span class="description">return the layout order of a provided ndarray.</span>
-   <span class="signature">[`orders()`][@patrtorg/facilis-saepe/orders]</span><span class="delimiter">: </span><span class="description">list of ndarray orders.</span>
-   <span class="signature">[`outputDataTypePolicies()`][@patrtorg/facilis-saepe/output-dtype-policies]</span><span class="delimiter">: </span><span class="description">list of output ndarray data type policies.</span>
-   <span class="signature">[`promotionRules( [dtype1, dtype2] )`][@patrtorg/facilis-saepe/promotion-rules]</span><span class="delimiter">: </span><span class="description">return the ndarray data type with the smallest size and closest "kind" to which ndarray data types can be **safely** cast.</span>
-   <span class="signature">[`safeCasts( [dtype] )`][@patrtorg/facilis-saepe/safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast.</span>
-   <span class="signature">[`sameKindCasts( [dtype] )`][@patrtorg/facilis-saepe/same-kind-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast or cast within the same "kind".</span>
-   <span class="signature">[`shape( x )`][@patrtorg/facilis-saepe/shape]</span><span class="delimiter">: </span><span class="description">return the shape of a provided ndarray.</span>
-   <span class="signature">[`sliceAssign( x, y, ...s[, options] )`][@patrtorg/facilis-saepe/slice-assign]</span><span class="delimiter">: </span><span class="description">assign element values from a broadcasted input `ndarray` to corresponding elements in an output `ndarray` view.</span>
-   <span class="signature">[`sliceDimensionFrom( x, dim, start[, options] )`][@patrtorg/facilis-saepe/slice-dimension-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimensionTo( x, dim, stop[, options] )`][@patrtorg/facilis-saepe/slice-dimension-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimension( x, dim, slice[, options] )`][@patrtorg/facilis-saepe/slice-dimension]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray` when sliced along a specified dimension.</span>
-   <span class="signature">[`sliceFrom( x, ...start[, options] )`][@patrtorg/facilis-saepe/slice-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input ndarray.</span>
-   <span class="signature">[`sliceTo( x, ...stop[, options] )`][@patrtorg/facilis-saepe/slice-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input ndarray.</span>
-   <span class="signature">[`slice( x, ...s[, options] )`][@patrtorg/facilis-saepe/slice]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray`.</span>
-   <span class="signature">[`stride( x, dim )`][@patrtorg/facilis-saepe/stride]</span><span class="delimiter">: </span><span class="description">return the stride along a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`strides( x )`][@patrtorg/facilis-saepe/strides]</span><span class="delimiter">: </span><span class="description">return the strides of a provided ndarray.</span>
-   <span class="signature">[`sub2ind( shape, ...subscripts[, options] )`][@patrtorg/facilis-saepe/sub2ind]</span><span class="delimiter">: </span><span class="description">convert subscripts to a linear index.</span>
-   <span class="signature">[`ndarray2array( x )`][@patrtorg/facilis-saepe/to-array]</span><span class="delimiter">: </span><span class="description">convert an ndarray to a generic array.</span>
-   <span class="signature">[`zerosLike( x[, options] )`][@patrtorg/facilis-saepe/zeros-like]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`zeros( shape[, options] )`][@patrtorg/facilis-saepe/zeros]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having a specified shape and data type.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var ns = require( '@patrtorg/facilis-saepe' );

console.log( objectKeys( ns ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@patrtorg/facilis-saepe.svg
[npm-url]: https://npmjs.org/package/@patrtorg/facilis-saepe

[test-image]: https://github.com/patrtorg/facilis-saepe/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/patrtorg/facilis-saepe/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/patrtorg/facilis-saepe/main.svg
[coverage-url]: https://codecov.io/github/patrtorg/facilis-saepe?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/patrtorg/facilis-saepe.svg
[dependencies-url]: https://david-dm.org/patrtorg/facilis-saepe/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/patrtorg/facilis-saepe/tree/deno
[deno-readme]: https://github.com/patrtorg/facilis-saepe/blob/deno/README.md
[umd-url]: https://github.com/patrtorg/facilis-saepe/tree/umd
[umd-readme]: https://github.com/patrtorg/facilis-saepe/blob/umd/README.md
[esm-url]: https://github.com/patrtorg/facilis-saepe/tree/esm
[esm-readme]: https://github.com/patrtorg/facilis-saepe/blob/esm/README.md
[branches-url]: https://github.com/patrtorg/facilis-saepe/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/patrtorg/facilis-saepe/main/LICENSE

<!-- <toc-links> -->

[@patrtorg/facilis-saepe/at]: https://github.com/patrtorg/facilis-saepe/tree/main/at

[@patrtorg/facilis-saepe/broadcast-array]: https://github.com/patrtorg/facilis-saepe/tree/main/broadcast-array

[@patrtorg/facilis-saepe/broadcast-arrays]: https://github.com/patrtorg/facilis-saepe/tree/main/broadcast-arrays

[@patrtorg/facilis-saepe/casting-modes]: https://github.com/patrtorg/facilis-saepe/tree/main/casting-modes

[@patrtorg/facilis-saepe/data-buffer]: https://github.com/patrtorg/facilis-saepe/tree/main/data-buffer

[@patrtorg/facilis-saepe/defaults]: https://github.com/patrtorg/facilis-saepe/tree/main/defaults

[@patrtorg/facilis-saepe/dispatch]: https://github.com/patrtorg/facilis-saepe/tree/main/dispatch

[@patrtorg/facilis-saepe/dtype]: https://github.com/patrtorg/facilis-saepe/tree/main/dtype

[@patrtorg/facilis-saepe/dtypes]: https://github.com/patrtorg/facilis-saepe/tree/main/dtypes

[@patrtorg/facilis-saepe/empty-like]: https://github.com/patrtorg/facilis-saepe/tree/main/empty-like

[@patrtorg/facilis-saepe/empty]: https://github.com/patrtorg/facilis-saepe/tree/main/empty

[@patrtorg/facilis-saepe/fancy]: https://github.com/patrtorg/facilis-saepe/tree/main/fancy

[@patrtorg/facilis-saepe/flag]: https://github.com/patrtorg/facilis-saepe/tree/main/flag

[@patrtorg/facilis-saepe/flags]: https://github.com/patrtorg/facilis-saepe/tree/main/flags

[@patrtorg/facilis-saepe/from-scalar]: https://github.com/patrtorg/facilis-saepe/tree/main/from-scalar

[@patrtorg/facilis-saepe/ind2sub]: https://github.com/patrtorg/facilis-saepe/tree/main/ind2sub

[@patrtorg/facilis-saepe/index-modes]: https://github.com/patrtorg/facilis-saepe/tree/main/index-modes

[@patrtorg/facilis-saepe/maybe-broadcast-array]: https://github.com/patrtorg/facilis-saepe/tree/main/maybe-broadcast-array

[@patrtorg/facilis-saepe/maybe-broadcast-arrays]: https://github.com/patrtorg/facilis-saepe/tree/main/maybe-broadcast-arrays

[@patrtorg/facilis-saepe/min-dtype]: https://github.com/patrtorg/facilis-saepe/tree/main/min-dtype

[@patrtorg/facilis-saepe/mostly-safe-casts]: https://github.com/patrtorg/facilis-saepe/tree/main/mostly-safe-casts

[@patrtorg/facilis-saepe/ndims]: https://github.com/patrtorg/facilis-saepe/tree/main/ndims

[@patrtorg/facilis-saepe/next-dtype]: https://github.com/patrtorg/facilis-saepe/tree/main/next-dtype

[@patrtorg/facilis-saepe/numel-dimension]: https://github.com/patrtorg/facilis-saepe/tree/main/numel-dimension

[@patrtorg/facilis-saepe/numel]: https://github.com/patrtorg/facilis-saepe/tree/main/numel

[@patrtorg/facilis-saepe/offset]: https://github.com/patrtorg/facilis-saepe/tree/main/offset

[@patrtorg/facilis-saepe/order]: https://github.com/patrtorg/facilis-saepe/tree/main/order

[@patrtorg/facilis-saepe/orders]: https://github.com/patrtorg/facilis-saepe/tree/main/orders

[@patrtorg/facilis-saepe/output-dtype-policies]: https://github.com/patrtorg/facilis-saepe/tree/main/output-dtype-policies

[@patrtorg/facilis-saepe/promotion-rules]: https://github.com/patrtorg/facilis-saepe/tree/main/promotion-rules

[@patrtorg/facilis-saepe/safe-casts]: https://github.com/patrtorg/facilis-saepe/tree/main/safe-casts

[@patrtorg/facilis-saepe/same-kind-casts]: https://github.com/patrtorg/facilis-saepe/tree/main/same-kind-casts

[@patrtorg/facilis-saepe/shape]: https://github.com/patrtorg/facilis-saepe/tree/main/shape

[@patrtorg/facilis-saepe/slice-assign]: https://github.com/patrtorg/facilis-saepe/tree/main/slice-assign

[@patrtorg/facilis-saepe/slice-dimension-from]: https://github.com/patrtorg/facilis-saepe/tree/main/slice-dimension-from

[@patrtorg/facilis-saepe/slice-dimension-to]: https://github.com/patrtorg/facilis-saepe/tree/main/slice-dimension-to

[@patrtorg/facilis-saepe/slice-dimension]: https://github.com/patrtorg/facilis-saepe/tree/main/slice-dimension

[@patrtorg/facilis-saepe/slice-from]: https://github.com/patrtorg/facilis-saepe/tree/main/slice-from

[@patrtorg/facilis-saepe/slice-to]: https://github.com/patrtorg/facilis-saepe/tree/main/slice-to

[@patrtorg/facilis-saepe/slice]: https://github.com/patrtorg/facilis-saepe/tree/main/slice

[@patrtorg/facilis-saepe/stride]: https://github.com/patrtorg/facilis-saepe/tree/main/stride

[@patrtorg/facilis-saepe/strides]: https://github.com/patrtorg/facilis-saepe/tree/main/strides

[@patrtorg/facilis-saepe/sub2ind]: https://github.com/patrtorg/facilis-saepe/tree/main/sub2ind

[@patrtorg/facilis-saepe/to-array]: https://github.com/patrtorg/facilis-saepe/tree/main/to-array

[@patrtorg/facilis-saepe/zeros-like]: https://github.com/patrtorg/facilis-saepe/tree/main/zeros-like

[@patrtorg/facilis-saepe/zeros]: https://github.com/patrtorg/facilis-saepe/tree/main/zeros

[@patrtorg/facilis-saepe/base]: https://github.com/patrtorg/facilis-saepe/tree/main/base

[@patrtorg/facilis-saepe/iter]: https://github.com/patrtorg/facilis-saepe/tree/main/iter

[@patrtorg/facilis-saepe/array]: https://github.com/patrtorg/facilis-saepe/tree/main/array

[@patrtorg/facilis-saepe/ctor]: https://github.com/patrtorg/facilis-saepe/tree/main/ctor

<!-- </toc-links> -->

</section>

<!-- /.links -->
