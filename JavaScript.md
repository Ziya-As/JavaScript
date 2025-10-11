# JavaScript Cheatsheet

<hr>

- [JavaScript Cheatsheet](#javascript-cheatsheet)
  - [Useful Links](#useful-links)
  - [`use strict`](#use-strict)
  - [String Methods](#string-methods)
    - [Define a string and access characters](#define-a-string-and-access-characters)
    - [Turning the string into upper or lower case](#turning-the-string-into-upper-or-lower-case)
    - [`.length`](#length)
    - [`.indexOf()`](#indexof)
    - [`.lastIndexOf()`](#lastindexof)
    - [`.includes()`](#includes)
    - [`.startsWith()`, `.endsWith()`](#startswith-endswith)
    - [`.slice()`](#slice)
    - [`.substring()`](#substring)
    - [`.substr()`](#substr)
    - [`.split()`](#split)
    - [`.trim()`](#trim)
    - [Looping through strings](#looping-through-strings)
  - [Number Methods](#number-methods)
    - [`.toFixed()`](#tofixed)
    - [define numbers using `e`](#define-numbers-using-e)
    - [`isNaN()` and `Number.isNaN()`](#isnan-and-numberisnan)
    - [`isFinite()` and `Number.isFinite()`](#isfinite-and-numberisfinite)
    - [`Number.isInteger()`](#numberisinteger)
    - [`parseInt()` and `Number.parseInt()`](#parseint-and-numberparseint)
    - [`parseFloat()` and `Number.parseFloat()`](#parsefloat-and-numberparsefloat)
  - [Math Object](#math-object)
    - [`Math.random()`](#mathrandom)
    - [`Math.max()`](#mathmax)
    - [`Math.min()`](#mathmin)
    - [`Math.pow()`](#mathpow)
    - [`Math.PI`](#mathpi)
    - [`Math.trunc()`](#mathtrunc)
    - [`Math.round()`](#mathround)
    - [`Math.ceil()`](#mathceil)
    - [`Math.floor()`](#mathfloor)
    - [Supported Math Operations](#supported-math-operations)
  - [Type Conversion](#type-conversion)
    - [`String()`](#string)
    - [`Number()`](#number)
      - [`+` operator](#-operator)
    - [`Boolean()`](#boolean)
  - [Conditionals](#conditionals)
    - [`if()` on a single line](#if-on-a-single-line)
    - [`if()...else`](#ifelse)
    - [`if()...else if()...else`](#ifelse-ifelse)
    - [Ternary conditions](#ternary-conditions)
    - [`switch`](#switch)
  - [Loops](#loops)
    - [`while()`](#while)
    - [`while` with `break`](#while-with-break)
    - [`while()` loop on a single line](#while-loop-on-a-single-line)
    - [`do...while()`](#dowhile)
    - [`for()`](#for)
    - [Named `for` loop](#named-for-loop)
  - [Functions](#functions)
    - [Creating a function](#creating-a-function)
    - [Set a default value to a parameter in a function](#set-a-default-value-to-a-parameter-in-a-function)
    - [Access all arguments of a function](#access-all-arguments-of-a-function)
    - [Using the spread operator inside a function](#using-the-spread-operator-inside-a-function)
    - [Get the number of parameters of a function](#get-the-number-of-parameters-of-a-function)
    - [Returns from a function](#returns-from-a-function)
    - [Copying a function](#copying-a-function)
    - [Add a property to a function from outside](#add-a-property-to-a-function-from-outside)
    - [`setTimeout()` and `clearTimeout()`](#settimeout-and-cleartimeout)
    - [`setInterval()` and `clearInterval()`, and nested `setTimeout()`](#setinterval-and-clearinterval-and-nested-settimeout)
    - [`.call()`, `.apply()`, `.bind()`](#call-apply-bind)
    - [`eval()`](#eval)
    - [Currying](#currying)
  - [Objects](#objects)
    - [Creating an object](#creating-an-object)
    - [Object keys and values, and accessing them](#object-keys-and-values-and-accessing-them)
    - [Delete a key-value pair](#delete-a-key-value-pair)
    - [Test if a property exists in an object](#test-if-a-property-exists-in-an-object)
    - [Looping through object](#looping-through-object)
    - [Copy an object](#copy-an-object)
      - [`Object.assign()`](#objectassign)
      - [`structuredClone()`](#structuredclone)
    - [optional chaining `?.`](#optional-chaining-)
    - [`Object.fromEntries()`](#objectfromentries)
    - [`Object.keys()` and `Object.values()`](#objectkeys-and-objectvalues)
    - [`Object.entries()`](#objectentries)
    - [`Object.getOwnPropertyDescriptor()`](#objectgetownpropertydescriptor)
    - [`Object.getOwnPropertyDescriptors()`](#objectgetownpropertydescriptors)
    - [`Object.defineProperty`](#objectdefineproperty)
    - [`Object.defineProperties`](#objectdefineproperties)
    - [Copy an object together with all of its properties' flags](#copy-an-object-together-with-all-of-its-properties-flags)
    - [`Object.preventExtension()` and `Object.isExtensible()`](#objectpreventextension-and-objectisextensible)
    - [`Object.seal()` and `Object.isSealed()`](#objectseal-and-objectissealed)
    - [`Object.freeze()` and `Object.isFrozen()`](#objectfreeze-and-objectisfrozen)
    - [Accessor properties](#accessor-properties)
    - [Set the prototype of an object](#set-the-prototype-of-an-object)
    - [Add a method to a native prototype](#add-a-method-to-a-native-prototype)
    - [`.isPrototypeOf()`](#isprototypeof)
    - [Looping and prototypes](#looping-and-prototypes)
      - [`.hasOwnProperty()`](#hasownproperty)
      - [`Object.getOwnPropertyNames()`](#objectgetownpropertynames)
  - [Symbol](#symbol)
    - [Create a `Symbol()`](#create-a-symbol)
    - [`description` property](#description-property)
    - [Converting symbols to a string](#converting-symbols-to-a-string)
    - [Symbols in an object literal](#symbols-in-an-object-literal)
    - [Symbol properties and looping](#symbol-properties-and-looping)
    - [`Object.getOwnPropertySymbols()`](#objectgetownpropertysymbols)
    - [`Object.assign()` and symbols](#objectassign-and-symbols)
    - [`Symbol.for()`](#symbolfor)
    - [`Symbol.keyFor()`](#symbolkeyfor)
  - [Arrays](#arrays)
    - [Create an array](#create-an-array)
    - [Accessing array items](#accessing-array-items)
    - [Copy arrays with the spread operator](#copy-arrays-with-the-spread-operator)
    - [`.pop()`](#pop)
    - [`.push()`](#push)
    - [`.shift()`](#shift)
    - [`.unshift()`](#unshift)
    - [Return values of `.push()` and `.unshift()`](#return-values-of-push-and-unshift)
    - [Cutting out arrays with `.length`](#cutting-out-arrays-with-length)
    - [`.splice()`](#splice)
    - [`.concat()`](#concat)
    - [`.forEach()`](#foreach)
    - [`.indexOf()` and `.lastIndexOf`](#indexof-and-lastindexof)
    - [`.includes()`](#includes-1)
    - [`.find()`](#find)
    - [`.findIndex()` and `.findLastIndex`](#findindex-and-findlastindex)
    - [`.filter()`](#filter)
    - [`.map()`](#map)
    - [`.sort()`](#sort)
    - [`.toSorted()`](#tosorted)
    - [`.reverse()`](#reverse)
    - [`.toReversed()`](#toreversed)
    - [`.join()`](#join)
    - [`.reduce()`](#reduce)
    - [`.reduceRight()`](#reduceright)
    - [Higher order functions and `this`](#higher-order-functions-and-this)
    - [`Array.isArray()`](#arrayisarray)
    - [`.some()`](#some)
    - [`.every()`](#every)
    - [`Array.from()`](#arrayfrom)
    - [`.fill()`](#fill)
  - [Maps](#maps)
    - [Create a `Map`](#create-a-map)
    - [Add key-value pairs](#add-key-value-pairs)
    - [Get the value of a specific key](#get-the-value-of-a-specific-key)
    - [`.has()`](#has)
    - [`.size`](#size)
    - [`.keys()`](#keys)
    - [`.values()`](#values)
    - [`.entries()`](#entries)
    - [`.forEach()`](#foreach-1)
    - [`.delete()`](#delete)
    - [`.clear()`](#clear)
  - [WeakMaps](#weakmaps)
    - [Create a `WeakMap`](#create-a-weakmap)
    - [Add key-value pairs into a weakmap](#add-key-value-pairs-into-a-weakmap)
    - [Get the value of a specific key](#get-the-value-of-a-specific-key-1)
    - [`.has()`](#has-1)
    - [`.delete()`](#delete-1)
  - [Sets](#sets)
    - [Create a `Set`](#create-a-set)
    - [Add items to a set](#add-items-to-a-set)
    - [`.has()`](#has-2)
    - [`.size`](#size-1)
    - [Loop over the set items](#loop-over-the-set-items)
    - [`.forEach()`](#foreach-2)
    - [`.delete()`](#delete-2)
    - [`.clear()`](#clear-1)
  - [WeakSets](#weaksets)
    - [Create a `WeakSet`](#create-a-weakset)
    - [Add an item to a weakset](#add-an-item-to-a-weakset)
    - [`.has()`](#has-3)
    - [`.delete()`](#delete-3)
  - [Destructuring](#destructuring)
    - [Destructuring an array](#destructuring-an-array)
    - [Destructuring a string](#destructuring-a-string)
    - [Destructuring a set](#destructuring-a-set)
    - [Sawpping values using destructuring](#sawpping-values-using-destructuring)
    - [Destructuring an object](#destructuring-an-object)
  - [Date Object](#date-object)
    - [create a new `Date()`](#create-a-new-date)
    - [`Date.now()`](#datenow)
    - [`.getTime()`](#gettime)
    - [Setting a date using the `Date` object](#setting-a-date-using-the-date-object)
    - [Retrieve different parts of a date](#retrieve-different-parts-of-a-date)
    - [`.getTimezoneOffset()`](#gettimezoneoffset)
    - [Setting different parts of a date](#setting-different-parts-of-a-date)
    - [`Date.parse()`](#dateparse)
  - [JSON](#json)
    - [`JSON.stringify()`](#jsonstringify)
    - [`JSON.parse()`](#jsonparse)
  - [Classes](#classes)
    - [Define a class and create objects based on a class](#define-a-class-and-create-objects-based-on-a-class)
    - [Classes are functions](#classes-are-functions)
    - [Named class expressions](#named-class-expressions)
    - [getters/setters, and computed properties in classes](#getterssetters-and-computed-properties-in-classes)
    - [Class fields](#class-fields)
    - [Class inheritance](#class-inheritance)
    - [Override a method in a parent class](#override-a-method-in-a-parent-class)
    - [Extend the method in a parent class](#extend-the-method-in-a-parent-class)
    - [Static methods and properties](#static-methods-and-properties)
    - [Protected properties](#protected-properties)
    - [Private properties](#private-properties)
    - [Extend built-in classes](#extend-built-in-classes)
    - [`instanceof`](#instanceof)
    - [Mixin](#mixin)
  - [Error handling](#error-handling)
    - [`try...catch()`, and properties of an error object](#trycatch-and-properties-of-an-error-object)
    - [`try...catch()` and asynchronous code](#trycatch-and-asynchronous-code)
    - [`catch` without parentheses](#catch-without-parentheses)
    - [`throw` operator and different built-in error constructors](#throw-operator-and-different-built-in-error-constructors)
  - [Promises, async/await](#promises-asyncawait)
    - [Quick intro to promise](#quick-intro-to-promise)
    - [Internal properties of a returned promise object](#internal-properties-of-a-returned-promise-object)
    - [`.then` without catching the promise rejection](#then-without-catching-the-promise-rejection)
    - [Chained `then`s](#chained-thens)
    - [Controlling for errors using `.then`](#controlling-for-errors-using-then)
    - [`.then` after `.catch`](#then-after-catch)
    - [`finally`](#finally)
    - [A promise inside a promise](#a-promise-inside-a-promise)
    - [`Promise.all`](#promiseall)
    - [`Promise.allSettled`](#promiseallsettled)
    - [`Promise.race()`](#promiserace)
    - [`Promise.any`](#promiseany)
    - [`async`/`await`](#asyncawait)
  - [Generators](#generators)
    - [Intro to generators](#intro-to-generators)
    - [`next()`](#next)
    - [Looping over generators](#looping-over-generators)
    - [Spread syntax with generators](#spread-syntax-with-generators)
    - [Generator in a generator](#generator-in-a-generator)
    - [Passing an argument to a generator](#passing-an-argument-to-a-generator)
    - [Pass an error to the generator](#pass-an-error-to-the-generator)
    - [Finishing a generator early](#finishing-a-generator-early)
  - [Modules](#modules)
    - [`import.meta`](#importmeta)
    - [`this` in modules](#this-in-modules)
    - [Browser-specific differences of scripts with `type="module"`](#browser-specific-differences-of-scripts-with-typemodule)
    - [Fallback for old browsers](#fallback-for-old-browsers)
    - [Exporting and importing variables](#exporting-and-importing-variables)
      - [`export` while declaring a variable](#export-while-declaring-a-variable)
      - [`export` after declaring a variable](#export-after-declaring-a-variable)
      - [`import` by name](#import-by-name)
      - [`import` everything at once](#import-everything-at-once)
      - [`import` under different names](#import-under-different-names)
      - [`export` under different names](#export-under-different-names)
    - [`export default`](#export-default)
    - [Re-export](#re-export)
    - [Dynamic imports](#dynamic-imports)
  - [DOM](#dom)
    - [Accessing some topmost level tags on a webpage](#accessing-some-topmost-level-tags-on-a-webpage)
    - [Checking if an element or node has child nodes](#checking-if-an-element-or-node-has-child-nodes)
    - [Retrieving the collection of child nodes](#retrieving-the-collection-of-child-nodes)
    - [Accessing the child nodes](#accessing-the-child-nodes)
    - [Accessing the sibling nodes](#accessing-the-sibling-nodes)
    - [Accessing the parent node](#accessing-the-parent-node)
    - [Working with child elements](#working-with-child-elements)
    - [Accessing the child elements](#accessing-the-child-elements)
    - [Accessing the sibling elements](#accessing-the-sibling-elements)
    - [Accessing the parent element](#accessing-the-parent-element)
    - [Accessing the element by its `id`](#accessing-the-element-by-its-id)
    - [Table properties](#table-properties)
    - [Select elements using CSS selectors](#select-elements-using-css-selectors)
    - [Check if an element matches a CSS selector](#check-if-an-element-matches-a-css-selector)
    - [Select the nearest ancestor that matches a CSS selector](#select-the-nearest-ancestor-that-matches-a-css-selector)
    - [Select the HTML of an element](#select-the-html-of-an-element)
    - [Select the text of an element](#select-the-text-of-an-element)
    - [Retrieving the name of an HTML tag or node](#retrieving-the-name-of-an-html-tag-or-node)
    - [Hiding an HTML element](#hiding-an-html-element)
    - [Input properties](#input-properties)
    - [Anchor element's `href` property](#anchor-elements-href-property)
    - [Working with HTML tag attributes](#working-with-html-tag-attributes)
    - [The `style` object](#the-style-object)
    - [Retrieving the style information of an element](#retrieving-the-style-information-of-an-element)
    - [Working with Attributes starting with `data-`](#working-with-attributes-starting-with-data-)
    - [Creating an HTML element](#creating-an-html-element)
    - [Creating a text node](#creating-a-text-node)
    - [Adding elements to the DOM](#adding-elements-to-the-dom)
    - [Insert an HTML string with `<element>.insertAdjacentHTML(<where>, <html>)`](#insert-an-html-string-with-elementinsertadjacenthtmlwhere-html)
    - [Insert Text with `<element>.insertAdjacentText(<where>, <text>)`](#insert-text-with-elementinsertadjacenttextwhere-text)
    - [Remove a node from the DOM](#remove-a-node-from-the-dom)
    - [Copy a node](#copy-a-node)
    - [Dealing with HTML Classes](#dealing-with-html-classes)
    - [Accessing the positioned ancestor of HTML element](#accessing-the-positioned-ancestor-of-html-element)
    - [Retrieving the coordinates of an element relative to `<element>.offsetParent`](#retrieving-the-coordinates-of-an-element-relative-to-elementoffsetparent)
    - [Retrieving the width and height of an element](#retrieving-the-width-and-height-of-an-element)
    - [Deal with scrolling on a screen](#deal-with-scrolling-on-a-screen)
    - [Retrieve the element size and coordinates with `getBoundingClientRect`](#retrieve-the-element-size-and-coordinates-with-getboundingclientrect)
    - [Retrieving the element coordinates with `elementFromPoint`](#retrieving-the-element-coordinates-with-elementfrompoint)
  - [DOM Events](#dom-events)
    - [Pointer events](#pointer-events)
      - [Pointer event properties](#pointer-event-properties)
      - [Capturing pointer id](#capturing-pointer-id)
    - [Mouse events](#mouse-events)
      - [The properties of mouse events](#the-properties-of-mouse-events)
    - [Keyboard events](#keyboard-events)
    - [`<form>` element events](#form-element-events)
    - [`transitionend`](#transitionend)
    - [Clipboard events](#clipboard-events)
    - [Scroll events](#scroll-events)
    - [`input` and `change` events](#input-and-change-events)
    - [Ways to assign an event handler](#ways-to-assign-an-event-handler)
    - [`this` in the DOM event](#this-in-the-dom-event)
    - [Properties of the event object](#properties-of-the-event-object)
    - [Preventing the default event action](#preventing-the-default-event-action)
    - [Custom events](#custom-events)
    - [Events that come from real user actions](#events-that-come-from-real-user-actions)
    - [Document and resource loading](#document-and-resource-loading)
      - [`DOMContentLoaded`](#domcontentloaded)
      - [`load`](#load)
      - [`unload`](#unload)
      - [`beforeunload`](#beforeunload)
      - [`async`, `defer`](#async-defer)
      - [Tracking the loading scripts and other external resources](#tracking-the-loading-scripts-and-other-external-resources)
  - [Forms](#forms)
    - [`document.forms`](#documentforms)
    - [`form.elements`](#formelements)
    - [`<fieldset>`](#fieldset)
    - [`<element>.form`](#elementform)
    - [`<select>` element](#select-element)
      - [`<option>`](#option)
    - [submit a form to a server manually](#submit-a-form-to-a-server-manually)
  - [Window object](#window-object)
    - [`window.caches`](#windowcaches)
      - [Create a new cache with `window.caches.open`](#create-a-new-cache-with-windowcachesopen)
      - [Add to cache with the `add()` method from a `Cache` instance](#add-to-cache-with-the-add-method-from-a-cache-instance)
      - [Add to cache with the `addAll()` method from a `Cache` instance](#add-to-cache-with-the-addall-method-from-a-cache-instance)
      - [Change and override cache with the `put()` method from a `Cache` instance](#change-and-override-cache-with-the-put-method-from-a-cache-instance)
      - [Retrieve an item in cache using `match()` method from `Cache` and `CacheStorage`](#retrieve-an-item-in-cache-using-match-method-from-cache-and-cachestorage)
      - [Retrieve all items in cache using `matchAll()` method from `Cache` and `CacheStorage`](#retrieve-all-items-in-cache-using-matchall-method-from-cache-and-cachestorage)
      - [Iterate through cache items using `keys()` method from `Cache` and `CacheStorage`](#iterate-through-cache-items-using-keys-method-from-cache-and-cachestorage)
      - [Delete an item from cache using `delete()` method from `Cache`](#delete-an-item-from-cache-using-delete-method-from-cache)
      - [Remove a cache with `window.caches.delete()`](#remove-a-cache-with-windowcachesdelete)
      - [Find a cache with `window.caches.has()`](#find-a-cache-with-windowcacheshas)
    - [`window.clientInformation` or `window.navigator`](#windowclientinformation-or-windownavigator)
      - [`navigator.clipboard`](#navigatorclipboard)
    - [`window.history`](#windowhistory)
      - [Moving back and forward in the browsing history](#moving-back-and-forward-in-the-browsing-history)
      - [Number of pages in the browsing history](#number-of-pages-in-the-browsing-history)
      - [`history.pushState()` and `history.replaceState()`](#historypushstate-and-historyreplacestate)
    - [`window.innerHeight` and `window.innerWidth`](#windowinnerheight-and-windowinnerwidth)
    - [`window.location`](#windowlocation)
      - [Location properties to retrieve URL parts](#location-properties-to-retrieve-url-parts)
      - [`location.assign()`](#locationassign)
      - [`location.replace()`](#locationreplace)
      - [`location.reload()`](#locationreload)
    - [`window.open()` and `close`](#windowopen-and-close)
    - [`window.confirm()`](#windowconfirm)
    - [`window.getSelection()`](#windowgetselection)
      - [Range](#range)
      - [Selection](#selection)
      - [Selection in forms](#selection-in-forms)
  - [Fetch](#fetch)
    - [GET request](#get-request)
    - [POST request](#post-request)
    - [Fetch and HTTP status codes](#fetch-and-http-status-codes)
    - [Headers](#headers)
    - [Cancel a fetch request](#cancel-a-fetch-request)
  - [Regular Expressions](#regular-expressions)
    - [Creating Regular Expressions](#creating-regular-expressions)
    - [Flags](#flags)
    - [Regular Expression methods](#regular-expression-methods)
      - [`.match()`](#match)
      - [`.replace()`](#replace)
      - [`.replaceAll()`](#replaceall)
      - [`<regexp>.test()`](#regexptest)
    - [Character classes](#character-classes)
      - [Inverse classes](#inverse-classes)
    - [Using dot `.`](#using-dot-)
    - [Unicode encoding and `u` flag](#unicode-encoding-and-u-flag)
    - [Anchors: string start `^` and end `$`](#anchors-string-start--and-end-)
      - [Multiline mode of anchors `^`, `$` and the flag `m`](#multiline-mode-of-anchors---and-the-flag-m)
    - [Word boundary: `\b`](#word-boundary-b)
    - [Escaping Special characters](#escaping-special-characters)
    - [Sets and ranges](#sets-and-ranges)
    - [Quantifiers `+`, `\*`, `?` and `{<number>}`](#quantifiers----and-number)
    - [Greedy and lazy quantifiers](#greedy-and-lazy-quantifiers)
    - [Capturing groups](#capturing-groups)
    - [Backreferences in pattern: `\N` and `\k<name>`](#backreferences-in-pattern-n-and-kname)
    - [Alternation (OR) `|`](#alternation-or-)
    - [Lookahead and lookbehind](#lookahead-and-lookbehind)
    - [Catastrophic backtracking](#catastrophic-backtracking)
    - [Sticky flag `y`, searching at position](#sticky-flag-y-searching-at-position)
    - [Methods of RegExp and String](#methods-of-regexp-and-string)
    - [Summary of Regular Expressions](#summary-of-regular-expressions)
  - [URL](#url)
    - [Creating a `URL` object](#creating-a-url-object)
    - [Properties of a `URL` object](#properties-of-a-url-object)
    - [`URLSearchParams`](#urlsearchparams)
    - [Functions for encoding and decoding url and url components](#functions-for-encoding-and-decoding-url-and-url-components)
    - [`createObjectURL()` and `revokeObjectURL()`](#createobjecturl-and-revokeobjecturl)
  - [Binary files](#binary-files)
    - [`ArrayBuffer`](#arraybuffer)
      - [Typed Arrays](#typed-arrays)
      - [Typed Array Methods](#typed-array-methods)
      - [`DataView`](#dataview)
    - [`TextDecoder` and `TextEncoder`](#textdecoder-and-textencoder)
      - [`TextDecoder`](#textdecoder)
      - [`TextEncoder`](#textencoder)
    - [Blob](#blob)
      - [Downloading Blobs](#downloading-blobs)
    - [File and FileReader](#file-and-filereader)
      - [`File`](#file)
      - [`FileReader`](#filereader)
    - [Summary of Binary Files](#summary-of-binary-files)

<hr>
<hr>

## Useful Links

- https://javascript.info
- https://developer.mozilla.org
- https://www.smashingmagazine.com/2012/06/all-about-unicode-utf8-character-sets/
- https://blog.hubspot.com/website/what-is-utf-8

<hr>
<hr>

## `use strict`

Strict mode makes several changes to normal JavaScript semantics:

- Eliminates some JavaScript silent errors by changing them to throw errors.
- Fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that's not strict mode.
- Prohibits some syntax likely to be defined in future versions of ECMAScript.

To invoke strict mode for an entire script, put the exact statement `"use strict"` before any other statements.

```js
"use strict";
```

<hr>
<hr>

## String Methods

### Define a string and access characters

Here is an easy way to define a string:

```js
const str = `This is a string`;
```

<hr>

Accessing different characters of a string:

```js
const str = `This is a string`;

str[0]; // T

str.at(0); // default is zero. T

str.charAt(); // default is zero. T
```

<hr>

### Turning the string into upper or lower case

Turning the string into upper or lower case:

```js
const str = `This is a string`;

str.toUpperCase(); // THIS IS A STRING

str.toLowerCase(); // this is a string
```

<hr>

### `.length`

`length` returns the number of characters in a string:

```js
const str = `This is a string`;

str.length; // 16
```

<hr>

### `.indexOf()`

`indexOf(<characters>, [optional position number])` returns the position of the first occurrence of a substring from a specified position number. Returns `-1` when can't find the string.

```js
const str = `This is a string`;

str.indexOf("is"); // 2

str.indexOf("is", 3); // 5

str.indexOf("is", 6); // -1
```

<hr>

### `.lastIndexOf()`

`lastIndexOf(<characters>, [optional position number])` similar to `indexOf`, but searches from right to left. Returns the position of the first occurrence of a substring from a specified position number. Returns `-1` when can't find the string.

```js
const str = `This is a string`;

str.lastIndexOf("is"); // 5

str.lastIndexOf("is", 4); // 2
```

<hr>

### `.includes()`

`includes(<characters>, [optional position number])` searches for characters in a given string, and returns `true` or `false`. It starts the search from an optional position number if provided.

```js
const str = `This is a string`;

str.includes("is"); // true
str.includes("is", 6); // false
```

<hr>

### `.startsWith()`, `.endsWith()`

`startsWith(<characters>)` checks if a string starts with given characters. Returns `true` or `false`. It's case sensitive:

```js
const str = `This is a string`;

str.startsWith("This"); // true
str.startsWith("this"); // false
```

`endsWith(<characters>)` checks if a string ends with given characters. Returns `true` or `false`. It's case sensitive:

```js
const str = `This is a string`;

str.endsWith("string"); // true
str.endsWith("String"); // false
```

<hr>

### `.slice()`

`slice(<start>, <end>)` returns a section of a string based on given start, and end positions:

```js
const str = `This is a string`;

str.slice(); // This is a string
str.slice(0); // This is a string
str.slice(0, 4); // This
str.slice(-6, -1); // strin
str.slice(-6); // string

str.slice(5, 2); // nothing is returned, as the end position number is smaller than the start position number
```

<hr>

### `.substring()`

`substring(<start> or <end>, <end> or <start>)` returns a section of a string based on given start, and end positions. Unlike `slice`, the end position provided to `substring` can be lower than the start position. Also, if either or both of the arguments to `substring()` are negative or `NaN`, the `substring()` method treats them as if they were 0:

```js
const str = `This is a string`;

str.substring(); // This is a string
str.substring(0); // This is a string
str.substring(2, 9); // is is a
str.substring(9, 2); // is is a.

str.substring(-5, -2); // nothing is returned
```

<hr>

### `.substr()`

`substr(<start>, <number of characters>)` returns a section of a string at the specified location and having the specified length. Negative lengths in `substr()` are treated as zero. This method is deprecated, and is not advised to be used.

```js
const str = `This is a string`;

str.substr(); // This is a string
str.substr(0); // This is a string
str.substr(5, 4); // is a
str.substr(-4, 4); // ring

str.substr(-4, -4); // nothing is returned
```

<hr>

### `.split()`

`split(<delimiter> [, <limit>])` returns a string split by a provided delimiter. If you provide a number to `split` as a second argument, it will return the limited number of split items in the resulting array:

```js
const str = `This is a string`;

str.split(); // ['This is a string']
str.split(" "); // ['This', 'is', 'a', 'string']
str.split(" ", 2); // ['This', 'is']
str.split(""); // ['T', 'h', 'i', 's', ' ', 'i', 's', ' ', 'a', ' ', 's', 't', 'r', 'i', 'n', 'g']
str.split("is"); // ['Th', ' ', ' a string']
```

<hr>

### `.trim()`

The `trim()` method removes whitespace from both ends of a string without modifying the original string.:

```js
const sentence = "   JavaScript is amazing!   ";

console.log(sentence.trim()); // JavaScript is amazing!
```

<hr>

### Looping through strings

You can loop through strings:

```js
const str = `This is a string`;

for (let char of str) {
  console.log(char);
}
```

```js
const str = `This is a string`;

for (let charIndex = 0; charIndex < str.length; charIndex++) {
  console.log(str[charIndex]);
}
```

<hr>
<hr>

## Number Methods

### `.toFixed()`

`toFixed([<decimal place>])` method rounds a number to given (optional) decimal places:

```js
const num = 123456.789;

num.toFixed(); // 123457, rounds to 0 decimal places
num.toFixed(2); // 123456.79, rounds to 2 decimal places
```

<hr>

### define numbers using `e`

We can define numbers using `e`:

```js
const thousand = 1e3; // same as 1000 (10^3)
const oneThousandth = 1e-3; // same as 1/1000
```

<hr>

### `isNaN()` and `Number.isNaN()`

`isNaN()` tells if the provided argument is not a number (`NaN`), after trying to convert the provided argument to a number, if necessary. Returns `true` or `false`:

```js
const num = 123456.789;
const numString = "123456.789";
const halfNum = "45.34tgy6";

isNaN(num); // false. num is a number
isNaN(numString); // false. numString is a number, because isNaN converted it to a number
isNaN(halfNum); // true. halfNum is not a number
isNaN(NaN); // true. NaN is not a number
```

`Number.isNaN()` tells if the provided argument is precisely the value `NaN`. Returns `true` or `false`:

```js
const num = 123456.789;
const numString = "123456.789";
const halfNum = "45.34tgy6";

Number.isNaN(num); // false. num is not NaN
Number.isNaN(numString); // false. numString is not NaN
Number.isNaN(halfNum); // false. halfNum is not NaN
Number.isNaN(NaN); // true. NaN is NaN
```

<hr>

### `isFinite()` and `Number.isFinite()`

`isFinite()` tells if a number is finite or not, after trying to convert the provided argument to a number, if necessary. Returns `true` or `false`:

```js
isFinite(15); // true
isFinite("15"); // true
isFinite(NaN); // false
isFinite(Infinity); // false
isFinite(-Infinity); // false
```

`Number.isFinite()` tells if a number is finite or not, without converting the provided argument to a number. It checks that a given value is a number, and the number is neither positive `Infinity`, negative `Infinity`, nor `NaN`:

```js
Number.isFinite(15); // true
Number.isFinite("15"); // false
Number.isFinite(NaN); // false
Number.isFinite(Infinity); // false
Number.isFinite(-Infinity); // false
```

<hr>

### `Number.isInteger()`

`Number.isInteger()` tells if a provided number is integer or not:

```js
Number.isInteger(123456); // true
Number.isInteger(123456.789); // false
Number.isInteger(NaN); // false
Number.isInteger(Infinity); // false
Number.isInteger(-Infinity); // false
Number.isInteger("10"); // false
Number.isInteger(true); // false
Number.isInteger(false); // false
```

<hr>

### `parseInt()` and `Number.parseInt()`

`parseInt()` and `Number.parseInt()` parses a string to an integer. They have the same functionality:

```js
const halfNum = "45.34tgy6";

parseInt("100px"); // 100
parseInt("12.3.4"); // 12
parseInt(halfNum); // 45

Number.parseInt("100px"); // 100
Number.parseInt("12.3.4"); // 12
Number.parseInt(halfNum); // 45
```

<hr>

### `parseFloat()` and `Number.parseFloat()`

`parseFloat()` and `Number.parseFloat()` parses a string to a number. They have the same functionality:

```js
const halfNum = "45.34tgy6";

parseFloat("100px"); // 100
parseFloat("12.3.4"); // 12.3
parseFloat(halfNum); // 45.34

Number.parseFloat("100px"); // 100
Number.parseFloat("12.3.4"); // 12.3
Number.parseFloat(halfNum); // 45.34
```

<hr>
<hr>

## Math Object

### `Math.random()`

`Math.random()` returns a number between 0 and 1 (exclusive).

<hr>

### `Math.max()`

`Math.max()` returns the maximum number from provided arguments.

```js
Math.max(2, 6, 8); // 8
```

### `Math.min()`

`Math.min()` returns the minimum number from provided arguments.

```js
Math.min(2, 6, 8); // 2
```

<hr>

### `Math.pow()`

`Math.pow()` takes a number (as a first argument) to a power provided as a second argument:

```js
Math.pow(5, 2); // 25
```

<hr>

### `Math.PI`

`Math.PI` returns the number Pi.

<hr>

### `Math.trunc()`

`Math.trunc()` truncates a number:

```js
Math.trunc(Math.PI); // 3
```

### `Math.round()`

`Math.round()` rounds a number to the nearest integer:

```js
Math.round(3.5); // 4
```

### `Math.ceil()`

`Math.ceil()` rounds a number up:

```js
Math.ceil(3.1); // 4
```

### `Math.floor()`

`Math.floor()` rounds a number down:

```js
Math.floor(3.5); // 3
```

<hr>

### Supported Math Operations

The following math operations are supported:

- Addition `+`,
- Subtraction `-`,
- Multiplication `*`,
- Division `/`,
- Remainder `%`,
- Exponentiation `**`.

<hr>
<hr>

## Type Conversion

### `String()`

`String()` turns the provided argument into a string:

```js
typeof String(10); // string
```

### `Number()`

`Number()` turns the provided argument into a number:

```js
typeof Number("10"); // number
```

#### `+` operator

As well as adding numbers, `+` operator, can be used to convert a variable to a number:

```js
typeof +"10"; // number
```

### `Boolean()`

`Boolean()` turns the provided argument to either `true` or `false`:

```js
Boolean(" "); // true
Boolean(""); // false
```

<hr>
<hr>

## Conditionals

### `if()` on a single line

We can write an `if()` statement on a single line like this:

```js
const condition1 = true,
  condition2 = true;

if (condition1 === condition2) console.log(`It worked`); // It worked
```

### `if()...else`

An example for an `if()...else` statement:

```js
const condition1 = true,
  condition2 = false;

if (condition1 === condition2) {
  console.log(`${condition1} and ${condition2} are equal`);
} else {
  console.log(`some default result`);
}
```

### `if()...else if()...else`

An example for `if()...else if()...else` statement:

```js
const condition1 = true,
  condition2 = false;

if (condition1 === condition2) {
  console.log(`${condition1} and ${condition2} are equal`);
} else if (condition1 < condition2) {
  console.log(`${condition1} is less than ${condition2}`);
} else {
  console.log(`some default result`);
}
```

<hr>

### Ternary conditions

We can set ternary conditions like this:

```js
const condition1 = true,
  condition2 = false;

const resultOfConditions =
  condition1 === condition2
    ? `Equal`
    : condition1 < condition2
    ? `Less`
    : condition1 > condition2
    ? `More`
    : `None is true`;

console.log(resultOfConditions); // More
```

<hr>

### `switch`

Another conditional statement is `switch`. `switch` statement needs a strict match, meaning the same data type:

```js
const condition1 = true;

switch (condition1) {
  case 0:
    console.log(0);
    break;
  case 1:
  case 2:
    console.log(`1 or 2`);
    break;
  case 3:
    console.log(3);
    break;
  default:
    console.log(`Default result`);
}
```

<hr>
<hr>

## Loops

### `while()`

An example for the `while()` loop:

```js
let condition = 1;

while (condition < 3) {
  console.log(condition);
  condition++;
} // 1 2
```

### `while` with `break`

We can use `while` with `break` as well:

```js
let condition = 1;

while (condition < 3) {
  console.log(condition);
  condition++;
  break;
} // 1
```

### `while()` loop on a single line

We can write a `while()` loop on one line:

```js
let condition = 1;

while (condition < 3) console.log(condition++);
```

<hr>

### `do...while()`

`do...while()` loop runs at least once, then checks if a condition for the loop is true:

```js
let condition = 1;

do {
  console.log(condition);
  condition++;
} while (condition < 1);
```

<hr>

### `for()`

An example for the `for()` loop:

```js
for (let i = 0; i < 3; i++) {
  console.log(i);
}
```

`for` loops can also be like these:

```js
let condition = 1;

for (; condition < 3; condition++) {
  console.log(condition);
}
```

```js
let condition = 1;

for (; condition < 3; ) {
  console.log(condition++);
  break;
}
```

<hr>

### Named `for` loop

We can name a `for` loop and then `break` the loop using the name:

```js
label: for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
    if (j == 1) continue; // skips the inner loop when j == 1
    if (i == 1) break label; // breaks the outer loop when i == 1

    console.log(`i is ${i}, j is ${j}`);
  }
}
```

```js
// Example 2: Using break to exit the inner loop:
outerLoop: for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
    if (j == 1) {
      console.log(`Breaking out of inner loop`);
      break;
    }
    console.log(`i: ${i}, j: ${j}`);
  }
}
```

<hr>
<hr>

## Functions

### Creating a function

There are several ways to create a function:

1. This type of creating a function is called a function declaration:

```js
function declaration() {
  console.log(
    `This type of creating a function is called function declaration`
  );
  // you don't need ; after a function declaration
}

declaration();
```

2. This type of creating a function is called a function expression:

```js
const functionName = function () {
  console.log(
    `This type of creating a function is called a function expression`
  );
};

functionName();
```

3. This type of function is called an arrow function:

```js
const arrowFunctionName = () =>
  `This type of function is called an arrow function`;

console.log(arrowFunctionName());
```

When an arrow function has a single parameter, it doesn't need parentheses, curly braces, and the `return` statement:

```js
const arrowFunctionWithSingleParameter = (singleParameter) =>
  `${singleParameter} doesn't need parentheses, curly braces, and an explicit return`;

console.log(arrowFunctionWithSingleParameter);
```

A multiline arrow function needs curly braces and the `return` statement:

```js
const multilineArrowFunction = () => {
  // multiline arrow function needs curly braces and an explicit return statement, if we want to return something
  return `something`;
};

console.log(multilineArrowFunction);
```

4. Another way to declare a function is to use `new Function()`:

   ```js
   const functionName = new Function(
     `console.log("this is a code inside the function")`
   );

   functionName();
   ```

   ```js
   const functionName = new Function(
     "parameter1",
     "parameter2",
     "return parameter1 + parameter2"
   );

   console.log(functionName(1, 2)); // 3
   ```

<hr>

### Set a default value to a parameter in a function

We can set a default value to a parameter, when we are creating a function:

```js
function declaration(parameter1, parameterWithDefaultValue = `Default value`) {
  // this parameter will be undefined, if it won't be set while calling the function
  console.log(`parameter1: ${parameter1}`);

  //  - this parameter will have the default value, if nothing is set while calling the function
  console.log(`parameterWithDefaultValue: ${parameterWithDefaultValue}`);
}

declaration();
declaration(10);
declaration(10, 20);
```

<hr>

### Access all arguments of a function

We can access all arguments of a function using the spread operator like this:

```js
function threeDots(...args) {
  for (let arg of args) console.log(`${arg} is part of ${args} array`);

  return args;
}

function threeDots2(...anyWord) {
  for (let arg of anyWord) console.log(`${arg} is part of ${anyWord} array`);

  return anyWord;
}

console.log(threeDots(1, 2, 3));
console.log(threeDots2(1, 2, 3));

// both functions log
// 1 is part of 1, 2, 3 array
// 2 is part of 1, 2, 3 array
// 3 is part of 1, 2, 3 array
// finally, both functions return [1, 2, 3] in the end.
```

We can use the `...` operator together with other parameters as well:

```js
function twoParametersAndTheRest(parameter1, parameter2, ...theRest) {
  console.log(
    `Here is parameter1: ${parameter1},\nhere is parameter2: ${parameter2},\nand here are the rest of the parameters: ${theRest}`
  );

  return theRest;
}

console.log(twoParametersAndTheRest(1, 2, 3, 4, 5));
// logs
// Here is parameter1: 1,
// here is parameter2: 2,
// and here are the rest of the parameters: 3,4,5
// finally, returns [3, 4, 5]
```

<hr>

`arguments` is a keyword to access all the arguments provided to a function:

```js
function accessingAllArguments() {
  console.log(`${arguments} is an array-like object`);
  console.log(`${arguments[0]} is the first argument of the function`);
  console.log(
    `${arguments.length} is the number of arguments called with the function`
  );
}

accessingAllArguments(1, 2);
// logs
// [object Arguments] is an array-like object
// 1 is the first argument of the function
// 2 is the number of arguments called with the function
```

<hr>

### Using the spread operator inside a function

Using the spread operator inside a function, turns an iterable into a list of arguments:

```js
function callWith3Dots(arr) {
  console.log(...arr); // 3 Dots in a function call turns an iterable into a list of arguments
  return Math.max(...arr);
}
callWith3Dots([3, 5, 8]);
// logs 1 2 3
// returns 8
```

<hr>

### Get the number of parameters of a function

We can access how many parameters a function has using the `length`:

```js
function functionWith2Parameters(a, b) {}
function functionWithManyParameters(a, b, ...more) {}

console.log(functionWith2Parameters.length); // returns 2
console.log(functionWithManyParameters.length); // still returns 2
```

<hr>

### Returns from a function

When a function is not set to return anything explicitly, it returns `undefined`:

```js
function returnsUndefined() {
  // nothing is happening, so function returns undefined
}
```

```js
function returnsUndefined() {
  let a = 0;
  let b = 0;
  a + b;
  // again, function returns undefined
}
```

A function with an empty `return` also returns `undefined`:

```js
function emptyReturnGivesUndefined() {
  return; // returns undefined
}
```

<hr>

### Copying a function

Here is a quick way to copy a function:

```js
function func1() {
  console.log(`copied`);
}
const func2 = func1; // both are functions now

func1(); // copied
func2(); // copied
```

<hr>

### Add a property to a function from outside

We can also add a property to a function from the outside of the function:

```js
function withExternalProperty() {}

withExternalProperty.addedExternally = `you can add a property to a function from the outside`;

console.log(withExternalProperty.addedExternally);
```

<hr>

### `setTimeout()` and `clearTimeout()`

Here is how to use `setTimeout` and `clearTimeout`:

```js
const functionName = function () {
  console.log(`function has run`);
};

const timerId = setTimeout(functionName, 1000); // runs after 1 second (1000 milliseconds)
```

```js
setTimeout(() => {
  console.log(`this also works`);
}, 1000);
```

```js
setTimeout(`console.log("this also works)`, 1000);
```

`clearTimeout` clears the timeout and stops the `setTimeout` from running:

```js
const condition = true;

const timerId = setTimeout(() => {
  console.log(`this function doesn't run`);
}, 1000);

if (condition) {
  clearTimeout(timerId);
}
```

Here is a way to provide arguments to a function used inside `setTimeout`:

```js
const functionName = function (arg1, arg2) {
  console.log(`function has run with arguments: ${arg1} and ${arg2}`);
};

const timerId = setTimeout(functionName, 1000, `argument1`, `argument2`);
```

<hr>

### `setInterval()` and `clearInterval()`, and nested `setTimeout()`

Here is how to use `setInterval` and `clearInterval`:

```js
const functionName = function () {
  console.log(`function has run`);
};

const timerId = setInterval(functionName, 2000); // runs every 2 seconds
// not exactly 2 seconds. As it runs more, the call to a function is being delayed
```

`clearInterval` clears the interval and stops the `setInterval` from running:

```js
const functionName = function () {
  console.log(`function has run`);
};

const timerId = setInterval(functionName, 2000); // runs every 2 seconds

// clears the interval after 5 seconds
setTimeout(clearInterval, 5000, timerId);
```

Nested `setTimeout` is more preferred than `setInterval`:

```js
const nestedSetTimeoutId = setTimeout(function tick() {
  console.log(`tick`);
  setTimeout(tick, 2000);
}, 2000); // this works more precisely than setInterval
```

Here is an example of clearing a nested `setTimeout`:

```js
let count = 0;

const timerID = setTimeout(function tick() {
  count++;
  if (count > 3) {
    return;
  }
  console.log(`tick`);
  setTimeout(tick, 1000);
}, 1000);
```

<hr>

### `.call()`, `.apply()`, `.bind()`

`.call()` method of the `Function` instance applies `this` keyword to a provided argument:

```js
function func(parameter1) {
  console.log(`${param1}, ${this.name}`);
}

const user = { name: `some name` };

// function.call(setThis, arguments)
func.call(user, "Hi"); // "this" in func now refers to the user object
```

`.apply()` method is similar to `.call()`. But the arguments provided to the function using `.apply()` should be either in an array or an array-like object:

```js
function func(parameter1, parameter2) {
  console.log(this.name + parameter1 + parameter2);
}

const user = { name: `some name` };

// function.apply(setThis, arrayLikeObjectOfArguments);
func.apply(user, [" hi", " bye"]);
```

`.bind()` method binds `this` keyword of a function (or method) to a provided object:

```js
function func() {
  console.log(this.name);
}

const user = { name: `some name` };

// function.bind(this)
const bindUser = func.bind(user);

bindUser(); // logs some name
```

```js
const user = {
  firstName: "John",
  sayHi() {
    alert(`Hello, ${this.firstName}!`);
  },
};

const sayHi = user.sayHi.bind(user);

// can now run it without an object
sayHi(); // Hello, John!

const user2 = {
  firstName: "Jack",
};

const sayHi2 = user.sayHi.bind(user2);

sayHi2(); // Hello, Jack!
```

```js
function test(arg) {
  console.log(this.number, arg);
}

const bindedFn = test.bind({ number: 99 }, "argument");

bindedFn(); // 99, "argument"
```

> Summary:
>
> - `.call()`: binds `this` keyword value, **invokes the function**, and allows you to pass **a list of arguments**.
> - `.apply()`: binds `this` keyword value, **invokes the function**, and allows you to pass arguments as an **array**.
> - `.bind()`: binds `this` keyword value, **returns** a new function, and allows you to pass **a list of arguments**.

<hr>

### `eval()`

`eval()` evaluates a code provided to it as a string, and executes it:

```js
eval(`console.log("Hello")`); // Hello
```

`eval` returns the last statement, if more than one statement is provided to it:

```js
const evalReturnsLastValue = eval(`let i = 0; ++i`);
console.log(evalReturnsLastValue); // 1
```

<hr>

### Currying

Here is an example of currying:

```js
function add(a) {
  return function (b) {
    return a + b;
  };
}

console.log(add(5)(3)); // 8

let addFive = add(5);

console.log(addFive(3)); // 8
```

<hr>
<hr>

## Objects

### Creating an object

This way of creating an object is called "object constructor" syntax:

```js
const obj = new Object();
```

This way of creating an object is called "object literal" syntax:

```js
const obj = {};
```

<hr>

Here is an example of creating an object with a custom constructor function:

```js
function ConstructorFunction(name) {
  this.name = name;
  this.someProperty = "someProperty";
}

const obj = new ConstructorFunction("some name");

console.log(obj); // ConstructorFunction {name: 'some name', someProperty: 'someProperty'}
console.log(typeof obj); // object
```

<hr>

### Object keys and values, and accessing them

Objects consist of key-value pairs separated with a colon. If object keys have more than one word, they need to be written in quotes:

```js
const obj = {
  name: "some name",
  surname: "some surname",
  "multi-word property": "some value",
};
```

<hr>

To get the value of an object property, we can use the below ways:

```js
const obj = {
  name: "some name",
  surname: "some surname",
  "multi-word property": "some value",
};

obj.name;
obj["name"];
obj["multi-word property"];
```

<hr>

We can also use string concatenation while referring to or creating an object property:

```js
const obj = {
  name: "some name",
  surname: "some surname",
  "multi-word property": "some value",
};

const multi = "multi-";
obj[multi + "word property"];
```

```js
const prop = "property";
const obj = {
  [prop + "Name"]: "some value",
};

console.log(obj["propertyName"]);
```

<hr>

Instead of writing `name: name` in an object, we can simply write `name`:

```js
const name = "some name";

const obj = {
  name, // same as name:name
  age: 30,
};
```

```js
const obj = {
  name, // same as name: ""
  age: 30,
};
```

<hr>

### Delete a key-value pair

To delete a key-value pair from an object, we use `delete`:

```js
const obj = {
  name,
  age: 30,
};

console.log(obj); // {name: '', age: 30}

delete obj.name;

console.log(obj); // {age: 30}
```

<hr>

### Test if a property exists in an object

Here is one way to test if a property exists in an object:

```js
const obj = {
  name,
  age: 30,
};

console.log("name" in obj); // true

delete obj.name;

console.log("name" in obj); // false
```

<hr>

### Looping through object

Here is one way to loop through an object's keys and values:

```js
const obj = {
  name: "some name",
  age: 30,
};

for (let key in obj) {
  console.log(`${key}: ${obj[key]}`);
}
```

<hr>

### Copy an object

Here is one way to copy an object:

```js
const obj = {
  name: "some name",
  age: 30,
};

const copyOfObj = {};

for (let key in obj) {
  copyOfObj[key] = obj[key];
}
```

#### `Object.assign()`

`Object.assign()` accepts an object as a first argument, and copies all the properties of other objects given to it, into the first argument:

```js
const obj = {
  name: "some name",
  age: 30,
};

const copyOfObj = {};

Object.assign(copyOfObj, obj, {
  "key in another object": "some value",
});
```

#### `structuredClone()`

The global `structuredClone()` method creates a deep copy of an object. If there is a nested object this function copies the nested object as well, and not just a reference to that nested object. It copies together with all the nested objects, and properties, except functions:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

const copyOfObj = structuredClone(obj);
```

<hr>

### optional chaining `?.`

The optional chaining `?.` syntax constructor is like the `.` chaining operator, except that instead of causing an error if a reference is nullish (`null` or `undefined`), the expression returns `undefined`.

- We can use `?.` for safely reading and deleting, but not writing.
- When used with function calls, it returns `undefined`, if the given function does not exist.
- The variable before `?.` must be declared. Otherwise, if there’s no variable at all, then `?.` also triggers an error.

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

// console.log(obj.fullName.surname); // this would cause an error
console.log(obj.fullName?.surname); // undefined

// returns undefined even though obj.func() doesn't exist
console.log(obj.func?.()); // undefined

const anotherObj = null;

// console.log(anotherObj.someProp); // this would cause an error
console.log(anotherObj?.someProp); // undefined
```

<hr>

### `Object.fromEntries()`

Given an array that consists of arrays that have key-value pairs (`[key, value]`), `Object.fromEntries()` creates an object:

```js
const objFromArr = Object.fromEntries([
  ["some property", 1],
  ["another property", 4],
]);
```

We can also create an object from a Map using `Object.fromEntries()`:

```js
const map = new Map();
map.set("property1", 1);
map.set("property2", "value 2");

const obj = Object.fromEntries(map); // create an object from a map

// this also works
console.log(map.entries()); // map iterator
const obj2 = Object.fromEntries(map.entries());
```

<hr>

### `Object.keys()` and `Object.values()`

`Object.keys()` returns an array of object keys. `Object.values()` returns an array of object values:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

Object.keys(obj); // returns an array of keys
Object.values(obj); // returns an array of values
```

These 2 methods provide another way for us to loop through an object. Here is an example of looping through an object's values:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

for (let value of Object.values(obj)) {
  console.log(value); // loop over values
}
```

<hr>

### `Object.entries()`

`Object.entries()` returns an array that includes arrays consisting of key-value pairs:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

Object.entries(obj); // returns an array of [key, value] pairs.
```

<hr>

### `Object.getOwnPropertyDescriptor()`

The method `Object.getOwnPropertyDescriptor()` allows to query the full information about an object's property, including its flags:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

const descriptor = Object.getOwnPropertyDescriptor(obj, "name");
```

### `Object.getOwnPropertyDescriptors()`

The method `Object.getOwnPropertyDescriptors()` allows to query the full information about **all** the properties of an object, including their flags:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

const allDescriptors = Object.getOwnPropertyDescriptors(obj);
```

<hr>

### `Object.defineProperty`

To change the flags of an object's property, we can use the `Object.defineProperty()` method:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

Object.defineProperty(obj, "name", {
  value: "new name",

  writable: true,

  enumerable: false, // Non-enumerable properties are excluded from Object.keys, and for...in

  configurable: true,
  // Non-configurable property can’t be deleted, its attributes can’t be modified.
  // Making a property non-configurable is a one-way road.
  // configurable: false prevents changes of property flags and its deletion, while allowing to change its value.
});
```

If we define a new property with `Object.defineProperty`, by default, all the flags will be false. We need to explicitly list which flag is true.

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

Object.defineProperty(obj, "newProp", {
  value: "new property",
  writable: true,
});
```

### `Object.defineProperties`

To change the flags of several properties at once, we can use `Object.defineProperties`:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

Object.defineProperties(obj, {
  name: { value: "new name", writable: false, enumerable: true },
  surname: { value: "new surname", writable: false, configurable: true },
});
```

<hr>

### Copy an object together with all of its properties' flags

Previous methods provide a new way for us to copy an object. To copy an object together with all of its properties' flags, we can use the below code:

```js
const obj = {
  name: "name",
  sizes: {
    height: 182,
    width: 50,
  },
};

const copyOfObjectWithFlags = Object.defineProperties(
  {},
  Object.getOwnPropertyDescriptors(obj)
);
```

<hr>

### `Object.preventExtension()` and `Object.isExtensible()`

`Object.preventExtension()` prevents the addition of new properties to an object:

```js
Object.preventExtensions(obj);
```

We can check if we can add properties to an object using `Object.isExtensible()`:

```js
Object.isExtensible(obj);
```

### `Object.seal()` and `Object.isSealed()`

`Object.seal()` forbids adding or removing properties. This means that it sets `configurable: false` for all existing properties.

```js
Object.seal(obj);
```

We can check if an object is sealed, using `Object.isSealed()`:

```js
Object.isSealed(obj);
```

### `Object.freeze()` and `Object.isFrozen()`

`Object.freeze()` forbids adding, removing, and changing properties. This means that it sets `configurable: false`, and `writable: false` for all existing properties.

```js
Object.freeze(obj);
```

We can check if an object is frozen using `Object.isFrozen()`:

```js
Object.isFrozen(obj);
```

<hr>

### Accessor properties

Accessor properties are essentially functions that execute on getting and setting a value, but look like regular properties to an external code. In an object literal they are denoted by `get` and `set`:

```js
const objectWithAccessorProperties = {
  name: "John",
  surname: "Doe",

  get fullName() {
    return `${this.name} ${this.surname}`;
  },

  // setter must have exactly one parameter
  set fullName(value) {
    [this.name, this.surname] = value.split(" ");
  },
};

// using the getter
console.log(objectWithAccessorProperties.fullName); // John Doe

// using the setter
objectWithAccessorProperties.fullName = "differentName differentSurname";

// using the getter
console.log(objectWithAccessorProperties.fullName); // differentName differentSurname
```

Note that while using the `defineProperty` method on accessor properties, there is no `value` or `writable`:

```js
const objectWithAccessors = {
  name: "name",
  surname: "surname",
};

Object.defineProperty(objectWithAccessors, "fullName", {
  // For accessor properties, there is no value or writable,
  // but instead there are get and set functions.
  get() {
    return `${this.name} ${this.surname}`;
  },

  set(value) {
    [this.name, this.surname] = value.split(" ");
  },
});

console.log(objectWithAccessors.fullName); // name surname

obj.fullName = "differentName differentSurname";
console.log(obj.fullName); // differentName differentSurname
```

<hr>

### Set the prototype of an object

We can set the prototype of an object with the `__proto__`. Here are 2 ways to do that:

```js
// Object that will be used as a prototype
const Prototype1 = {
  prototypeProp: "prototypeValue",
};

const ChildOfPrototype1 = {
  childProp: "childValue",
};

// Set the Prototype1 object as the prototype
ChildOfPrototype1.__proto__ = Prototype1;

// child object inherits the property from Prototype1
console.log(ChildOfPrototype1.prototypeProp); // prototypeValue

// Another way to set the Prototype_1 object as the prototype
const anotherChildOfPrototype1 = {
  anotherChildProp: "anotherChildValue",
  __proto__: Prototype1,
};

// Property from the Prototype1 can now be accessed in the child object
console.log(anotherChildOfPrototype1.prototypeProp); // prototypeValue
```

<hr>

Here is another way to set the prototype of an object:

```js
// Object that will be used as a prototype
const Prototype1 = {
  prototypeProp: "prototypeValue",
};

function ConstructorFunction(name) {
  this.name = name;
}

// Set the Prototype1 object as the prototype
ConstructorFunction.prototype = Prototype1;
const obj = new ConstructorFunction("new name");

console.log(obj.prototypeProp); // true
```

<hr>

We can create a new object and provide a prototype for it using the `Object.create()` method:

```js
// Object that will be used as a prototype
const Prototype1 = {
  prototypeProp: "prototypeValue",
};

// creates an object with the prototype Prototype_1
const obj = Object.create(Prototype1, {
  objProp: {
    value: "objValue",
    writable: false,
  },
});

console.log(obj.objProp); // objValue
console.log(obj.prototypeProp); // prototypeValue
```

`Object.setPrototypeOf()` helps to set the prototype of an object:

```js
// Objects that will be used as a prototype
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const Prototype2 = {
  prototypeProp2: "prototypeValue2",
};

const obj = {};

// Set the Prototype1 as the prototype of obj
Object.setPrototypeOf(obj, Prototype1);
console.log(obj.prototypeProp1); // prototypeValue1

// change the prototype of obj to Prototype2
Object.setPrototypeOf(obj, Prototype2);
console.log(obj.prototypeProp1); // undefined
console.log(obj.prototypeProp2); // prototypeValue2
```

The `Object.getPrototypeOf()` static method returns the prototype (i.e. the value of the internal `[[Prototype]]` property) of the specified object:

```js
// Objects that will be used as a prototype
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const Prototype2 = {
  prototypeProp2: "prototypeValue2",
};

const obj = {};

// Set the Prototype1 as the prototype of obj
Object.setPrototypeOf(obj, Prototype1);
console.log(Object.getPrototypeOf(obj)); // {prototypeValue1: 'prototypeValue1'}

// change the prototype of obj to Prototype2
Object.setPrototypeOf(obj, Prototype2);
console.log(Object.getPrototypeOf(obj)); // {prototypeValue2: 'prototypeValue2'}
```

Combining `Object.create()`, `Object.getPrototypeOf()`, and `Object.getOwnPropertyDescriptors()` helps us to copy an object with all of its properties and descriptors:

```js
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const powerfulCopyOfObject = Object.create(
  Object.getPrototypeOf(Prototype1),
  Object.getOwnPropertyDescriptors(Prototype1)
);
```

<hr>

### Add a method to a native prototype

Here is how we can add a method to a native prototype:

```js
String.prototype.newMethodToNativePrototype = function () {
  return `this adds a method to the native String prototype`;
};

console.log("any string".newMethodToNativePrototype());
// this adds a method to the native String prototype
```

<hr>

### `.isPrototypeOf()`

There’s also a method `objA.isPrototypeOf(objB)`, that returns `true`, if `objA` is somewhere in the chain of prototypes for `objB`.

```js
// Objects that will be used as a prototype
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const Prototype2 = {
  prototypeProp2: "prototypeValue2",
};

const Prototype3 = {
  prototypeProp3: "prototypeValue3",
};

const Child1 = {
  childProp1: "childValue1",
};

Object.setPrototypeOf(Prototype2, Prototype1);
Object.setPrototypeOf(Child1, Prototype2);

console.log(Prototype2.isPrototypeOf(Child1)); // true
console.log(Prototype1.isPrototypeOf(Child1)); // true

console.log(Prototype3.isPrototypeOf(Child1)); // false
```

<hr>

### Looping and prototypes

`Object.keys` only returns own keys of an object:

```js
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const Child1 = {
  childProp1: "childValue1",
};

Object.setPrototypeOf(Child1, Prototype1);

console.log(Object.keys(Child1)); // ['childProp1']
```

`for ... in` loop loops over both own and inherited keys (from a prototype) of an object:

```js
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const Child1 = {
  childProp1: "childValue1",
};

Object.setPrototypeOf(Child1, Prototype1);

for (let key in Child1) {
  console.log(key); // childProp1 prototypeProp1
}
```

#### `.hasOwnProperty()`

`hasOwnProperty()` accepts property as an argument and returns `true`, if the property is own, not an inherited one:

```js
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const Child1 = {
  childProp1: "childValue1",
};

Object.setPrototypeOf(Child1, Prototype1);

for (let key in Child1) {
  // returns true if the property is own property, not an inherited one
  console.log(key, Child1.hasOwnProperty(key));
  // childProp1 true
  // prototypeProp1 false
}
```

<hr>

#### `Object.getOwnPropertyNames()`

`Object.getOwnPropertyNames()` returns all own property names in an array:

```js
const Prototype1 = {
  prototypeProp1: "prototypeValue1",
};

const Child1 = {
  childProp1: "childValue1",
};

Object.setPrototypeOf(Child1, Prototype1);

console.log(Object.getOwnPropertyNames(Child1)); // ['childValue1']
```

<hr>
<hr>

## Symbol

### Create a `Symbol()`

Here is how to create a `Symbol()`.

```JS
const id = Symbol();

console.log(id); // Symbol()
```

<hr>

Note that 2 different symbols do not equal each other, even if they have the same description:

```js
const id1 = Symbol("id");
const id2 = Symbol("id");

console.log(id1); // Symbol(id)
console.log(id2); // Symbol(id)

console.log(id1 == id2); // false
console.log(id1 === id2); // false
```

<hr>

### `description` property

All symbols have the `description` property:

```js
const id = Symbol("test");

console.log(id.description); // test
```

<hr>

### Converting symbols to a string

To convert the symbols to a string, we can either use the `String()` function or call `.toString()` method on them:

```js
const id = Symbol("id");

console.log(String(id)); // Symbol(id)
console.log(id.toString()); // Symbol(id)
```

<hr>

### Symbols in an object literal

If we want to use a symbol in an object literal `{...}`, we need square brackets around it:

```js
const id = Symbol("id");

const obj = {
  name: "SomeName",
  [id]: 123,
};

console.log(obj); // {name: 'some name', Symbol(id): 123}
```

<hr>

### Symbol properties and looping

Symbolic properties do not participate in the `for...in` loop and `Object.keys()` also ignores them:

```js
const id = Symbol("id");

const obj = {
  name: "SomeName",
  [id]: 123,
};

for (key in obj) {
  console.log(key);
} // name

console.log(Object.keys(obj)); // ['name']
```

<hr>

### `Object.getOwnPropertySymbols()`

There is a built-in method `Object.getOwnPropertySymbols(<obj>)` that allows us to get all symbols of an object.

```js
const id = Symbol("id");

const obj = {
  name: "SomeName",
  [id]: 123,
};

console.log(Object.getOwnPropertySymbols(obj)); // [Symbol(id)]
```

<hr>

### `Object.assign()` and symbols

`Object.assign()` copies both string and symbol properties:

```js
const id = Symbol("id");

const obj = {
  name: "SomeName",
  [id]: 123,
};

const copyWithSymbols = Object.assign({}, obj);

console.log(copyWithSymbols[id]); // 123
```

<hr>

### `Symbol.for()`

As we’ve seen, usually all symbols are different, even if they have the same description. But sometimes we want the symbols with the same description to be the same entities. To achieve that, there exists a global symbol registry. In order to read (create if absent) a symbol from the registry, use `Symbol.for(<key>)`.

```js
// creates id Symbol in the global registry
const idGlobal = Symbol.for("id");

// reads the same Symbol as the above line
const idGlobal2 = Symbol.for("id");

console.log(idGlobal === idGlobal2); //true
```

<hr>

### `Symbol.keyFor()`

`Symbol.for(<key>)` returns a symbol by description. To do the opposite – to return a description by a global symbol – we can use `Symbol.keyFor(<sym>)`:

```js
// get (or create) a symbol by name
const sym = Symbol.for("name");
const sym2 = Symbol.for("id");

// get name by symbol
console.log(Symbol.keyFor(sym)); // name
console.log(Symbol.keyFor(sym2)); // id
```

<hr>
<hr>

## Arrays

### Create an array

Here are some ways to create an array:

```js
const array = new Array();

console.log(array); // []
```

```js
const array = new Array(4); // creates an array of length 4

console.log(array); // [empty × 4]
console.log(array.length); // 4
```

```js
const array = new Array("value1", "value2", "value3");

console.log(array); // ['value1', 'value2', 'value3']
```

```js
const array = ["value1", "value2", "value3"];

console.log(array); // ['value1', 'value2', 'value3']
```

<hr>

### Accessing array items

We can access the array items using the square bracket notation. Also, `.at()` method helps us to access an array items in a specific position:

```js
const arr = ["value1", "value2", "value3"];

console.log(arr[1]); // value2
console.log(arr.at(1)); // value2
```

<hr>

### Copy arrays with the spread operator

We can copy arrays into another array using the spread operator:

```js
const arr1 = new Array("value1", "value2", "value3");
const arr2 = ["value1", "value2", "value3"];

const arr3 = [0, ...arr1, ...arr2];
console.log(arr3); // [ 0, "value1", "value2", "value3", "value1", "value2", "value3" ]
```

<hr>

### `.pop()`

`.pop()` method deletes and returns the last array item:

```js
const arr = ["value1", "value2", "value3"];

const deletedLastItem = arr.pop();

console.log(arr); // ['value1', 'value2']
console.log(deletedLastItem); // value3
```

### `.push()`

`.push()` method inserts an item to the end of an array. It returns the length of the array:

```js
const arr = ["value1", "value2", "value3"];

const lengthOfArr = arr.push("value4");
console.log(lengthOfArr); // 4

arr.push("value5", "value6");
console.log(arr); // ['value1', 'value2', 'value3', 'value4', 'value5', 'value6']
```

### `.shift()`

`.shift()` deletes and returns the first item of an array:

```js
const arr = ["value1", "value2", "value3"];

const deletedFirstItem = arr.shift();

console.log(arr); // ['value2', 'value3']
console.log(deletedFirstItem); // value1
```

### `.unshift()`

`.unshift()` method inserts an item or items to the beginning of an array. It returns the length of the array:

```js
const arr = ["value1", "value2", "value3"];

arr.unshift("new value1");
arr.unshift("new value2", "new value3");

console.log(arr); // ['new value2', 'new value3', 'new value1', 'value1', 'value2', 'value3']
```

### Return values of `.push()` and `.unshift()`

Remember `.push()` and `.unshift()` returns the length of an array:

```js
const array = ["value1", "value2", "value3"];

const newLength1 = array.push("value4");
const newLength2 = array.push("value5", "value6");

console.log(newLength1); // 4
console.log(newLength2); // 6
```

```js
const array = ["value1", "value2", "value3"];

const newLength1 = array.unshift("new value1");
const newLength2 = array.unshift("new value2", "new value3");

console.log(newLength1); // 4
console.log(newLength2); // 6
```

<hr>

### Cutting out arrays with `.length`

If there is an array with several items, we can keep specific number of them and cut the rest out by specifying the `.length`:

```js
const arr = ["value1", "value2", "value3"];

// keeps only first 2 values of the array
arr.length = 2;

console.log(arr); // ['value1', 'value2']
```

<hr>

### `.splice()`

`.splice()` helps to remove given number of array items starting from a given index:

```js
const arr = ["value1", "value2", "value3"];

// removes 2 values from index 1
arr.splice(1, 2);

console.log(arr); // ['value1']
```

We can also use `.splice()` to add items to a specific position in an array without deleting any existing items:

```js
const arr = ["value1", "value2", "value3"];

// removes 0 values from index 2, and adds 2 values
arr.splice(2, 0, "splice 1", "splice 2");

console.log(arr); // ['value1', 'value2', 'splice 1', 'splice 2', 'value3']
```

<hr>

### `.concat()`

`.concat()` method merges two or more arrays. It does not change the existing arrays, but instead **returns a new array**.

```js
const arr1 = new Array();
const arr2 = ["value2"];
const arr3 = ["value3"];

const newArr = arr1.concat([1, 2], 3, 4, [5, 6], arr2, arr3);

console.log(newArr); // [1, 2, 3, 4, 5, 6, 'value2', 'value3']
```

<hr>

### `.forEach()`

`forEach` method loops through an array and gives access to the **array item**, **index** of the item and the **array** itself:

```js
const arr = ["value1", "value2", "value3"];

arr.forEach((item, index, array) => {
  console.log(
    `${item} is at index ${index} in an array with these items: ${array}`
  );
});
```

<hr>

### `.indexOf()` and `.lastIndexOf`

`.indexOf()` method looks for an item starting from a given index, returns either the index or `-1`. The method `arr.lastIndexOf` is the same as `.indexOf()`, but looks for an item from right to left.

```js
const arr = ["value1", "value2", "value3"];

// looks for "looked up item" starting from index 2 to the right
console.log(arr.indexOf("looked up item", 2)); // -1

// looks for "value1" starting from index 0 to the right
console.log(arr.indexOf("value1", 0)); // 0

// looks for "value1" starting from index 1 to the right
console.log(arr.indexOf("value1", 1)); // -1

// looks for "value1" starting from index 0 to the left
console.log(arr.lastIndexOf("value1", 0)); // 0

// looks for "value1" starting from index 1 to the left
console.log(arr.lastIndexOf("value1", 1)); // 0
```

<hr>

### `.includes()`

`.includes()` looks for an array item starting from a given `index`, and returns `true` or `false`.

```js
const arr = ["value1", "value2", "value3"];

console.log(arr.includes("looked up item", 2)); // false
```

<hr>

### `.find()`

`.find()` method returns the **first array item** that meets a given condition, and returns `undefined` otherwise. It gives access to the **array item**, **index** of the item and the **array** itself:

```js
const arr = [1, 2, 3, 4, 5];

const foundItem = arr.find(function (item, index, array) {
  return item < 3;
});

console.log(foundItem); // 1
```

```js
const arr = [1, 2, 3, 4, 5];

const foundItem = arr.find(function (item, index, array) {
  return item > 3;
});

console.log(foundItem); // 4
```

<hr>

### `.findIndex()` and `.findLastIndex`

`.findIndex()` method returns **index** that meets a given condition. It gives an access to the **array item**, **index** of the item and the **array** itself. The `findLastIndex` method is like `.findIndex()`, but searches from right to left:

```js
const arr = [1, 2, 3, 4, 3, 2, 1];

const result = arr.findIndex(function (item, index, array) {
  return item === 3;
});

console.log(result); // 2
```

```js
const arr = [1, 2, 3, 4, 3, 2, 1];

const result = arr.findLastIndex(function (item, index, array) {
  return item === 3;
});

console.log(result); // 4
```

<hr>

### `.filter()`

`.filter()` method filters the array using the provided condition and returns a new array. It gives an access to the **array item**, **index** of the item and the **array** itself. _It doesn't change the original array_.

```js
const arr = ["value1", "value2", "value3"];

const result = arr.filter(function (item, index, array) {
  return item.startsWith("value") && (item.endsWith("2") || item.endsWith("3"));
});

console.log(result); // ['value2', 'value3']
console.log(arr); // ['value1', 'value2', 'value3']
```

<hr>

### `.map()`

`.map()` method applies the provided function on every array item and returns a new array without changing the original one. It gives an access to the **array item**, **index** of the item and the **array** itself.

```js
const arr = ["value1", "value2", "value3"];

const result = arr.map(function (item, index, array) {
  return item + 0;
});

console.log(result); // ['value10', 'value20', 'value30']
```

<hr>

### `.sort()`

The `.sort()` method of `Array` instances sorts the elements of an array in place and returns the reference to the same array, now sorted. The default sort order is ascending, built upon converting the elements into strings, then comparing their sequences of UTF-16 code unit values.

```js
const arr = ["value3", "value1", "value2", 1, 2, 10, 23];

arr.sort();

console.log(arr); // [1, 10, 2, 23, 'value1', 'value2', 'value3']
```

`.sort()` method also accepts a function to compare the items in an array. The return value should be a number that indicates the relative order of the two array items that are compared: negative if `a` is less than `b`, positive if `a` is greater than `b`, and zero if they are equal.

```js
const array = ["value3", "value1", "value2", 1, 23, 10, 2];

// doesn't change the order of string items in the array
array.sort(function (a, b) {
  return a - b;
});

console.log(array); // ['value3', 'value1', 'value2', 1, 2, 10, 23]
```

### `.toSorted()`

The `.toSorted()` method of Array instances is the copying version of the `.sort()` method. It returns a new array with the elements sorted in ascending order.

```js
const arr = ["value3", "value1", "value2", 1, 2, 10, 23];

// returns new array without modifying the original one
const newArr = arr.toSorted();

console.log(arr); // ['value3', 'value1', 'value2', 1, 2, 10, 23]
console.log(newArr); // [1, 10, 2, 23, 'value1', 'value2', 'value3']
```

<hr>

### `.reverse()`

The `.reverse()` method of Array instances reverses an array in place and returns the reference to the same array:

```js
const arr = ["value3", "value1", "value2", 1, 23, 10, 2];

arr.reverse();

console.log(arr); // [2, 10, 23, 1, 'value2', 'value1', 'value3']
```

### `.toReversed()`

The `.toReversed()` method of Array instances is the copying counterpart of the `.reverse()` method. It returns a new array with the elements in reversed order.

```js
const arr = ["value3", "value1", "value2", 1, 23, 10, 2];

// returns new array without modifying the original one
const newArr = arr.toReversed();

console.log(arr); // ['value3', 'value1', 'value2', 1, 23, 10, 2]
console.log(newArr); // [2, 10, 23, 1, 'value2', 'value1', 'value3']
```

<hr>

### `.join()`

`.join()` method accepts a delimeter as an argument and joins the array items with the provided delimeter.

```js
const arr = ["value1", "value2", "value3"];

console.log(arr.join(", ")); // value1, value2, value3
console.log(arr.join("-")); // value1-value2-value3
```

<hr>

### `.reduce()`

`.reduce()` method reduces the provided item to a single value:

```js
const arr = [1, 2, 3, 4];

const sum = array.reduce(function (acc, item, index, array) {
  return (acc += item);
}, 0); // 0 is initial value for accumulator

// logs 10 - the sum of all items in the array
console.log(sum);
```

### `.reduceRight()`

`.reduceRight()` method does the same thing as `.reduce()` but from right to left:

```js
const arr = [1, 2, 3, 4];

array.reduceRight(function (acc, item, index, array) {
  // does the same thing as above but in a descending order
  return (acc += item);
}, 0);

// logs 10 - the sum of all items in the array
console.log(sum);
```

<hr>

### Higher order functions and `this`

Almost all array methods that call functions – like `find`, `filter`, `map` with a notable exception of `sort`, accept an optional additional parameter `this`. This parameter determines what `this` refers to inside the callback function:

```js
arr.find(func, thisArg);
arr.filter(func, thisArg);
arr.map(func, thisArg);
```

```js
const user = {
  role: "admin",
};

const people = [
  { name: "Name1", role: "admin" },
  { name: "Name2", role: "user" },
  { name: "Name3", role: "admin" },
];

function func(item, index, array) {
  return item.role === this.role;
}

const result = people.filter(func, user);

console.log(result);
/* 
0: {name: 'Name1', role: 'admin'}
1: {name: 'Name3', role: 'admin'}
*/
```

<hr>

### `Array.isArray()`

`Array.isArray()` method returns `true`, if the provided argument is an array, or `false` otherwise:

```js
const arr = [1, 2, 3, 4];

console.log(Array.isArray(arr)); // true
```

<hr>

### `.some()`

If a function returns a truthy value, `.some()` immediately returns `true` and stops iterating over the rest of the items:

```js
const arr = [1, 2, 3, 4];

const result = arr.some(function (item, index, array) {
  return item >= 2;
});

// logs true after the first item that met the condition
console.log(result); // true.
```

<hr>

### `.every()`

If a function returns a falsy value, `.every()` immediately returns `false` and stops iterating over the rest of the items:

```js
const arr = [1, 2, 3, 4];

const result = arr.every(function (item, index, array) {
  return item <= 1;
});

// logs false after the first item that returned a falsy value
console.log(result); // false.
```

<hr>

### `Array.from()`

`Array.from(<obj>)` takes an iterable or array-like value and makes a “real” array from it.

```js
const arrayLike = {
  0: "Hello",
  1: "World",
  length: 2,
};

const arrayFromObject = Array.from(arrayLike);

console.log(arrayFromObject); // ['Hello', 'World']
```

```js
const arrFromStrings = Array.from("Hello");

console.log(arrFromStrings); // ['H', 'e', 'l', 'l', 'o']
```

<hr>

### `.fill()`

`.fill(<value> [, <beginning_index>, <ending_index>])` fills the array with a given value.

```js
const arr = [1, 2, 3, 4];

arr.fill(100, 2, 3);
console.log(arr); // [1, 2, 100, 4]

arr.fill(100, 2, 8);
console.log(arr); // [1, 2, 100, 100]

arr.fill(100);
console.log(arr); // [100, 100, 100, 100]
```

<hr>
<hr>

## Maps

### Create a `Map`

To create a `Map`, we use the `new Map()` syntax:

```js
const map = new Map();
```

<hr>

We can create a map from an object:

```js
const obj = {
  key: "value",
  key2: "value2",
};

const mapFromObj = new Map(Object.entries(obj));

console.log(mapFromObj); // {'key' => 'value', 'key2' => 'value2'}
```

<hr>

We can create a map from an array of arrays:

```js
const map = new Map([
  ["1", "str1"],
  [1, "num1"],
  [true, "bool1"],
]);

console.log(map);
// {'1' => 'str1', 1 => 'num1', true => 'bool1'}
```

<hr>

### Add key-value pairs

To add key-value pairs into a map, we use the `.set()` method:

```js
const map = new Map();

map.set("key", "value");
map.set(1, "value");
map.set("another key", 3).set(4, true);

console.log(map);
// {'key' => 'value', 1 => 'value', 'another key' => 3, 4 => true}
```

<hr>

### Get the value of a specific key

To get the value of a specific key, we use the `.get()` method:

```js
const map = new Map();

map.set("key", "value");
map.set("another key", 3).set(4, true);

const result = map.get("key");

console.log(result); // value
```

<hr>

### `.has()`

`.has()` method returns `true`, if a map has a specific key or `false` otherwise:

```js
const map = new Map();

map.set("key", "value");
map.set("another key", 3).set(4, true);

const result = map.has("key");

console.log(result); // true
```

<hr>

### `.size`

`.size` property of a map returns how many key-value pairs a map has:

```js
const map = new Map([
  ["1", "str1"],
  [1, "num1"],
  [true, "bool1"],
]);

console.log(map.size); // 3
```

<hr>

### `.keys()`

`.keys()` returns an iterable for keys of a map:

```js
const map = new Map([
  ["1", "str1"],
  [1, "num1"],
  [true, "bool1"],
]);

for (let key of map.keys()) {
  console.log(key);
}
```

<hr>

### `.values()`

`.values()` returns an iterable for values of a map:

```js
const map = new Map([
  ["1", "str1"],
  [1, "num1"],
  [true, "bool1"],
]);

for (let value of map.values()) {
  console.log(value);
}
```

<hr>

### `.entries()`

`.entries()` returns an iterable for key-value pairs of a map. Each key-value pair is returned as an array of 2 items - [key, value]:

```js
const map = new Map([
  ["1", "str1"],
  [1, "num1"],
  [true, "bool1"],
]);

for (let entry of map.entries()) {
  console.log(entry);
}
```

We can also loop over the key-value pairs of a map without using `entries` and simply using map itself:

```js
const map = new Map([
  ["1", "str1"],
  [1, "num1"],
  [true, "bool1"],
]);

for (let entry of map) {
  console.log(entry);
}
```

<hr>

### `.forEach()`

Map has a built-in `.forEach()` method, which provides access to each value, key, and the map itself:

```js
const map = new Map();

map.set("key", "value");
map.set("another key", 3).set(4, true);

map.forEach((value, key, map) => {
  console.log(`${key}: ${value} in ${map}`);
});
```

<hr>

### `.delete()`

`.delete()` method deletes a specific key-value pair from map:

```js
const map = new Map();

map.set("key", "value");
map.set("another key", 3).set(4, true);

console.log(map); // {'key' => 'value', 'another key' => 3, 4 => true}

map.delete("key");

console.log(map); // {'another key' => 3, 4 => true}
```

<hr>

### `.clear()`

`.clear()` method deletes all the key-value pairs from a map:

```js
const map = new Map();

map.set("key", "value");
map.set("another key", 3).set(4, true);

console.log(map); // {'key' => 'value', 'another key' => 3, 4 => true}

map.clear();

console.log(map); // {size: 0}
```

<hr>
<hr>

## WeakMaps

### Create a `WeakMap`

To create a `WeakMap`, we use the `new WeakMap()` syntax:

```js
const weakMap = new WeakMap();
```

<hr>

### Add key-value pairs into a weakmap

To add key-value pairs into a weakmap, we use the `.set()` method. Remember the key of a weakmap must be an object:

```js
const weakMap = new WeakMap();

const obj = {
  key: "value",
  key2: "value2",
};

weakMap.set(obj, "value1");
```

<hr>

### Get the value of a specific key

To get the value of a specific key, we use the `.get()` method:

```js
const weakMap = new WeakMap();

const obj = {
  key: "value",
  key2: "value2",
};

weakMap.set(obj, "value1");

console.log(weakMap.get(obj)); // value1
```

<hr>

### `.has()`

`.has()` method returns `true`, if a weakmap has a specific key or `false` otherwise:

```js
const weakMap = new WeakMap();

const obj = {
  key: "value",
  key2: "value2",
};

weakMap.has(obj);
```

<hr>

### `.delete()`

`.delete()` method deletes a specific key-value pair from weakmap:

```js
const weakMap = new WeakMap();

const obj = {
  key: "value",
  key2: "value2",
};

weakMap.delete(obj); // true
```

<hr>
<hr>

## Sets

### Create a `Set`

To create a `Set`, we use the `new Set()` syntax:

```js
const set = new Set();
```

We can create a set from an array:

```js
const set = new Set(["value1", "value1", "value2", "value3"]);

console.log(set); // Set(3) {'value1', 'value2', 'value3'}
```

<hr>

### Add items to a set

To add items to a set, we use the `add` method:

```js
const set = new Set();

set.add("value");
set.add({ name: "some name" });
```

<hr>

### `.has()`

`.has()` method returns `true`, if a set has a specific item or `false` otherwise:

```js
const set = new Set();

set.add("value");
set.add({ name: "some name" });

const result = set.has("value");

console.log(result); // true
```

<hr>

### `.size`

We can find how many items a set has using the `.size` property:

```js
const set = new Set();

set.add("value");
set.add({ name: "some name" });

const result = set.size;

console.log(result); // 2
```

<hr>

### Loop over the set items

We can loop over the set items using the `for...of` loop:

```js
const set = new Set();

set.add("value");
set.add({ name: "some name" });

for (let item of set) console.log(item);
```

<hr>

### `.forEach()`

Set has a `.forEach()` method, which provides access to each value (twice) and the set itself:

```js
const set = new Set();

set.add("value");
set.add({ name: "some name" });

set.forEach((value, valueAgain, set) => {
  console.log(value);
});
```

<hr>

### `.delete()`

`.delete()` method deletes a specific item from a set:

```js
const set = new Set();

set.add("value");
set.add({ name: "some name" });

set.delete("value");
```

### `.clear()`

`.clear()` method deletes all the key-value pairs from a set:

```js
const set = new Set();

set.add("value");
set.add({ name: "some name" });

set.clear();
```

<hr>

The same methods Map has for iterators are also supported with Set:

- `.keys()` – returns an iterable object for values,
- `.values()` – same as `.keys()`, for compatibility with Map,
- `.entries()` – returns an iterable object for entries [value, value], exists for compatibility with Map.

```js
const set = new Set(["value1", "value2"]);

for (let key of set.keys()) console.log(key);
for (let value of set.values()) console.log(value);
for (let entry of set.entries()) console.log(entry);
```

<hr>
<hr>

## WeakSets

### Create a `WeakSet`

To create a `WeakSet`, we use the `new WeakSet()` syntax:

```js
const weakSet = new WeakSet();
```

<hr>

### Add an item to a weakset

To add an item to a weakset, we use the `add` method:

```js
const obj = {
  key: "value",
  key2: "value2",
};

const weakSet = new WeakSet();

weakSet.add(obj);
```

<hr>

### `.has()`

`.has()` method returns `true`, if a weakset has a specific item or `false` otherwise:

```js
const obj = {
  key: "value",
  key2: "value2",
};

const weakSet = new WeakSet();

weakSet.has(obj);
```

<hr>

### `.delete()`

`.delete()` method deletes a specific item from a weakset:

```js
const obj = {
  key: "value",
  key2: "value2",
};

const weakSet = new WeakSet();

weakSet.delete(obj);
```

<hr>
<hr>

## Destructuring

### Destructuring an array

Here is an example of destructuring an array:

```js
const arr = ["Firstname", "Lastname"];

const [firstname, lastname] = arr;

console.log(firstname); // John
console.log(lastname); // Smith
```

Another example of destructuring an array (`.split()` returns an array):

```js
const [firstname, lastname] = "Firstname Lastname".split(" ");

console.log(firstname); // John
console.log(lastname); // Smith
```

Here is an example of destructuring an array and setting the destructured items as values of keys in an object:

```js
const obj = {};
[obj.key1, obj.key2] = "value1 value2".split(" ");

console.log(obj); // {key1: 'value1', key2: 'value2'}
```

We can also destructure partially by taking only some of the array items:

```js
const arr = [1, 2, 3, 4, 5];

const [firstValue, secondValue] = arr; // takes first 2 values and ignores the rest
```

Here is a similar example, but this time the rest of the array items are saved into an array using destructuring:

```js
const arr = [1, 2, 3, 4, 5];
const [first, second, ...theRest] = arr;

console.log(first); // 1
console.log(second); // 2
console.log(theRest); // [3, 4, 5]
```

Here is an example of destructuring by setting default values to variables:

```js
const [value1 = "default value1", value2 = "default value2"] = ["new value1"];

console.log(value1); // new value1
console.log(value2); // default value2
```

### Destructuring a string

Here is an example of destructuring a string:

```js
const [a, b, c] = "abc";
```

### Destructuring a set

Here is an example of destructuring a set:

```js
const [one, two, three] = new Set([1, 2, 3]);
```

### Sawpping values using destructuring

Here is how to swap the values of variables using destructuring:

```js
let one = 2;
let two = 1;

[one, two] = [two, one];

console.log(one); // 1
console.log(two); // 2
```

### Destructuring an object

Destructuring an object:

```js
const obj = {
  title: "title",
  height: 100,
  width: 200,
};

const { title, height, width } = obj;
```

Destructuring an object by setting default values to variables:

```js
const obj = {
  title: "title",
};

const { title = "default value", height = "default height" } = obj;

console.log(title); // title
console.log(height); // default height
```

Instead of using the variables that are exactly the same as keys of an object, we can also rename those variables while destructuring:

```js
const obj = {
  title: "title",
  height: 100,
  width: 200,
};

const { title: t, height: h, width: w } = obj;

console.log(t); // title
console.log(h); // 100
console.log(w); // 200

console.log(title); // Uncaught ReferenceError: title is not defined
```

We can combine both setting the default values and renaming the keys of an object that we are destructuring:

```js
const obj = {
  title: "title",
  height: 100,
};

const {
  title: t = "default value",
  height: h,
  width: w = "default value",
} = obj;

console.log(t); // title
console.log(h); // 100
console.log(w); // default value
```

We can use the spread operator together with the object destructuring as well:

```js
const obj = {
  title: "title",
  height: 100,
  width: 200,
};

const { title, ...restOfObj } = obj;

console.log(title); // title
console.log(restOfObj); // {height: 100, width: 200}
```

We can destructure an object in the function parameters as well:

```js
const obj = {
  title: "some title",
  height: 100,
  width: 200,
};

function func({ title }) {
  return title;
}

console.log(func(obj)); // some title
```

We can also destructure nested objects and arrays:

```js
const obj = {
  size: {
    length: 100,
    altitude: 200,
  },
  items: ["Cake", "Donut"],
  extra: true,
};

const {
  size: { length, altitude },
  items: [item1, item2],
  anotherItem = "default value",
} = obj;

console.log(length); // 100
console.log(item1); // cake
```

<hr>
<hr>

## Date Object

### create a new `Date()`

We can create a new `Date()` variable using the `new` keyword:

```js
// new Date(year, month[, date, hours, minutes, seconds, ms)]
const date = new Date();
console.log(date); // For example, Fri Oct 06 2023 20:40:15 GMT-0700 (Pacific Daylight Time)

// year and month specified (months start from 0)
const date2 = new Date(1991, 2);
console.log(date2); // Mon Mar 25 1991 00:00:00
```

<hr>

### `Date.now()`

The `Date.now()` static method returns the number of milliseconds elapsed since the epoch, which is defined as the midnight at the beginning of January 1, 1970, UTC. If we provide these milliseconds to the `new Date()` syntax, we will get current date and time:

```js
const nowInMS = Date.now();

console.log(nowInMS); // For example, 1519211809934
console.log(new Date(nowInMS)); // logs current date and time
```

### `.getTime()`

`.getTime()` method returns the same as above:

```js
const nowInMS = new Date().getTime();

console.log(nowInMS);
```

<hr>

### Setting a date using the `Date` object

There are different ways of setting a date using the `Date` object. The exact time might vary depending on your time zone:

- Providing `0` to the `Date()` as an argument, will give the date of January 1, 1970, UTC (this might vary depending on the time zone).

  ```js
  const jan_01_1970 = new Date(0);
  ```

- We can provide a date with milliseconds from January 1, 1970, UTC. Below code multiplies number of seconds in an hour with 1000 to get the number of milliseconds in an hour. Then multiplies it with negative 24 hours, to go one day back from January 1, 1970, UTC.

  ```js
  const dec_31_1969 = new Date(-24 * 3600 * 1000);

  console.log(dec_31_1969);
  ```

- We can set a date as a string:

  ```js
  const date2017 = new Date("2017-01-26");
  ```

- A month in the `Date` object starts from `0` (January is `0`). If we provide number of days in a month more than the month can have, the `Date` object automatically calculates a proper date. Below code, for example, returns February 1st, not January 32nd.

  ```js
  // new Date(year, month[, date, hours, minutes, seconds, ms)]
  const date2013 = new Date(2013, 0, 32);

  console.log(date2013); // Fri Feb 01 2013 00:00:00 GMT-0800 (Pacific Standard Time)
  ```

- Here is another example of setting a date with the `Date` object. This time even the optional values are set:

  ```js
  // new Date(year, month[, date, hours, minutes, seconds, ms)]
  new Date(2011, 0, 1, 0, 0, 0, 0); // 1 Jan 2011, 00:00:00
  ```

- The below code returns the same as above. Hours, minutes, seconds, and milliseconds are `0` by default:

  ```js
  // new Date(year, month[, date, hours, minutes, seconds, ms)]
  new Date(2011, 0, 1);
  ```

<hr>

### Retrieve different parts of a date

After creating a date, we can use various methods of the `Date` object to retrieve different parts of a date:

```js
const now = new Date();

now.getFullYear();
now.getMonth(); // number of a month, starting from 0
now.getDate(); // day of a month
now.getDay(); // day of a week
now.getHours();
now.getMinutes();
now.getSeconds();
now.getMilliseconds();
```

The above methods return different values depending on your time zone. There is UTC version of these methods. UTC stands for Coordinated Universal Time. Greenwich Mean Time and UTC display the same time:

```js
const nowUTC = new Date();

nowUTC.getUTCFullYear();
nowUTC.getUTCMonth();
nowUTC.getUTCDate();
nowUTC.getUTCDay();
nowUTC.getUTCHours();
nowUTC.getUTCMinutes();
nowUTC.getUTCSeconds();
nowUTC.getUTCMilliseconds();
```

<hr>

### `.getTimezoneOffset()`

The `.getTimezoneOffset()` method of `Date` instances returns the difference, in minutes, between this date as evaluated in the UTC time zone, and the same date as evaluated in the local time zone:

```js
new Date().getTimezoneOffset();
```

<hr>

### Setting different parts of a date

Here are various ways of setting different parts of a date:

```js
const now = new Date();

now.setFullYear(2011, 1, 1); // setFullYear(year, [month], [date])

now.setMonth(1, 1); // setMonth(month, [date])

now.setDate(1);

now.setHours(1, 0, 0, 0); // setHours(hour, [min], [sec], [ms])

now.setMinutes(20, 0, 0); // setMinutes(min, [sec], [ms])

now.setSeconds(20, 0); // setSeconds(sec, [ms])

now.setMilliseconds(100); // setMilliseconds(ms)
```

<hr>

### `Date.parse()`

`Date.parse(<str>)` can read a date from a string. The JavaScript specification only specifies one format to be universally supported: `YYYY-MM-DDTHH:mm:ss.sssZ`

Various components can be omitted, so the following are all valid:

- Date-only form: YYYY, YYYY-MM, YYYY-MM-DD
- Date-time form: one of the above date-only forms, followed by T, followed by HH:mm, HH:mm:ss, or HH:mm:ss.sss. Each combination can be followed by a time zone offset.

For example, "2011-10-10" (date-only form), "2011-10-10T14:48:00" (date-time form), or "2011-10-10T14:48:00.000+09:00" (date-time form with milliseconds and time zone) are all valid date time strings.

```js
// parses the date into milliseconds
Date.parse("2012-01-26T13:51:50.417-07:00"); // 1327611110417
```

<hr>
<hr>

## JSON

### `JSON.stringify()`

`JSON.stringify(value[, replacer, space])` method converts a JavaScript value to a JSON string, optionally replacing values if a replacer function is specified or optionally including only the specified properties if a replacer array is specified.

```js
const obj = {
  name: "John",
  age: 30,
  isAdmin: false,
  courses: ["html", "css", "js"],
  spouse: null,
};

const json = JSON.stringify(obj);

console.log(json); // {"name":"John","age":30,"isAdmin":false,"courses":["html","css","js"],"spouse":null}
```

Using the replacer function in the `JSON.stringify(value[, replacer, space])`:

```js
const obj = {
  key1: "value1",
  key2: "value2",
  key3: 3,
  key4: "value 4",
  key5: 5,
};

function replacer(key, value) {
  // Filtering out strings
  if (typeof value === "string") {
    return;
  }
  return value;
}

const json = JSON.stringify(obj, replacer);
console.log(json); // {"key3":3,"key5":5
```

<hr>

Be careful with circular references. Use the replacer in `JSON.stringify()`:

```js
const room = {
  number: 23,
};

const meetup = {
  title: "Conference",
  participants: [{ name: "John" }, { name: "Alice" }],
  place: room, // meetup references room
};

// room references meetup
room.occupiedBy = meetup;

// stringifies only the properties in the array
const json = JSON.stringify(meetup, ["title", "participants", "name"]);

console.log(json); // {"title":"Conference","participants":[{"name":"John"},{"name":"Alice"}]}
```

Here is the above example with the replacer function instead of an array:

```js
const room = {
  number: 23,
};

const meetup = {
  title: "Conference",
  participants: [{ name: "John" }, { name: "Alice" }],
  place: room, // meetup references room
};

room.occupiedBy = meetup; // room references meetup

const json = JSON.stringify(meetup, function replacer(key, value) {
  return key == "occupiedBy" ? undefined : value;
});

console.log(json);
// {"title":"Conference","participants":[{"name":"John"},{"name":"Alice"}],"place":{"number":23}}
```

<hr>

### `JSON.parse()`

`JSON.parse()` parses a JSON string, constructing the JavaScript value or object described by the string. An optional reviver function can be provided to perform a transformation on the resulting object before it is returned.

```js
const jsonNumbers = "[0, 1, 2, 3]";

const arr = JSON.parse(jsonNumbers);

console.log(arr); // [0, 1, 2, 3]
```

```js
const json = '{"title":"Conference","date":"2017-11-30T12:00:00.000Z"}';

const obj = JSON.parse(json, function (key, value) {
  if (key == "date") return new Date(value);
  return value;
});

console.log(obj);
// {title: 'Conference', date: Thu Nov 30 2017 04:00:00 GMT-0800 (Pacific Standard Time)}
```

<hr>
<hr>

## Classes

### Define a class and create objects based on a class

We use the `class` keyword to define a new class, and then use that class with the `new` keyword to create a new object based on that class:

```js
class ClassName {
  constructor(name) {
    this.name = name;
  }
  sayHi() {
    console.log(`Hi, ${this.name}`);
  }
}

new ClassName("test").sayHi(); // Hi, test

// create an object based on ClassName
const obj = new ClassName("Ziya");

obj.sayHi(); // Hi, Ziya
```

<hr>

### Classes are functions

A class is actually a function in JavaScript:

```js
class ClassName {
  constructor(name) {
    this.name = name;
  }
  sayHi() {
    console.log(this.name);
  }
}

console.log(typeof ClassName); // function
```

<hr>

### Named class expressions

Similar to Named Function Expressions, class expressions may have a name.

If a class expression has a name, the name used with the `class` keyword is visible inside the class only:

```js
// "Named Class Expression"
// (no such term in the spec, but that's similar to Named Function Expression)
const User = class MyClass {
  sayHi() {
    console.log(MyClass); // MyClass name is visible only inside the class
  }
};

new User().sayHi();
/* logs 
class MyClass {
  sayHi() {
    console.log(MyClass); // MyClass name is visible only inside the class
  }
} */

console.log(MyClass); // error, MyClass name isn't visible outside of the class
```

<hr>

### getters/setters, and computed properties in classes

Just like literal objects, classes may include getters/setters, computed properties etc. These are helpful because they let us have more control.

```js
class User {
  constructor(name) {
    // this code invokes the setter function below
    this.name = name;
  }

  get name() {
    return this._name;
  }

  set name(value) {
    if (value.length < 4) {
      console.log("Name is too short.");
      return;
    }
    this._name = value;
  }
}

let user = new User("John");
console.log(user.name); // John

user = new User(""); // Name is too short.
```

Note that we have used underscore in getter and setter functions, while referring to a variable. This is because if we don't use underscore, and refer to `this.name`, we will trigger the setter function, which will try to set the `name`, which will further trigger the setter function, causing endless loop.

<hr>

### Class fields

In the past, our classes only had methods. “Class fields” is a syntax that allows to add any properties:

```js
class User {
  name = "Some Name";

  sayHi() {
    console.log(`Hello, ${this.name}!`);
  }
}

new User().sayHi(); // Hello, Some Name!
```

<hr>

When a class is created, its methods are stored in the prototype. So, `class User {...}` would store its methods in the `User.prototype`. The important difference of class fields is that they are set on individual objects, not `User.prototype`:

```js
class User {
  name = "Some Name";

  sayHi() {
    console.log(`Hi, ${this.name}`);
  }
}

const user = new User();
console.log(user.name); // Some Name
console.log(User.prototype.name); // undefined
console.log(User.prototype.sayHi); // function sayHi()

console.log(user.name === User.prototype.name); // false
console.log(user.sayHi === User.prototype.sayHi); // true
```

<hr>

### Class inheritance

Class inheritance is a way for one class to extend another class. So we can create a new functionality on top of the existing one. We use the `extends` keyword for this:

```js
class Parent {
  constructor(name) {
    this.name = name + ` this is a parent class`;
  }
  parentMethod() {
    console.log(`hi from parent`);
  }
}

class Child extends Parent {
  childMethod() {
    console.log(`hi from child`);
  }
}

const child = new Child();

child.childMethod(); // hi from child

// the parent method is also available in the Child class, as the Child extends the Parent class
child.parentMethod(); // hi from parent
```

### Override a method in a parent class

We can also override a method in a parent class:

```js
class Parent {
  constructor(name) {
    this.name = name + ` this is a parent class`;
  }
  method() {
    console.log(`This will be overridden`);
  }
}

class Child extends Parent {
  method() {
    console.log(`Child method overrode the parent method`);
  }
}

const child = new Child();

child.method(); // Child method overrode the parent method
```

### Extend the method in a parent class

What if we don't want to override the parent method, but to extend the functionality of it. We can use `super.<method>` to call the method and then add more functionality to it:

```js
class Parent {
  constructor(name) {
    this.name = name + ` this is a parent class`;
  }
  sayHi() {
    console.log(`hi from parent`);
  }
}

// super.method(...) to call a parent method.
class Child extends Parent {
  bye() {
    console.log(`bye from child`);
  }

  sayBye() {
    super.sayHi();
    this.bye();
  }
}

const child = new Child();
child.sayBye(); // hi from parent, bye from child
```

Constructors in **inheriting classes** must call `super(...)` before using `this`.

```js
class Animal {
  constructor(name) {
    this.speed = 0;
    this.name = name;
  }

  // ...
}

class Rabbit extends Animal {
  constructor(name, earLength) {
    // super(...) to call a parent constructor (inside our constructor only).
    super(name);
    this.earLength = earLength;
  }

  // ...
}

const rabbit = new Rabbit("White Rabbit", 10);

console.log(rabbit.speed); // 0
console.log(rabbit.name); // White Rabbit
console.log(rabbit.earLength); // 10
```

<hr>

### Static methods and properties

We can also assign a method to the class that won't be inherited by objects. Such methods are called **static**. Usually, static methods are used to implement functions that belong to the class as a whole, but not to any particular object of it. Static methods and properties are inherited by extended classes. In a class declaration, they are prepended by `static` keyword like this:

```js
class User {
  static staticMethod() {
    console.log(`this is a STATIC method in the User class constructor`);
  }
}

class User2 extends User {
  method() {
    console.log(`this is a method in the User2 class constructor`);
  }
}

User.staticMethod(); // this is a STATIC method in the User class constructor
User2.staticMethod(); // this is a STATIC method in the User class constructor

const user = new User();
// this throws an error
user.staticMethod();
```

Static properties are also possible, they look like regular class properties, but prepended by the keyword `static`:

```js
class User {
  static prop = "Some Name";
}

class User2 extends User {
  method() {
    console.log(`this is a method in the User2 class constructor`);
  }
}

console.log(User.prop); // Some Name
console.log(User2.prop); // Some Name

const user = new User();
console.log(user.prop); // undefined
```

<hr>

### Protected properties

We can have **protected properties** in classes. Protected properties are usually prefixed with an underscore `_`. Here is an example of a protected property. Here we control that the `wateramount` is not below zero:

```js
class CoffeeMachine {
  constructor(power) {
    this.power = power;
  }

  _waterAmount = 0;

  set waterAmount(value) {
    this._waterAmount += value;
    if (this._waterAmount < 0) {
      this._waterAmount = 0;
    }
  }

  get waterAmount() {
    return this._waterAmount;
  }
}

// create the coffee machine
const coffeeMachine = new CoffeeMachine(100);

// add water
coffeeMachine.waterAmount = -10; // _waterAmount will become 0, not -10
```

<hr>

It sometimes happens that a property must be set at creation time only, and then never be modified. To do so, we only need to make a getter, but not a setter. Here the `power` property becomes read-only:

```js
class CoffeeMachine {
  constructor(power) {
    this._power = power;
  }

  get power() {
    return this._power;
  }
}

// create the coffee machine
const coffeeMachine = new CoffeeMachine(100);
console.log(`Power is: ${coffeeMachine.power}W`); // Power is: 100W

coffeeMachine.power = 25; // Error (no setter)
```

But most of the time `get...`/`set...` functions are preferred to be like this:

```js
class CoffeeMachine {
  constructor(power) {
    this._power = power;
  }

  getPower() {
    return this._power;
  }

  _waterAmount = 0;

  setWaterAmount(value) {
    this._waterAmount += value;
    this._waterAmount < 0 ? (this._waterAmount = 0) : this._waterAmount;
  }

  getWaterAmount() {
    return this._waterAmount;
  }
}

const coffeeMachine = new CoffeeMachine(100);
console.log(coffeeMachine.getPower());

coffeeMachine.setWaterAmount(-1000);
console.log(coffeeMachine.getWaterAmount());
```

<hr>

### Private properties

There are also private properties. Privates should start with `#`. They are only accessible from inside the class.

```js
class CoffeeMachine {
  #waterLimit = 200;

  _waterAmount = 0;

  #fixWaterAmount(value) {
    this._waterAmount += value;

    this._waterAmount < 0 ? (this._waterAmount = 0) : this._waterAmount;
    this._waterAmount > this.#waterLimit
      ? (this._waterAmount = this.#waterLimit)
      : this._waterAmount;

    return this._waterAmount;
  }

  setWaterAmount(value) {
    this._waterAmount = this.#fixWaterAmount(value);
  }

  getWaterAmount() {
    return this._waterAmount;
  }
}

const coffeeMachine = new CoffeeMachine();

coffeeMachine.setWaterAmount(100);
console.log(coffeeMachine.getWaterAmount()); // 100

coffeeMachine.setWaterAmount(-100);
console.log(coffeeMachine.getWaterAmount()); // 0

coffeeMachine.setWaterAmount(300);
console.log(coffeeMachine.getWaterAmount()); // 200

// can't access privates from outside of the class
coffeeMachine.#fixWaterAmount(13); // Error
coffeeMachine.#waterLimit = 1000; // Error
```

<hr>

### Extend built-in classes

We can add more functionality to the built-in classes like Array, Map and others using the `extends` keyword.

```js
class PowerArray extends Array {
  isEmpty() {
    return this.length === 0;
  }
}

const arrClass = new PowerArray(1, 2, 3, 4, 5);
console.log(arrClass.isEmpty()); // false
```

<hr>

### `instanceof`

The `instanceof` operator allows to check whether an object belongs to a certain class. It also takes inheritance into account.

```js
class Rabbit {}
const rabbit = new Rabbit();

// is it an object of Rabbit class?
console.log(rabbit instanceof Rabbit); // true
```

It also works with constructor functions instead of classes.

```js
function Rabbit() {}

console.log(new Rabbit() instanceof Rabbit); // true
```

It also works with built-in classes like Array:

```js
const arr = [1, 2, 3];

console.log(arr instanceof Array); // true
```

<hr>

### Mixin

A **mixin** is a class, containing methods that can be used by other classes, without a need to inherit from it.

```js
const sayHiMixin = {
  sayHi() {
    console.log(`Hello ${this.name}`);
  },
  sayBye() {
    console.log(`Bye ${this.name}`);
  },
};

// usage:
class User {
  constructor(name) {
    this.name = name;
  }
}

// copy the methods
Object.assign(User.prototype, sayHiMixin);

// now User can say hi
new User("someone").sayHi(); // Hello, someone
```

<hr>
<hr>

## Error handling

### `try...catch()`, and properties of an error object

To handle the errors, we can use `try...catch()` or `try...catch()...finally` block. For all built-in errors, the error object has two main properties: `name`, and `message`. There are other non-standard properties available in the most environments. One of the most widely used and supported is `stack`:

```js
try {
  console.log(`try runs`);
} catch (err) {
  console.log(`if there is an error this part of the code catches it`);
  console.log(err.name);
  console.log(err.message);
  console.log(err.stack);
  console.log(err);
} finally {
  console.log(`finally always runs`);
}
```

```js
try {
  // throw an error to see the catch block working
  throw new Error("custom message");
} catch (err) {
  console.log(`if there is an error this part of the code catches it`);
  console.log(err.name);
  console.log(err.message);
  console.log(err.stack);
  console.log(err);
} finally {
  console.log(`finally always runs`);
}
```

<hr>

### `try...catch()` and asynchronous code

`try...catch()` works synchronously. If an exception happens in a “scheduled” code, like in `setTimeout`, then `try...catch()` won’t catch it. That’s because the function itself is executed later, when the engine has already left the `try...catch()` construct. To catch an exception inside a scheduled function, `try...catch()` must be inside that function:

```js
setTimeout(function () {
  try {
    undefinedVariable; // try...catch handles the error!
  } catch (err) {
    console.log("Here is the error: " + err);
  }
}, 1000);
```

<hr>

### `catch` without parentheses

If we don’t need the error details, `catch` might be used without parentheses:

```js
try {
  undefinedVariable;
} catch {
  console.log(`catch runs`);
} finally {
  console.log(`finally always runs`);
}
```

<hr>

### `throw` operator and different built-in error constructors

The `throw` operator generates an error. JavaScript has many built-in constructors for standard errors: `Error`, `SyntaxError`, `ReferenceError`, `TypeError` and others. We can use them to throw our own errors, if needed:

```js
try {
  console.log(`we can throw our own errors if needed`);

  if (!someVariable) {
    throw new SyntaxError(`custom Syntax Error message`);
  }
} catch (err) {
  if (!(err instanceof SyntaxError)) {
    throw new Error(`This is not a Syntax Error, do something else`);
  }

  console.log(`Here is the syntax error message: ${err.message}`);
}
```

<hr>
<hr>

## Promises, async/await

### Quick intro to promise

Here is an example of using `Promise`. The function passed to `new Promise` is called the executor. When a `new Promise` is created, the executor runs automatically. Its arguments `resolve` and `reject` are callbacks provided by the JavaScript itself. When the executor obtains the result, it should call one of these callbacks:

- `resolve(value)` — if the job is finished successfully, with the result `value`.
- `reject(error)` — if an error has occurred, error is the `error` object.

```js
const promise = new Promise(function (resolve, reject) {
  resolve("done");
}).then(
  function (result) {
    console.log(`result is ${result}`);
  },
  function (error) {
    console.log(`error is ${error}`);
  }
);
```

The executor should call only one `resolve` or one `reject`. Any state change is final. All further calls of `resolve` and `reject` are ignored.

```js
const promise = new Promise(function (resolve, reject) {
  resolve("done");
  reject("this doesn't run");
}).then(
  function (result) {
    console.log(`result is ${result}`);
  },
  function (error) {
    console.log(`error is ${error}`);
  }
);
```

<hr>

### Internal properties of a returned promise object

The promise object returned by the new Promise constructor has these internal properties:

- `state` — initially "pending", then changes to either "fulfilled" when resolve is called or "rejected" when reject is called.
- `result` — initially `undefined`, then changes to `value` when `resolve(value)` is called or `error` when `reject(error)` is called.

The properties `state` and `result` of the `Promise` object are internal. We can’t directly access them. We can use the methods `.then`/`.catch`/`.finally` for that.

The first argument of `.then` is a function that runs when the promise is resolved and receives the result. The second argument of `.then` is a function that runs when the promise is rejected and receives the error.

```js
const promise = new Promise(function (resolve, reject) {
  setTimeout(() => resolve("done!"), 1000);
});

// the first function runs because promise resolves
promise.then(
  function (result) {
    console.log(`result is ${result}`);
  },
  function (error) {
    console.log(`error is ${error}`);
  } // doesn't run because promise is not rejected
);
```

```js
const promise = new Promise(function (resolve, reject) {
  setTimeout(() => reject(new Error("Custom Error Message")), 1000);
});

// the second function runs
promise.then(
  function (result) {
    console.log(`result is ${result}`); // doesn't run
  },
  function (error) {
    console.log(`error is ${error}`); // "Custom Error Message" after 1 second
  }
);
```

### `.then` without catching the promise rejection

`.then` accepts 2 functions: one to handle the result from a resolved promise, and the second one to handle the promise rejection. However, we can also use `.then` with one function alone, if we don't want to control for a possible error:

```js
const promise = new Promise(function (resolve, reject) {
  setTimeout(() => resolve("done!"), 1000);
});

promise.then(function (result) {
  console.log(`result is ${result}`);
});
```

### Chained `then`s

We can have chained `then`s as well:

```js
const promise = new Promise(function (resolve, reject) {
  resolve("done");
})
  .then(function (result) {
    return `this goes to the next function in the chain with the result: ${result}`;
  })
  .then(function (result) {
    console.log(
      `This is from the second "then". This is what was returned from the first "then": ${result}`
    );
  });
```

### Controlling for errors using `.then`

If we’re interested only in errors, then we can use `null` as the first argument to the `.then`: `.then(null, errorHandlingFunction)`. Or we can use `.catch(errorHandlingFunction)`, which is exactly the same:

```js
const promise = new Promise(function (resolve, reject) {
  setTimeout(() => reject(new Error("Custom Error Message")), 1000);
});

// the second function runs
promise.then(
  null, // doesn't run
  function (error) {
    console.log(`error: ${error}`);
  }
);
```

```js
const promise = new Promise(function (resolve, reject) {
  setTimeout(() => reject(new Error("Custom Error Message")), 1000);
});

// catch runs
promise.catch(
    console.log(`error: ${error}`);
);
```

### `.then` after `.catch`

Usually, we define the `then` part of the promise and after that define the `catch`. However, we can use `.then` after a `.catch` as well:

```js
const promise = new Promise((resolve, reject) => {
  throw new Error("Custom Error Message");
})
  .catch(function (error) {
    console.log(error);
    return `this is not an error, keep running`;
  })
  .then((result) => {
    console.log("Final `then` runs");
    console.log(result);
  });
```

Moreover, we can define `then`, after that `catch`, and after that one more `then` again:

```js
const promise = new Promise((resolve, reject) => {
  throw new Error("Custom Error Message");
})
  .then(function (result) {
    console.log(`this doesn't run`);
  })
  .catch(function (error) {
    console.log(error);
    return `this is not an error, keep running`;
  })
  .then((result) => {
    console.log("Final `then` runs");
    console.log(result);
  });
```

### `finally`

`finally` always runs, and it shouldn't return anything. If it returns something, it will be ignored.

```js
const promise = new Promise(function (resolve, reject) {
  reject("error");
})
  .then(function (result) {
    console.log(result);
  })
  .catch(function (error) {
    console.log(error);
  })
  .finally(function () {
    console.log(`will run anyway`);
    // finally shouldn't return anything, if returns it will be ignored
  });
```

<hr>

### A promise inside a promise

A handler function, used in `.then(<handler>)` may create and return a promise. In that case further handlers wait until it settles, and then get its result.

```js
const promise = new Promise(function (resolve, reject) {
  resolve("1st promise");
})
  .then(function (result) {
    console.log(result);
    return new Promise(function (resolve, reject) {
      resolve("2nd promise");
    });
  })
  .then(function (result) {
    console.log(result);
  });
```

<hr>

### `Promise.all`

`Promise.all` takes an iterable (usually, an array of promises) and returns a new promise. The new promise resolves when all listed promises are resolved, and the array of their results becomes its result. If any promise is rejected, all gets rejected.

```js
const arrOfPromises = [
  new Promise((resolve, reject) => setTimeout(() => resolve(1), 1000)),
  new Promise((resolve, reject) => setTimeout(() => resolve(2), 1500)),
  new Promise((resolve, reject) => setTimeout(() => resolve(3), 2000)),
];

// executes promises in parallel and waits until all of them are ready.
// If any promise is rejected, all gets rejected.
Promise.all(arrOfPromises)
  .then((res) => console.log(res)) // [1, 2, 3]
  .catch((err) => console.log(err));
```

```js
const arrOfPromises = [
  new Promise((resolve, reject) => setTimeout(() => resolve(1), 1000)),
  new Promise((resolve, reject) =>
    setTimeout(() => reject(new Error("Rejected with an Error")), 1500)
  ),
  new Promise((resolve, reject) => setTimeout(() => resolve(3), 2000)),
];

// executes promises in parallel and waits until all of them are ready.
// If any promise is rejected, all gets rejected.
Promise.all(arrOfPromises)
  .then((res) => console.log(res))
  .catch((err) => console.log(err)); // Error: Rejected with an Error
```

`Promise.all(...)` accepts an iterable (in most cases an array) of promises. But it also accepts non-`Promise` items. Those non-`Promise` items are passed to the resulting array “as is”.

```js
Promise.all([
  new Promise((resolve, reject) => {
    setTimeout(() => resolve(1), 1000);
  }),
  2,
  3,
]).then(console.log); // 1, 2, 3
```

<hr>

### `Promise.allSettled`

`Promise.allSettled` waits for all promises to settle, regardless of the result. The resulting array has:

- `{status:"fulfilled", value:result}` for successful responses,
- `{status:"rejected", reason:error}` for errors.

```js
const arrOfPromises = [
  new Promise((resolve, reject) => setTimeout(() => resolve(1), 1000)),
  new Promise((resolve, reject) =>
    setTimeout(() => reject(new Error("Rejected with an Error")), 1500)
  ),
  new Promise((resolve, reject) => setTimeout(() => resolve(3), 2000)),
];

Promise.allSettled(arrOfPromises).then(console.log);
```

<hr>

### `Promise.race()`

`Promise.race()` waits only for the first settled promise and gets its result. If there is an error, then it returns the error:

```js
const arrOfPromises = [
  new Promise((resolve, reject) => setTimeout(() => resolve(1), 1000)),
  new Promise((resolve, reject) =>
    setTimeout(() => reject(new Error("Rejected with an Error")), 1500)
  ),
  new Promise((resolve, reject) => setTimeout(() => resolve(3), 2000)),
];

Promise.race(arrOfPromises).then(console.log);
```

<hr>

### `Promise.any`

`Promise.any` waits only for the first fulfilled promise and gets its result. If all of the given promises are rejected, then the returned promise is rejected with the `AggregateError` – a special error object that stores all promise errors in its `errors` property.

```js
const arrOfPromises = [
  new Promise((resolve, reject) => setTimeout(() => resolve(1), 1000)),
  new Promise((resolve, reject) =>
    setTimeout(() => reject(new Error("Rejected with an Error")), 1500)
  ),
  new Promise((resolve, reject) => setTimeout(() => resolve(3), 2000)),
];

Promise.any(arrOfPromises)
  .then((res) => console.log(`fulfilled result ${res}`))
  .catch((error) => {
    console.log(error.constructor.name);
    console.log(error.errors[0]);
  });
```

<hr>

### `async`/`await`

`async`/`await` is a more comfortable special syntax to work with promises. Async functions are defined by putting the word `async` before the function. `async` before a function means that a function always returns a promise.

```js
async function asyncFunc() {
  return 1; // same as return Promise.resolve(1)
}
```

`async` functions also can use `.then` and `.catch`:

```js
async function asyncFunc() {
  return 1; // same as return Promise.resolve(1)
}

asyncFunc().then(console.log).catch(console.log);
```

The `await` keyword makes JavaScript wait until the promise settles and returns its result. `await` can only be used inside an `async` function.

```js
async function asyncFunc() {
  const promise = new Promise((resolve, reject) => {
    setTimeout(() => resolve("done!"), 1000);
  });

  const result = await promise; // wait until the promise resolves

  console.log(result); // "done!"
}

asyncFunc();
```

<hr>
<hr>

## Generators

### Intro to generators

Regular functions return single value (or nothing). Generators can return (`yield`) multiple values, one after another, on-demand. To create a generator, we use `function*`, so-called “generator function”.

```js
function* generatorFunc() {
  yield 1;
  yield 2;
  return 3;
}
```

<hr>

When a generator function is called, it doesn’t run its code. It returns a special object, called “generator object”, to manage the execution.

```js
function* generatorFunc() {
  yield 1;
  yield 2;
  return 3;
}

const generator = generatorFunc();
console.log(generator); // // [object Generator]
```

<hr>

### `next()`

To run the code of a generator, we use the `next()` method. When called, it runs the execution until the nearest `yield <value>` statement and returns the yielded value. The result of `next()` is always an object with two properties:

- `value`: the yielded value.
- `done`: `true` if the function code has finished, otherwise `false`.

```js
function* generatorFunc() {
  yield 1;
  yield 2;
  return 3;
}

const generator = generatorFunc();

console.log(generator.next()); // {value: 1, done: false}
console.log(generator.next()); // {value: 2, done: false}
console.log(generator.next()); // {value: 3, done: true}
```

After the final return value is reached, if the `next()` method is used again, it will return `{value: undefined, done: true}`.

<hr>

### Looping over generators

Generators are iterable. We can loop over their values using `for..of`:

```js
function* generatorFunc() {
  yield 1;
  yield 2;
  return 3;
}

const generator = generatorFunc();

for (let value of generator) {
  console.log(value);
  // outputs 1, 2. To output 3, yield should be used instead of return
}
```

`for..of` ignores the last value, when `done: true`. So, if we want all results to be shown by `for..of`, we must return them with `yield` not `return`.

```js
function* generatorFunc() {
  yield 1;
  yield 2;
  yield 3;
}

const generator = generatorFunc();

for (let value of generator) {
  console.log(value);
  // outputs 1, 2, 3
}
```

<hr>

### Spread syntax with generators

As generators are iterable, we can also use the spread syntax `...` with them:

```js
function* generatorFunc() {
  yield 1;
  yield 2;
  return 3;
}

const generator = generatorFunc();

const arrFilledByGenerator = [0, ...generator];

// To have 3 in the array, `yield` should be used instead of `return`
console.log(arrFilledByGenerator); // [0, 1, 2]
```

<hr>

### Generator in a generator

Generator composition allows to have generators in each other. There’s a special `yield*` syntax to embed one generator into another one. The `yield*` directive delegates the execution to another generator. In other words, `yield* <gen>` iterates over the generator `<gen>` and transparently forwards its yields outside, as if the values were yielded by the outer generator.

```js
function* generatorFunc(start, end) {
  for (let i = start; i <= end; i++) yield i;
}

function* genWithinGen() {
  yield* generatorFunc(40, 60);
}

const generator = genWithinGen();

console.log(generator.next()); // { value: 40, done: false }
console.log(generator.next()); // { value: 41, done: false }
```

<hr>

### Passing an argument to a generator

`yield` not only returns the result to the outside, but also can pass the value inside the generator. To pass a value inside, we should call `generator.next(<arg>)`, with an argument. That argument becomes the result of `yield`.

```js
function* generatorFunc() {
  let result = yield `2 + 2 = ?`;

  console.log(result);
}

const generator = generatorFunc();
console.log(generator.next().value); // here the value returns the yielded "2 + 2 = ?"
generator.next(4); // 4 passed inside and becomes the result, after which it is logged to the console
```

The first call `generator.next()` should always be made without an argument. The argument is ignored if passed.

<hr>

### Pass an error to the generator

We can also pass an error to the generator. To pass an error into a `yield`, we should call `generator.throw(<err>)`.

```js
function* generatorFunc() {
  try {
    let result = yield `2 + 2 = ?`;
    console.log(result);
  } catch (error) {
    console.log(error);
  }
}

const generator = generatorFunc();
generator.next().value;

generator.throw(new Error("Custom Error message"));
```

<hr>

### Finishing a generator early

Even if a generator has more values to yield, we can finish it using the `generator.return(<arg>)`. It returns the provided `<arg>`:

```js
function* generatorFunc() {
  yield 1;
  yield 2;
  yield 3;
}

const generator = generatorFunc();
console.log(generator.next()); // { value: 1, done: false }

// generator.return(value) finishes the generator execution and returns the given value.
console.log(generator.return("The End")); // { value: "The End", done: true }

console.log(generator.next()); // { value: undefined, done: true }
```

<hr>
<hr>

## Modules

- A module is a javascript file.
- Modules always work in strict mode.
- Each module has its own top-level scope. In other words, top-level variables and functions from a module are not seen in other scripts. Modules should `export` what they want to be accessible from outside and `import` what they need.

<hr>

### `import.meta`

The object `import.meta` contains the information about the current module.

Its content depends on the environment. In the browser, it contains the URL of the script, or a current webpage URL if inside HTML:

```html
<script type="module">
  console.log(import.meta.url); // script URL
  // for an inline script - the URL of the current HTML-page
</script>
```

If you are using the `import.meta` inside a JS file, make sure that the `script` tag, within the html file, referring to the JS file include `type="module"`. Otherwise, an error will pop up saying "Cannot use `'import.meta'` outside a module.

<hr>

### `this` in modules

In a module, top-level `this` is undefined. In non-module scripts, `this` is a global object:

```html
<script>
  console.log(this); // window
</script>

<script type="module">
  console.log(this); // undefined
</script>
```

<hr>

### Browser-specific differences of scripts with `type="module"`

There are several browser-specific differences of scripts with `type="module"` compared to regular scripts.

- Module scripts are always deferred, same effect as `defer` attribute, for both external and inline scripts.

  - downloading external module scripts `<script type="module" src="...">` doesn’t block HTML processing, they load in parallel with other resources.
  - module scripts wait until the HTML document is fully ready, and then run.
  - relative order of scripts is maintained: scripts that go first in the document, execute first.

```html
<script type="module">
  const button = document.querySelector("button");
  console.log(button);
  // as modules are deferred, the script runs after the whole page is loaded
</script>
<button id="button">Button</button>
```

Compare to regular script below:

```html
<script>
  const button = document.querySelector("button");
  console.log(button);
  // button is null, the script can't see elements below
  // regular scripts run immediately, before the rest of the page is processed
</script>

<button id="button">Button</button>
```

- For non-module scripts, the `async` attribute only works on external scripts. Async scripts run immediately when ready, independently of other scripts or the HTML document. For module scripts, it works on inline scripts as well.

<hr>

### Fallback for old browsers

Old browsers do not understand `type="module"`. Scripts of an unknown type are just ignored. For them, it’s possible to provide a fallback using the `nomodule` attribute:

```html
<script type="module">
  console.log("Runs in modern browsers");
</script>

<script nomodule>
  console.log(
    "Modern browsers know both type=module and nomodule, so skip this"
  );
  console.log(
    "Old browsers ignore script with unknown type=module, but execute this."
  );
</script>
```

<hr>

### Exporting and importing variables

#### `export` while declaring a variable

We can label any declaration as exported, by placing `export` before it, be it a variable, function or a class.

```js
// module.js

// export an array
export const numbers = [1, 2, 3, 4, 5];

// export a constant
export const simpleVar = "simpleVar";

// export a class
export class ClassName {
  constructor(name) {
    this.name = name;
  }
}
```

#### `export` after declaring a variable

We can put `export` after declaring the variable, as well.

```js
// module.js
function sayHi(user) {
  console.log(`Hello, ${user}`);
}

function sayBye(user) {
  console.log(`Bye, ${user}`);
}

export { sayHi, sayBye }; // a list of exported variables
```

#### `import` by name

In the above example, the exports are called named exports, as the variables were not default exported. To import named exports, we can put a list of what to import in curly braces in `import {...}`, like this:

```js
// index.js
// index.js should have type="module" in the script tag of the html file that downloads it
import { sayHi, sayBye } from "./say.js";

sayHi("Ziya"); // Hello, Ziya!
sayBye("Ziya"); // Bye, Ziya!
```

#### `import` everything at once

If there’s a lot to import, we can import everything as an object using `import * as <obj>`, for instance:

```js
// index.js
import * as obj from "./module.js";

obj.sayHi("Ziya");
obj.sayBye("Ziya");
```

#### `import` under different names

We can also use `as` to import under different names.

```js
// index.js
import { sayHi as hi, sayBye as bye } from "./module.js";

hi("Ziya");
bye("Ziya");
```

#### `export` under different names

We can also use `as` to export under different names:

```js
// module.js
function sayHi(user) {
  console.log(`Hello, ${user}`);
}

function sayBye(user) {
  console.log(`Bye, ${user}`);
}

export { sayHi as hi, sayBye as bye };
```

After the above change, now `hi` and `bye` could be used in imports:

```js
// index.js
import * as say from "./module.js";

say.hi("Ziya"); // Hello, Ziya!
say.bye("Ziya"); // Bye, Ziya!
```

<hr>

### `export default`

Sometimes, it's preferred to export one entity in a module rather than several variables. Modules provide a special `export default` (“the default export”) syntax to make the “one thing per module” way look better. There may be only one `export default` per file.

You can put `export default` before the entity to export:

```js
// module.js
export default class ClassName {
  constructor(name) {
    this.name = name;
  }
}
```

The default exports could be imported without curly braces:

```js
// index.js
import ClassName from "./module.js"; // not {ClassName}, just ClassName

const className = new ClassName("Name");
console.log(className.name);
```

**Note: `import` needs curly braces for named exports and doesn’t need them for the default one.**

As there may be at most one default export per file, the exported entity may have no name.

```js
// module.js
export default class {
  // no class name
  constructor(name) {
    this.name = name;
  }
}
```

```js
// module.js
export default function (user) {
  // no function name
  console.log(`Hello, ${user}!`);
}
```

```js
// module.js
export default ["Jan", "Feb", "Mar", "Apr", "Aug", "Sep", "Oct", "Nov", "Dec"]; // no array name
```

<hr>

`default` keyword could be used to export a variable after it's declaration:

```js
// module.js
function sayHi(user) {
  console.log(`Hello, ${user}!`);
}

// same as if we added "export default" before the function
export { sayHi as default };
```

If a file exports one “default” item, and a few named ones, we can import the default export along with a named one:

```js
// module.js
export default class User {
  constructor(name) {
    this.name = name;
  }
}

export function sayHi(user) {
  console.log(`Hello, ${user}!`);
}
```

This is how we would import the above exports:

```js
// index.js
import { default as ClassName, sayHi } from "./module.js";

console.log(new ClassName("Ziya").name);
sayHi("test");
```

If we import everything with `*` as an object, then the `default` property is exactly the default export:

```js
// index.js
import * as obj from "./module.js";

const ClassName = obj.default; // the default export
console.log(new ClassName("Ziya").name);
```

<hr>

### Re-export

“Re-export” syntax `export ... from ...` allows to import things and immediately export them:

```js
export { sayHi } from "./module.js"; // re-export sayHi
export { default as ClassName } from "./module.js"; // re-export default
```

`export ... from ...` is just a shorter form of the below way of importing and exporting:

```js
// import default as ClassName and export it
import ClassName from "./module.js";
export { ClassName };
```

The notable difference of `export ... from` compared to `import`/`export` is that re-exported modules aren’t available in the current file. So inside the above file, we can’t use the `sayHi` function.

We need to be careful about using `export ... from` with a default export.

- `export ClassName from './module.js'` won’t work. We need to use `export {default as ClassName}`
- `export * from './module.js'` re-exports only named exports, but ignores the default one. If we’d like to re-export both named and default exports, then two statements are needed:

```js
export * from "./module.js"; // to re-export named exports
export { default } from "./module.js"; // to re-export the default export
```

<hr>

### Dynamic imports

The `import()` syntax, also called dynamic import, is an expression that allows loading an ECMAScript module asynchronously and dynamically. The `import()` call is a syntax that closely resembles a function call, but `import` itself is a keyword, not a function (You cannot assign it to a variable the way you could do with a function).

The import declaration syntax (`import something from "somewhere"`) is static and will always result in the imported module being evaluated at load time. Dynamic imports allow to load a module conditionally or on demand. Use dynamic import only when necessary. The static form is preferable for loading initial dependencies, and can benefit more readily from static analysis tools and tree shaking.

If a file is referenced in an HTML file, but it doesn't have the script tag `type="module"`, then you can't use static import declaration but the asynchronous dynamic import syntax will always be available, allowing you to import modules even into non-module environments.

The `import(<module>)` expression loads the module and **returns a promise** that resolves into a module object that contains all its exports.

```js
import * as mod from "/module.js";

import("/module.js").then((mod2) => {
  console.log(mod === mod2); // true
});
```

The dynamic import syntax allows to use importing with an `if` statement. As it returns a promise, we need to use `await` with it, inside an `async` function.

```js
const condition = true;

(async () => {
  if (condition) {
    const mod = await import("./module.js");
    console.log(mod);
  }
})();
```

To dynamically import a default export, we need to use `default` keyword. For example, here we destructure and assign a different name to a default export:

```js
const condition = true;

(async () => {
  if (condition) {
    const { default: myDefault } = await import("./module.js");
    console.log(myDefault);
  }
})();
```

<hr>
<hr>

## DOM

### Accessing some topmost level tags on a webpage

- To get the topmost document node - the `<html>` tag, we can use the `document.documentElement`.
- To get the `head` element, we can use `document.head`.
- For the `body` element, we can use `document.body`.

```js
console.log(document); // HTMLDocument
console.log(document.head); // <head>
console.log(document.body); // <body>
console.log(document.documentElement); // <html lang="en">
```

<hr>

### Checking if an element or node has child nodes

If we want to check if a node has child nodes, we can use `<node>.hasChildNodes()`. It returns `true` or `false`.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.hasChildNodes()); // true
    console.log(document.body.childNodes);
    // NodeList(8) [ #text, h1, #text, p, #text, script, #text, script ]

    console.log(document.body.childNodes[0]); // #text "\n  "
    console.log(document.body.childNodes[0].hasChildNodes()); // false
    console.log(document.body.childNodes[0].childNodes); // NodeList []
  </script>
</body>
```

### Retrieving the collection of child nodes

To get collection of (immediate) child nodes of an element, we use `<node>.childNodes`.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.documentElement.childNodes); // NodeList(3) [ head, #text, body ]
    console.log(document.body.childNodes);
    // NodeList(8) [ #text, h1, #text, p, #text, script, #text, script ]
  </script>
</body>
```

We can use `for..of` to iterate over `childNodes`. But array methods won't work on it, because `childNodes` is not an array. It's a collection, and we can use `Array.from()` to create an array from it.

Here is an example of using `for..of` with `childNodes`:

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    for (let node of document.documentElement.childNodes) {
      console.log(node);
      // head, #text "\n", body
    }

    for (let node of document.body.childNodes) {
      console.log(node);
      // #text "\n", h1, #text "\n  ", p, #text "\n  ", script, #text "\n  ", script
    }
  </script>
</body>
```

Here is an example of using `Array.from()` with `childNodes`:

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.childNodes);
    // NodeList(8) [ #text, h1, #text, p, #text, script, #text, script ]

    console.log(Array.from(document.body.childNodes));
    // Array(8) [ #text, h1, #text, p, #text, script, #text, script ]
  </script>
</body>
```

<hr>

### Accessing the child nodes

`<node>.firstChild` gets the first child node. It's the same as `document.<node>.childNodes[0]`.

`<node>.lastChild` gets the last child. It's the same as `document.<node>.childNodes[document.<node>.childNodes.length-1]`.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.childNodes);
    // NodeList(8) [ #text, h1, #text, p, #text, script, #text, script ]

    console.log(document.body.firstChild); // #text "\n  "
    console.log(document.body.lastChild); // <script>

    // same as above
    console.log(document.body.childNodes[0]); // #text "\n  "
    console.log(document.body.childNodes[document.body.childNodes.length - 1]); // <script>
  </script>
</body>
```

<hr>

### Accessing the sibling nodes

To get the sibling nodes we can use `<node>.nextSibling` and `<node>.previousSibling`

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.childNodes);
    // NodeList(8) [ #text, h1, #text, p, #text, script, #text, script ]

    console.log(document.body.childNodes[1]); // <h1>

    console.log(document.body.childNodes[1].previousSibling); // #text "\n  "
    console.log(document.body.childNodes[0]); // #text "\n  ", this is the same node as the above one

    console.log(document.body.childNodes[1].nextSibling.nextSibling); // <p>
    console.log(document.body.childNodes[3]); // <p>, this is the same node as the above one
  </script>
</body>
```

<hr>

### Accessing the parent node

`<node>.parentNode` helps to get the parent node.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.childNodes);
    // NodeList(8) [ #text, h1, #text, p, #text, script, #text, script ]

    console.log(document.body.childNodes[0]); // #text
    console.log(document.body.childNodes[0].parentNode); // <body>

    console.log(document.body.childNodes[1]); // <h1>
    console.log(document.body.childNodes[1].parentNode); // <body>
  </script>
</body>
```

<hr>

### Working with child elements

Navigation properties listed above refer to all nodes. For instance, in `childNodes` we can see text nodes, element nodes, and even comment nodes, if they exist. But for many tasks, we don’t want text or comment nodes. We want to manipulate element nodes that represent tags and form the structure of the page.

To get the element nodes of an element, we can use `<node>.children`.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.childNodes);
    // NodeList(8) [ #text, h1, #text, p, #text, script, #text, script ]

    console.log(document.body.children);
    // HTMLCollection(4) [h1, p, script, script]
  </script>
</body>
```

<hr>

### Accessing the child elements

- `<node>.firstElementChild` helps to get the first child element.
- `<node>.lastElementChild` helps to get the last child element.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.firstElementChild); // <h1>
    console.log(document.body.lastElementChild); // <script>

    console.log(document.body.children[0]); // <h1>
    console.log(document.body.children[document.body.children.length - 1]); // <script>
  </script>
</body>
```

<hr>

### Accessing the sibling elements

`<node>.previousElementSibling` and `<node>.nextElementSibling` help to get neighboring elements.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.children);
    // HTMLCollection { 0: h1, 1: p, 2: script, 3: script, length: 4 }

    console.log(document.body.children[1]); // <p>

    console.log(document.body.children[1].previousElementSibling); // <h1>
    console.log(document.body.children[0]); // <h1>, this is the same node as the above one

    console.log(document.body.children[1].nextElementSibling); // <script src="./index.js">
    console.log(document.body.children[2]); // <script src="./index.js">, this is the same node as the above one
  </script>
</body>
```

<hr>

### Accessing the parent element

`<node>.parentElement` helps to get the parent element.

```html
<body>
  <h1>Heading</h1>
  <p>Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.children);
    // HTMLCollection { 0: h1, 1: p, 2: script, 3: script, length: 4 }

    console.log(document.body.children[0]); // <h1>
    console.log(document.body.children[0].parentElement); // <body>

    console.log(document.body.children[1]); // <p>
    console.log(document.body.children[1].parentElement); // <body>
  </script>
</body>
```

<hr>

### Accessing the element by its `id`

`document.getElementById("<Id>")` gets the element with the specific Id. Also, `window.<Id>`, `window[<Id>]` and even `<Id>` alone work but they are not advisable.

```html
<body>
  <h1 id="heading">Heading</h1>
  <p id="paragraph">Paragraph</p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.children);
    // HTMLCollection { 0: h1#heading, 1: p#paragraph, 2: script, 3: script, length: 4, … }

    const headingElem = document.getElementById("heading");
    console.log(headingElem); // <h1 id="heading">

    // These are not preferred, but possible
    console.log(window.heading); // <h1 id="heading">
    console.log(window["heading"]); // <h1 id="heading">
    console.log(heading); // <h1 id="heading">
  </script>
</body>
```

<hr>

### Table properties

There are also some element-specific properties. For example, `<table>` tag has its own properties that helps to access and manipulate table-related tags.

- `<table>.caption` - reference to the `<caption>` element.
- `<table>.tHead` - reference to the `<thead>` element.
- `<table>.tBodies` - the collection of `<tbody>` elements
- `<table>.tFoot` - reference to the `<tfoot>` element.

These properties help to select different parts of a table:

```html
<style>
  table {
    border: 1px solid black;
    border-collapse: collapse;
  }

  th,
  td {
    border: 1px solid black;
  }
</style>
<body>
  <table id="tableId">
    <caption>
      Title for the Table
    </caption>
    <thead>
      <tr>
        <th scope="col" rowspan="2">Header 1</th>
        <th scope="col" colspan="2">Header 2</th>
        <th scope="col" rowspan="2">Header 3</th>
      </tr>
      <tr>
        <th scope="col">Subheader 2.1</th>
        <th scope="col">Subheader 2.2</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Cell 1.1</th>
        <td>Cell 1.2</td>
        <td>Cell 1.3</td>
        <td>Cell 1.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 2.1</th>
        <td>Cell 2.2</td>
        <td>Cell 2.3</td>
        <td>Cell 2.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 3.1</th>
        <td>Cell 3.2</td>
        <td>Cell 3.3</td>
        <td>Cell 3.4</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <th colspan="3">Footer Header</th>
        <td>Footer cell</td>
      </tr>
    </tfoot>
  </table>

  <script src="./index.js"></script>
  <script>
    const table = document.getElementById("tableId");
    console.log(table); // <table id="tableId">

    // different parts of the table
    console.log(table.caption); // <caption>
    console.log(table.tHead); // <thead>
    console.log(table.tBodies); // HTMLCollection { 0: tbody, length: 1 }
    console.log(table.tBodies[0]); // <tbody>
    console.log(table.tFoot); // <tfoot>
  </script>
</body>
```

The rows of the table as a whole or the rows within different parts of the table could be selected as well, using the `rows` property:

- `<table>.rows` - the collection of `<tr>` elements of the table.
- `<thead>.rows` - the collection of `<tr>` inside `<thead>`.
- `<tbody>.rows` - the collection of `<tr>` inside `<tbody>`.
- `<tfoot>.rows` - the collection of `<tr>` inside `<tfoot>`.

```html
<body>
  <table id="tableId">
    <caption>
      Title for the Table
    </caption>
    <thead>
      <tr>
        <th scope="col" rowspan="2">Header 1</th>
        <th scope="col" colspan="2">Header 2</th>
        <th scope="col" rowspan="2">Header 3</th>
      </tr>
      <tr>
        <th scope="col">Subheader 2.1</th>
        <th scope="col">Subheader 2.2</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Cell 1.1</th>
        <td>Cell 1.2</td>
        <td>Cell 1.3</td>
        <td>Cell 1.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 2.1</th>
        <td>Cell 2.2</td>
        <td>Cell 2.3</td>
        <td>Cell 2.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 3.1</th>
        <td>Cell 3.2</td>
        <td>Cell 3.3</td>
        <td>Cell 3.4</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <th colspan="3">Footer Header</th>
        <td>Footer cell</td>
      </tr>
    </tfoot>
  </table>

  <script src="./index.js"></script>
  <script>
    const table = document.getElementById("tableId");
    console.log(table); // <table id="tableId">

    // collection of rows
    console.log(table.rows);
    // HTMLCollection { 0: tr, 1: tr, 2: tr, 3: tr, 4: tr, 5: tr, length: 6 }

    console.log(table.tHead.rows); // HTMLCollection { 0: tr, 1: tr, length: 2 }
    console.log(table.tBodies[0].rows); // HTMLCollection { 0: tr, 1: tr, 2: tr, length: 3 }
    console.log(table.tFoot.rows); // HTMLCollection { 0: tr, length: 1 }
  </script>
</body>
```

We can also retrieve the row number of a `<tr>` tag:

- `<tr>.sectionRowIndex` - the position (index) of the given `<tr>` inside the enclosing `<thead>`/`<tbody>`/`<tfoot>`.
- `<tr>.rowIndex` - the number of the `<tr>` in the table as a whole (including all table rows).

```html
<body>
  <table id="tableId">
    <caption>
      Title for the Table
    </caption>
    <thead>
      <tr>
        <th scope="col" rowspan="2">Header 1</th>
        <th scope="col" colspan="2">Header 2</th>
        <th scope="col" rowspan="2">Header 3</th>
      </tr>
      <tr>
        <th scope="col">Subheader 2.1</th>
        <th scope="col">Subheader 2.2</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Cell 1.1</th>
        <td>Cell 1.2</td>
        <td>Cell 1.3</td>
        <td>Cell 1.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 2.1</th>
        <td>Cell 2.2</td>
        <td>Cell 2.3</td>
        <td>Cell 2.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 3.1</th>
        <td>Cell 3.2</td>
        <td>Cell 3.3</td>
        <td>Cell 3.4</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <th colspan="3">Footer Header</th>
        <td>Footer cell</td>
      </tr>
    </tfoot>
  </table>

  <script src="./index.js"></script>
  <script>
    const table = document.getElementById("tableId");
    console.log(table); // <table id="tableId">

    // collection of rows
    console.log(table.rows);
    // HTMLCollection { 0: tr, 1: tr, 2: tr, 3: tr, 4: tr, 5: tr, length: 6 }

    // The row number of `<tr>` inside the enclosing `<thead>`/`<tbody>`/`<tfoot>`
    console.log(table.tHead.rows[0].sectionRowIndex); // 0
    console.log(table.tHead.rows[1].sectionRowIndex); // 1

    // the row number of the `<tr>` in the table as a whole
    console.log(table.tHead.rows[0].rowIndex); // 0

    // the difference between sectionRowIndex and rowIndex
    console.log(table.tFoot.rows[0].sectionRowIndex); // 0
    console.log(table.tFoot.rows[0].rowIndex); // 5
  </script>
</body>
```

We can also select the individual cells, and retrieve the number of a cell within the row:

- `<tr>.cells` - the collection of `<td>` and `<th>` cells inside the given `<tr>`.
- `td.cellIndex` - the number of a cell inside the enclosing `<tr>`.

```html
<body>
  <table id="tableId">
    <caption>
      Title for the Table
    </caption>
    <thead>
      <tr>
        <th scope="col" rowspan="2">Header 1</th>
        <th scope="col" colspan="2">Header 2</th>
        <th scope="col" rowspan="2">Header 3</th>
      </tr>
      <tr>
        <th scope="col">Subheader 2.1</th>
        <th scope="col">Subheader 2.2</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Cell 1.1</th>
        <td>Cell 1.2</td>
        <td>Cell 1.3</td>
        <td>Cell 1.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 2.1</th>
        <td>Cell 2.2</td>
        <td>Cell 2.3</td>
        <td>Cell 2.4</td>
      </tr>
      <tr>
        <th scope="row">Cell 3.1</th>
        <td>Cell 3.2</td>
        <td>Cell 3.3</td>
        <td>Cell 3.4</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <th colspan="3">Footer Header</th>
        <td>Footer cell</td>
      </tr>
    </tfoot>
  </table>

  <script src="./index.js"></script>
  <script>
    const table = document.getElementById("tableId");
    console.log(table); // <table id="tableId">

    // collection of cells
    console.log(table.tHead.rows[0].cells); // HTMLCollection { 0: th, 1: th, 2: th, length: 3 }
    console.log(table.tBodies[0].rows[0].cells); // HTMLCollection { 0: th, 1: td, 2: td, 3: td, length: 4 }
    console.log(table.tFoot.rows[0].cells); // HTMLCollection { 0: th, 1: td, length: 2 }

    // individual cells
    console.log(table.tHead.rows[0].cells[0]); // < th scope = "col" rowspan = "2" >

    // the cell number inside the enclosing <tr>
    console.log(table.tHead.rows[0].cells[0].cellIndex); // 0
    console.log(table.tHead.rows[0].cells[1].cellIndex); // 1

    console.log(table.tHead.rows[1].cells[0].cellIndex); // 0
    console.log(table.tHead.rows[1].cells[1].cellIndex); // 1
  </script>
</body>
```

<hr>

### Select elements using CSS selectors

Below two DOM methods are very useful. Using these we access the HTML elements using the elements' CSS selectors.

- `querySelectorAll("<css>")` returns all elements inside body matching the given CSS selector.
- `querySelector("<css>")` returns the first element inside body matching the given CSS selector.

```html
<body>
  <h1 id="headingId">Heading</h1>

  <section class="paragraphsSection">
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
    <p>Paragraph 3</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const paragraphs = document.querySelectorAll("p");
    console.log(paragraphs); // NodeList(3) [ p, p, p ]

    const heading = document.querySelector("#headingId");
    console.log(heading); // <h1 id="headingId">

    const paragraphsSection = document.querySelector(".paragraphsSection");
    console.log(paragraphsSection); // <section class="paragraphsSection">
  </script>
</body>
```

<hr>

### Check if an element matches a CSS selector

`matches("<css>")` checks if an element matches the given CSS-selector.

```html
<body>
  <h1 id="headingId">Heading</h1>

  <script src="./index.js"></script>
  <script>
    const heading = document.querySelector("#headingId");
    console.log(heading.matches("#headingId")); // true
    console.log(heading.matches("h1")); // true
  </script>
</body>
```

<hr>

### Select the nearest ancestor that matches a CSS selector

`closest("<css>")` looks for the nearest ancestor that matches the CSS-selector. The element itself is also included in the search.

```html
<body>
  <section class="outerSection">
    <section>
      <h2>Paragraph Heading</h2>
    </section>
    <section class="innerSection">
      <p>Paragraph 1</p>
      <p>Paragraph 2</p>
      <p>Paragraph 3</p>
    </section>
  </section>

  <script src="./index.js"></script>
  <script>
    const firstParagraph = document.querySelector("p");
    console.log(firstParagraph.closest("section")); // <section class="innerSection">
  </script>
</body>
```

<hr>

### Select the HTML of an element

- `innerHTML` gets the HTML inside the element as a string. Only valid for element nodes.
- `outerHTML` gets the same as `innerHTML` plus the element itself.

```html
<body>
  <section class="outerSection">
    <section>
      <h2>Paragraph Heading</h2>
    </section>
    <section class="innerSection">
      <p>Paragraph 1</p>
      <p>Paragraph 2</p>
      <p>Paragraph 3</p>
    </section>
  </section>

  <script src="./index.js"></script>
  <script>
    const firstParagraph = document.querySelector("p");
    console.log(firstParagraph.innerHTML); // Paragraph 1
    console.log(firstParagraph.outerHTML); // <p>Paragraph 1</p>

    const innerSection = document.querySelector(".innerSection");
    console.log(innerSection.innerHTML);
    /* 
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
    <p>Paragraph 3</p>
    */

    console.log(innerSection.outerHTML);
    /* 
    <section class="innerSection">
      <p>Paragraph 1</p>
      <p>Paragraph 2</p>
      <p>Paragraph 3</p>
    </section>
    */
  </script>
</body>
```

<hr>

### Select the text of an element

`textContent` accesses the text inside an element: only text, minus all tags.

```html
<body>
  <h1 id="headingId">Heading</h1>

  <section class="outerSection">
    <section>
      <h2>Paragraph Heading</h2>
    </section>
    <section class="innerSection">
      <p>Paragraph 1</p>
      <p>Paragraph 2</p>
      <p>Paragraph 3</p>
    </section>
  </section>

  <script src="./index.js"></script>
  <script>
    const firstParagraph = document.querySelector("p");
    console.log(firstParagraph.textContent); // Paragraph 1

    const innerSection = document.querySelector(".innerSection");
    console.log(innerSection.textContent);
    /* 
    Paragraph 1
    Paragraph 2
    Paragraph 3
    */
  </script>
</body>
```

<hr>

### Retrieving the name of an HTML tag or node

`tagName` and `nodeName` gets the name of a tag and the name of a node, respectively.

```html
<body>
  <h1 id="headingId">Heading</h1>

  <section class="outerSection">
    <section>
      <h2>Paragraph Heading</h2>
    </section>
    <section class="innerSection">
      <p>Paragraph 1</p>
      <p>Paragraph 2</p>
      <p>Paragraph 3</p>
    </section>
  </section>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.childNodes[0]); // #text "\n\n  "
    console.log(document.body.childNodes[0].tagName); // undefined
    console.log(document.body.childNodes[0].nodeName); // #text

    const firstParagraph = document.querySelector("p");
    console.log(firstParagraph.tagName); // P
    console.log(firstParagraph.nodeName); // P

    const innerSection = document.querySelector(".innerSection");
    console.log(innerSection.tagName); // SECTION
    console.log(innerSection.nodeName); // SECTION
  </script>
</body>
```

<hr>

### Hiding an HTML element

We can hide an element using `<node>.hidden = true`. It is the same as `display: none;` in CSS. However, if we hide an element using CSS code - `display: none;` -, instead of hiding it with the JavaScript code, the `hidden` attribute will still show `false`.

```html
<body>
  <h1 id="headingId">Heading</h1>
  <h1 id="headingId2">Heading 2</h1>

  <script src="./index.js"></script>
  <script>
    const heading1 = document.querySelector("#headingId");
    heading1.hidden = true;

    const heading2 = document.querySelector("#headingId2");

    console.log(heading1.hidden); // true
    console.log(heading2.hidden); // false
  </script>
</body>
```

<hr>

### Input properties

The `<input>` tag has its own specific properties as well.

- `<inputElement>.type`
- `<inputElement>.id`
- `<inputElement>.value`
- `<inputElement>.checked`. This one is boolean.

```html
<body>
  <form action="">
    <label for="username">Username</label>
    <input type="text" id="username" />

    <br />
    <br />

    <p>Agree ?</p>
    <label for="yes">Yes</label>
    <input type="radio" id="yes" checked value="yes" />
    <label for="no">No</label>
    <input type="radio" id="no" value="no" />
  </form>

  <script src="./index.js"></script>
  <script>
    const inputUsername = document.querySelector("input#username");
    console.log(inputUsername); // <input id="username" type="text">
    console.log(inputUsername.type); // text
    console.log(inputUsername.id); // username
    console.log(inputUsername.value); // <empty string>

    const inputYes = document.querySelector("input#yes");
    const inputNo = document.querySelector("input#no");
    console.log(inputYes.checked); // true
    console.log(inputYes.value); // yes
    console.log(inputNo.checked); // false
    console.log(inputNo.value); // no
  </script>
</body>
```

<hr>

### Anchor element's `href` property

To get the link of an anchor tag, we can use `<anchorElement>.href`.

```html
<body>
  <a href="https://example.com" target="_blank">Example</a>
  <a href="https://test.com" target="_blank">Test</a>

  <script src="./index.js"></script>
  <script>
    const anchorTags = document.querySelectorAll("a");
    anchorTags.forEach((item) => {
      console.log(item.href);
      /* 
      https://example.com/
      https://test.com/
      */
    });
  </script>
</body>
```

<hr>

### Working with HTML tag attributes

There are several DOM properties that let us work with the attributes of tags.

- `<element>.hasAttribute(<attribute>)` checks for existence of the attribute.

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");

    console.log(imgElem.hasAttribute("src")); // true
    console.log(imgElem.hasAttribute("width")); // false
  </script>
</body>
```

- `<element>.getAttribute(<attribute>)` gets the value of the attribute.

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    console.log(imgElem.getAttribute("src")); // ./inexistent.img
  </script>
</body>
```

- `<element>.setAttribute(<attribute>, 'value')` sets the value of the attribute.

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    console.log(imgElem.getAttribute("alt")); // This image doesn't exist

    imgElem.setAttribute("alt", "Inexistent image");
    console.log(imgElem.getAttribute("alt")); // Inexistent image
  </script>
</body>
```

- `<element>.removeAttribute(<attribute>)` removes the attribute.

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    console.log(imgElem.hasAttribute("style")); // true

    imgElem.removeAttribute("style");
    console.log(imgElem.hasAttribute("style")); // false
  </script>
</body>
```

- `<element>.attributes` returns a `NamedNodeMap` object, which is a collection of attribute objects. `setAttribute` and `getAttribute` might be enough to access and manipulate the attributes of an element. However, `NamedNodeMap` object also provides various ways that could let us retrieve and manipulate the attributes of an element.

For example, we can use an array and object syntax to access the attribute objects within the `NamedNodeMap` returned by `<element>.attributes`.

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    const imgNamedNodeMap = imgElem.attributes;

    console.log(imgNamedNodeMap);
    // NamedNodeMap(3) [ src="./inexistent.img", alt="This image doesn't exist", style="border: 1px solid red;" ]

    console.log(imgNamedNodeMap[0]); // src="./inexistent.img"
    console.log(imgNamedNodeMap[0]["value"]); // ./inexistent.img

    console.log(imgNamedNodeMap["src"]); // src="./inexistent.img"
    console.log(imgNamedNodeMap["src"]["value"]); // ./inexistent.img

    console.log(imgNamedNodeMap.src); // src="./inexistent.img"
    console.log(imgNamedNodeMap.src.value); // ./inexistent.img
  </script>
</body>
```

The `NamedNodeMap` also has the `getNamedItem` method that helps to retrieve the attribute of an element:

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    const imgNamedNodeMap = imgElem.attributes;

    console.log(imgNamedNodeMap.getNamedItem("src")); // src="./inexistent.img"
  </script>
</body>
```

Another method, that we can use to retrieve the attribute of an element, from the `NamedNodeMap` is the `item` method:

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    const imgNamedNodeMap = imgElem.attributes;

    console.log(imgNamedNodeMap.item(0)); // src="./inexistent.img"
    console.log(imgNamedNodeMap.item("src")); // src="./inexistent.img"
  </script>
</body>
```

To set an attribute, we can use the `setNamedItem` metod from `NamedNodeMap`. This method accepts an attribute object, so if we want to use this method, we might need to use the `Document.createAttribute` method as well.

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    const imgNamedNodeMap = imgElem.attributes;

    const createdAltAttr = document.createAttribute("alt");
    createdAltAttr.value = "Inexistent image";

    console.log(imgNamedNodeMap.getNamedItem("alt")); // alt="This image doesn't exist"

    imgNamedNodeMap.setNamedItem(createdAltAttr);
    console.log(imgNamedNodeMap.getNamedItem("alt")); // "Inexistent image"
  </script>
</body>
```

We can also use the `value` property of the attribute object to set or change it's value:

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    const imgNamedNodeMap = imgElem.attributes;

    imgNamedNodeMap.getNamedItem("alt").value = "Inexistent image";
    console.log(imgNamedNodeMap.getNamedItem("alt")); // "Inexistent image"
  </script>
</body>
```

To remove an attribute, we can use the `removeNamedItem` from the `NamedNodeMap`.

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");
    const imgNamedNodeMap = imgElem.attributes;

    console.log(imgNamedNodeMap.getNamedItem("alt")); // alt="This image doesn't exist"

    imgNamedNodeMap.removeNamedItem("alt");
    console.log(imgNamedNodeMap.getNamedItem("alt")); // null
  </script>
</body>
```

<hr>

### The `style` object

`style` is both an attribute and an object. So, it can be accessed using both:

- `<element>.getAttribute('style')`
- `<element>.style`

```html
<body>
  <img
    src="./inexistent.img"
    alt="This image doesn't exist"
    style="border: 1px solid red;"
  />

  <script src="./index.js"></script>
  <script>
    const imgElem = document.querySelector("img");

    console.log(imgElem.getAttribute("style")); // border: 1px solid red;
    console.log(imgElem.style); // CSSStyleDeclaration...
  </script>
</body>
```

Here is how to add and remove a styling of an element using the `style` property:

```html
<body>
  <p style="text-align: center;">This is a text</p>

  <script src="./index.js"></script>
  <script>
    const paragraphElem = document.querySelector("p");
    paragraphElem.style.backgroundColor = "lightblue";
    paragraphElem.style.border = "1px solid red";

    paragraphElem.style.removeProperty("border");
  </script>
</body>
```

We can also style an element using `<element>.style.cssText`. This one removes all the existing styles of an element:

```html
<body>
  <p style="text-align: center;">This is a text</p>

  <script src="./index.js"></script>
  <script>
    const paragraphElem = document.querySelector("p");
    paragraphElem.style.cssText = `background-color: lightgreen;
      border: 1px solid red;`;
  </script>
</body>
```

### Retrieving the style information of an element

To retrieve the style of an element, we can use `getComputedStyle`. This global method is read-only, and we cannot set the style of an element using it:

```html
<body>
  <p style="text-align: center;">This is a text</p>

  <script src="./index.js"></script>
  <script>
    const paragraphElem = document.querySelector("p");

    console.log(getComputedStyle(paragraphElem)); // CSSStyleDeclaration
    console.log(getComputedStyle(paragraphElem).textAlign); // center
    console.log(getComputedStyle(paragraphElem).marginTop); // not margin, but marginTop/Left etc. should be used

    // This causes an error
    // getComputedStyle(paragraphElem).textAlign = "right"
  </script>
</body>
```

<hr>

### Working with Attributes starting with `data-`

`data-*` attributes allow us to store extra information on standard, semantic HTML elements without other hacks such as non-standard attributes, or extra properties on DOM. Attributes starting with “`data-*`” are available in the `dataset` property.

```html
<body>
  <p style="text-align: center;" data-about-something="something">
    This is a text
  </p>

  <script src="./index.js"></script>
  <script>
    const paragraphElem = document.querySelector("p");

    console.log(paragraphElem.dataset.aboutSomething); // something

    paragraphElem.dataset.firstParagraph = true;
    if (paragraphElem.dataset.firstParagraph)
      paragraphElem.textContent = "This is the first paragraph.";
  </script>
</body>
```

<hr>

### Creating an HTML element

To create an element, we use `document.createElement("<element>")`.

```html
<body>
  <script src="./index.js"></script>
  <script>
    // This element has been created but not yet added to the webpage
    const newParagraphElem = document.createElement("p");

    console.log(newParagraphElem); // <p>
  </script>
</body>
```

### Creating a text node

To create a text node, we use `document.createTextNode("<text>");`

```html
<body>
  <script src="./index.js"></script>
  <script>
    const newTextNode = document.createTextNode(
      "This is a text node, which is not yet added to the webpage"
    );
    console.log(newTextNode); // #text "This is a text node, which is not yet added to the webpage"
  </script>
</body>
```

<hr>

### Adding elements to the DOM

There are various methods to add elements and nodes to the DOM:

- `append()` appends nodes or strings at the end of a node.
- `prepend()` inserts nodes or strings at the beginning of a node.

```html
<body>
  <p style="text-align: center;" data-about-something="something">
    This is a text
  </p>

  <script src="./index.js"></script>
  <script>
    console.log(document.body.childNodes); // NodeList(6)...
    console.log(document.body.children); // HTMLCollection { ...length: 3 }

    const newTextNode = document.createTextNode(
      "This text node is added to the webpage with JS"
    );
    const newParagraphElem = document.createElement("p");
    newParagraphElem.textContent =
      "This element is added to the webpage with JS";

    document.body.append(newTextNode); // append at the end of node
    document.body.prepend(newParagraphElem); // prepend at the beginning of node

    console.log(document.body.childNodes); // NodeList(8)...
    console.log(document.body.children); // HTMLCollection { ...length: 4 }
  </script>
</body>
```

- `before()` inserts nodes or strings before a node.
- `after()` inserts nodes or strings after a node.

```html
<body>
  <p style="text-align: center;" data-about-something="something">
    This is a text
  </p>

  <script src="./index.js"></script>
  <script>
    const existingParagraphElem = document.querySelector("p");

    const newTextNode = document.createTextNode(
      "This text node is added to the webpage with JS"
    );
    const newParagraphElem = document.createElement("p");
    newParagraphElem.textContent =
      "This element is added to the webpage with JS";

    existingParagraphElem.before(newTextNode); // insert nodes or strings before a node
    existingParagraphElem.after(newParagraphElem); // insert nodes or strings after a node
  </script>
</body>
```

- `replaceWith()` replaces a node with the given nodes or strings.

```html
<body>
  <p style="text-align: center;" data-about-something="something">
    This is a text
  </p>

  <script src="./index.js"></script>
  <script>
    const existingParagraphElem = document.querySelector("p");

    const newParagraphElem = document.createElement("p");
    newParagraphElem.textContent =
      "This element is added to the webpage with JS";

    existingParagraphElem.replaceWith(newParagraphElem);
  </script>
</body>
```

<hr>

### Insert an HTML string with `<element>.insertAdjacentHTML(<where>, <html>)`

To insert an HTML string “as html”, with all tags and stuff working, we can use `<element>.insertAdjacentHTML(<where>, <html>)`

- `<element>.insertAdjacentHTML('beforebegin', '<HTMLCode>');` - insert html immediately before the `<element>`.

```html
<body>
  <div>
    <p style="text-align: center;">This is a text</p>
  </div>

  <script src="./index.js"></script>
  <script>
    const divElement = document.querySelector("div");
    divElement.insertAdjacentHTML(
      "beforebegin",
      "<p>added before the DIV element</p>"
    );

    console.log(document.body.children); // HTMLCollection { 0: p, 1: div, ...length: 4 }
  </script>
</body>
```

- `<element>.insertAdjacentHTML('afterbegin', '<HTMLCode>');` - insert html into the `<element>`, at the beginning.

```html
<body>
  <div>
    <p style="text-align: center;">This is a text</p>
  </div>

  <script src="./index.js"></script>
  <script>
    const divElement = document.querySelector("div");
    divElement.insertAdjacentHTML(
      "afterbegin",
      "<p>added into the beginning of the DIV element</p>"
    );

    console.log(document.body.children); // HTMLCollection { 0: div, ...length: 3 }
  </script>
</body>
```

- `<element>.insertAdjacentHTML('beforeend', '<HTMLCode>');` - insert html into the `<element>`, at the end.

```html
<body>
  <div>
    <p style="text-align: center;">This is a text</p>
  </div>

  <script src="./index.js"></script>
  <script>
    const divElement = document.querySelector("div");
    divElement.insertAdjacentHTML(
      "beforeend",
      "<p>added into the end of the DIV element</p>"
    );

    console.log(document.body.children); // HTMLCollection { 0: div, ...length: 3 }
  </script>
</body>
```

- `<element>.insertAdjacentHTML('afterend', '<HTMLCode>');` - insert html immediately after the `<element>`.

```html
<body>
  <div>
    <p style="text-align: center;">This is a text</p>
  </div>

  <script src="./index.js"></script>
  <script>
    const divElement = document.querySelector("div");
    divElement.insertAdjacentHTML(
      "afterend",
      "<p>added after the DIV element</p>"
    );

    console.log(document.body.children); // HTMLCollection { 0: div, 1: p, ...length: 4 }
  </script>
</body>
```

### Insert Text with `<element>.insertAdjacentText(<where>, <text>)`

`<element>.insertAdjacentText(<where>, <text>)` has the same syntax as above but inserts text.

<hr>

### Remove a node from the DOM

To remove the node from a DOM, we can use the `remove()` method:

```html
<body>
  <section>
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const firstParagraph = document.querySelector("p");

    firstParagraph.remove();
  </script>
</body>
```

<hr>

### Copy a node

We can copy a node using the `cloneNode()` method:

- `<element>.cloneNode(true);` - the node, its attributes, and its whole subtree, including text that may be in child text nodes, is also copied.
- `<element>.cloneNode(false);` - only the node with all attributes is copied. The subtree, including any text that the node contains, is not cloned.

```html
<body>
  <section>
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");

    const newElem = sectionElem.cloneNode(true);
    document.body.append(newElem);
  </script>
</body>
```

<hr>

### Dealing with HTML Classes

There are various properties and methods to work with HTML classes:

- `<element>.className;` - access the class of an HTML element. The assignment to className, using this method, replaces the whole string of classes.
- `<element>.classList.contains("<className>");` - checks for the given class, returns `true` or `false`.

```html
<body>
  <section>
    <p class="blueBackground centerAligned">Paragraph 1</p>
    <p class="blueBackground centerAligned">Paragraph 2</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const firstParagraph = document.querySelector("p");

    console.log(firstParagraph.className); // blueBackground centerAligned
    firstParagraph.className = "greenBackground";
    console.log(firstParagraph.className); // greenBackground

    console.log(firstParagraph.classList.contains("blueBackground")); // false
    console.log(firstParagraph.classList.contains("greenBackground")); // true
  </script>
</body>
```

- `<element>.classList.add("<className>");` - adds given classes to an HTML element.
- `<element>.classList.remove("<className>");` - removes given classes from an HTML element.

```html
<body>
  <section>
    <p class="blueBackground centerAligned">Paragraph 1</p>
    <p class="blueBackground centerAligned">Paragraph 2</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const firstParagraph = document.querySelector("p");

    firstParagraph.classList.remove("centerAligned", "blueBackground");

    setTimeout(() => {
      firstParagraph.classList.add("centerAligned", "greenBackground");
    }, 1000);
  </script>
</body>
```

- `<element>.classList.toggle("<className>", <Boolean>);` adds the given class, if not present, to an HTML element. Also, removes the given class, if present, from an HTML element.
  - If the `<Boolean>` is `true`, then the class will only be added, but not removed.
  - If the `<Boolean>` is `false`, then the class will only be removed, but not added.

```html
<body>
  <section>
    <p class="blueBackground centerAligned">Paragraph 1</p>
    <p class="blueBackground centerAligned">Paragraph 2</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const firstParagraph = document.querySelector("p");

    count = 0;
    const timerId = setInterval(() => {
      firstParagraph.classList.toggle("centerAligned");
      count++;
      if (count === 3) {
        clearInterval(timerId);
      }
    }, 1000);
  </script>
</body>
```

<hr>

### Accessing the positioned ancestor of HTML element

`<element>.offsetParent` is a read-only property that returns the nearest ancestor that the browser uses for calculating coordinates during rendering. The nearest ancestor that is one of the following:

- **CSS-positioned** (If there is no positioned ancestor element, the `<body>` is returned),
- `<body>`,
- `<table>`,
- `<th>`,
- `<td>`

In some occasions `offsetParent` is `null`:

- For not shown elements (`display:none` or not in the document).
- For `<body>` and `<html>`.
- For elements with `position:fixed`.

```html
<body>
  <section>
    <p>Paragraph 1</p>
    <p style="display: none;">Paragraph 2</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const firstParagraph = document.querySelector("p");

    console.log(firstParagraph.offsetParent); // <body>, because section is not positioned
    console.log(firstParagraph.nextElementSibling.offsetParent); // null, because `display: none;`

    sectionElem.style.position = "absolute";
    console.log(firstParagraph.offsetParent); // <section style="position: absolute;">
  </script>
</body>
```

### Retrieving the coordinates of an element relative to `<element>.offsetParent`

- `<element>.offsetLeft` read-only property returns the number of pixels that the upper left corner of the current element is offset within the `<element>.offsetParent`.
- `<element>.offsetTop` read-only property returns the distance from the outer border of the current element (including its margin) to the top padding edge of the `<element>.offsetParent`.

```html
<body>
  <section>
    <p>Paragraph 1</p>
    <p style="display: none;">Paragraph 2</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const firstParagraph = document.querySelector("p");

    sectionElem.style.position = "absolute";

    console.log(firstParagraph.offsetParent); // <section style="position: absolute;">
    console.log(firstParagraph.offsetLeft); // 0

    firstParagraph.style.marginLeft = "5px";
    firstParagraph.style.marginTop = "150px";
    console.log(firstParagraph.offsetLeft); // 5
    console.log(firstParagraph.offsetTop); // 150
  </script>
</body>
```

<hr>

### Retrieving the width and height of an element

To get the content width and height together with paddings, without the scrollbar, we can use `<element>.clientWidth`, and `<element>.clientHeight`, respectively.

To get the content width and height together with paddings including the scrolled out parts, and without the scrollbar, we can use `<element>.scrollWidth`, and `<element>.scrollHeight`, respectively.

```html
<body>
  <section>
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
    <p>Paragraph 3</p>
    <p>Paragraph 4</p>
    <p>Paragraph 5</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");

    sectionElem.style.overflowY = "scroll";

    sectionElem.style.width = "100px";
    sectionElem.style.paddingLeft = "10px";
    sectionElem.style.height = "40px";
    sectionElem.style.paddingTop = "10px";

    console.log(sectionElem.clientWidth); // 110, width + padding
    console.log(sectionElem.scrollWidth); // 110, width + padding
    console.log(sectionElem.clientHeight); // 50, height + padding
    console.log(sectionElem.scrollHeight); // 196, visible height + scrolled-out height + padding

    sectionElem.style.width = "200px";
    sectionElem.style.height = "50px";

    console.log(sectionElem.clientWidth); // 210, width + padding
    console.log(sectionElem.scrollWidth); // 210, width + padding
    console.log(sectionElem.clientHeight); // 50, height + padding
    console.log(sectionElem.scrollHeight); // 196, visible height + scrolled-out height +
  </script>
</body>
```

### Deal with scrolling on a screen

- `<element>.scrollLeft` property gets or sets the number of pixels by which an element's content is scrolled from its left edge.
- `<element>.scrollTop` property gets or sets the number of pixels by which an element's content is scrolled from its top edge.

```html
<body>
  <section>
    <p>Paragraph 1</p>
    <p>Paragraph 2</p>
    <p>Paragraph 3</p>
    <p>Paragraph 4</p>
    <p>Paragraph 5</p>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");

    sectionElem.style.overflowY = "scroll";

    sectionElem.style.height = "40px";
    sectionElem.style.paddingTop = "10px";

    sectionElem.scrollTop = "40";

    console.log(sectionElem.scrollTop); // 40
    console.log(sectionElem.scrollLeft); // 0
  </script>
</body>
```

- The read-only `window.scrollY` property returns the number of pixels by which the document is currently scrolled vertically.
- Likewise, the `window.scrollX` property returns the number of pixels by which the document is scrolled horizontally.

These properties are read-only. To scroll the window to a particular place, use `Window.scroll()`. It also accepts an object, which we can use to set the coordinate and the scrolling behavior.

`window.scrollTo()` is the same as the above method.

```html
<body>
  <section>
    <div style="height: 200px; border: 1px solid red;">1</div>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const divElem = document.querySelector("div");

    for (let divCount = 0; divCount < 10; divCount++) {
      divClone = divElem.cloneNode(true);
      divClone.textContent = Number(divClone.textContent) + divCount + 1;
      document.body.append(divClone);
    }

    console.log(window.scrollY); // 0
    console.log(window.scrollX); // 0

    window.scroll({
      top: 200,
      left: 100,
      behavior: "smooth",
    });

    /* window.scrollTo({
        top:200,
        left: 100,
        behavior: "smooth"
    }) */

    console.log(window.scrollY); // 200
    console.log(window.scrollX); // 0
  </script>
</body>
```

`window.scrollBy(x,y)` scrolls the page relative to its current position.

```html
<body>
  <section>
    <button style="position: fixed;">Scroll a bit</button>
    <div style="height: 200px; border: 1px solid red;">1</div>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const divElem = document.querySelector("div");
    const button = document.querySelector("button");

    for (let divCount = 0; divCount < 10; divCount++) {
      divClone = divElem.cloneNode(true);
      divClone.textContent = Number(divClone.textContent) + divCount + 1;
      document.body.append(divClone);
    }

    button.addEventListener("click", () => {
      window.scrollBy(0, 100);

      /* window.scrollBy({
        top: 100,
        left: 0,
        behavior: "smooth",
      }); */
    });
  </script>
</body>
```

`<element>.scrollIntoView()` method scrolls the element's ancestor containers such that the element on which `scrollIntoView()` is called is visible to the user. We can use this method with arguments:

- If `true`, the top of the element will be aligned to the top of the visible area of the scrollable ancestor.
- If `false`, the bottom of the element will be aligned to the bottom of the visible area of the scrollable ancestor.
- It also accepts an optional object to have a better control on the method.

```html
<body>
  <section>
    <button id="top" style="position: fixed;">Scroll to align the top</button>
    <button id="bottom" style="position: fixed; top: 40px;">
      Scroll to align the bottom
    </button>
    <div style="height: 200px; border: 1px solid red;">1</div>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const divElem = document.querySelector("div");
    const buttonToTop = document.querySelector("#top");
    const buttonToBottom = document.querySelector("#bottom");

    for (let divCount = 0; divCount < 10; divCount++) {
      divClone = divElem.cloneNode(true);
      divClone.textContent = Number(divClone.textContent) + divCount + 1;
      divClone.id = "div" + divClone.textContent;
      document.body.append(divClone);
    }

    div8 = document.querySelector("#div8");

    buttonToTop.addEventListener("click", () => {
      div8.scrollIntoView();
    });

    buttonToBottom.addEventListener("click", () => {
      div8.scrollIntoView(false);
    });
  </script>
</body>
```

### Retrieve the element size and coordinates with `getBoundingClientRect`

`<element>.getBoundingClientRect()` method returns a `DOMRect` object providing information about the size of an element and its position relative to the viewport. The `left`, `top`, `right`, `bottom`, `x`, `y`, `width`, and `height` properties describe the position and size of the overall rectangle in pixels. Properties other than width and height are relative to the top-left of the viewport. The `width` and `height` properties of the `DOMRect` object returned by the method include the padding and border-width, not only the content width/height.

```html
<body>
  <section>
    <div style="height: 200px; border: 1px solid red;">1</div>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const divElem = document.querySelector("div");

    console.log(divElem.getBoundingClientRect());
    // DOMRect { x: 8, y: 8, width: 700, height: 202, top: 8, right: 708, bottom: 210, left: 8 }
  </script>
</body>
```

### Retrieving the element coordinates with `elementFromPoint`

`document.elementFromPoint(x, y)` returns the most nested element at window coordinates (x, y).

```html
<body>
  <section>
    <div id="outer" style="height: 200px; border: 1px solid red;">
      Outer
      <div id="inner" style="border: 1px solid blue; height: 100px;">Inner</div>
    </div>
  </section>

  <script src="./index.js"></script>
  <script>
    const sectionElem = document.querySelector("section");
    const outerDiv = document.querySelector("#outer");
    const innerDiv = document.querySelector("#inner");

    innerDiv.onclick = getCoord;

    function getCoord(event) {
      elemHorizontal = this.getBoundingClientRect().x;
      elemVertical = this.getBoundingClientRect().y;
      console.log(document.elementFromPoint(elemHorizontal, elemVertical));
    }
  </script>
</body>
```

<hr>
<hr>

## DOM Events

### Pointer events

Pointer event is newer and should be used instead of mouse events.

| Pointer event        | Similar mouse event |
| -------------------- | ------------------- |
| `pointerdown`        | `mousedown`         |
| `pointerup`          | `mouseup`           |
| `pointermove`        | `mousemove`         |
| `pointerover`        | `mouseover`         |
| `pointerout`         | `mouseout`          |
| `pointerenter`       | `mouseenter`        |
| `pointerleave`       | `mouseleave`        |
| `pointercancel`      | -                   |
| `gotpointercapture`  | -                   |
| `lostpointercapture` | -                   |

```html
<body>
  <section style="border: 1px solid red; height: 100px;">
    <button>Click</button>
  </section>

  <script src="./index.js"></script>
  <script>
    const section = document.querySelector("section");
    const button = document.querySelector("button");

    button.addEventListener("pointerdown", () => {
      console.log("clicked the button");
    });

    button.addEventListener("pointerup", () => {
      console.log("ended clicking the button");
    });

    section.addEventListener("pointerover", () => {
      console.log(
        "hovering over the section. Happens each time when you bring the cursor over the section. Even if you hover over the element within the section and then over the section itself"
      );
    });

    section.addEventListener("pointermove", () => {
      console.log(
        "moving the cursor within the section, including the elements within the section"
      );
    });

    section.addEventListener("pointerout", () => {
      console.log("out from the section");
    });

    section.addEventListener("pointerenter", () => {
      console.log(
        "enter into the section. Happens each time when you get the cursor into the section. Unlike, 'pointerover' doesn't fire when you enter the section, then hover over the element within the section, and then hover over the section again"
      );
    });

    section.addEventListener("pointerleave", () => {
      console.log("left the section");
    });
  </script>
</body>
```

#### Pointer event properties

Pointer events have the same properties as mouse events plus others:

- `pointerId` – the unique identifier of the pointer causing the event.
- `pointerType` – the pointing device type. Must be a string, one of: “mouse”, “pen” or “touch”.
- `isPrimary` – is `true` for the primary pointer (the first finger in multi-touch).
- `width` – the width of the area where the pointer (e.g. a finger) touches the device. Where unsupported, e.g. for a mouse, it’s always 1.
- `height` – the height of the area where the pointer touches the device. Where unsupported, it’s always 1.
- `pressure` – the pressure of the pointer tip, in range from 0 to 1. For devices that don’t support pressure must be either 0.5 (pressed) or 0.
- `tangentialPressure` – the normalized tangential pressure.
- `tiltX`, `tiltY`, `twist` – pen-specific properties that describe how the pen is positioned relative the surface.

```html
<body>
  <section style="border: 1px solid red; height: 100px;">
    <button>Click</button>
  </section>

  <script src="./index.js"></script>
  <script>
    const section = document.querySelector("section");
    const button = document.querySelector("button");

    button.addEventListener("pointerdown", (event) => {
      console.log("clicked the button");
      console.log(event.pointerId);
      console.log(event.pointerType);
    });
  </script>
</body>
```

#### Capturing pointer id

`<element>.setPointerCapture(pointerId)` binds events with the given `pointerId` to `<element>`. In other words, `<element>.setPointerCapture(pointerId)` retargets all subsequent events with the given `pointerId` to `<element>`.

`<element>.releasePointerCapture(pointerId)` removes the binding.

<hr>

### Mouse events

Mouse events:

- `click`
- `dblclick`
- `contextmenu`
- `mousedown`
- `mouseup`
- `mouseover`
- `mousemove`
- `mouseout`
- `mouseenter`
- `mouseleave`

```html
<body>
  <section style="border: 1px solid red; height: 100px;">
    <button>Click</button>
  </section>

  <script src="./index.js"></script>
  <script>
    const section = document.querySelector("section");
    const button = document.querySelector("button");

    button.addEventListener("mousedown", () => {
      console.log("clicked the button");
    });

    button.addEventListener("mouseup", () => {
      console.log("ended clicking the button");
    });

    section.addEventListener("mouseover", () => {
      console.log(
        "hovering over the section. Happens each time when you bring the cursor over the section. Even if you hover over the element within the section and then over the section itself"
      );
    });

    section.addEventListener("mousemove", () => {
      console.log(
        "moving the cursor within the section, including the elements within the section"
      );
    });

    section.addEventListener("mouseout", () => {
      console.log("out from the section");
    });

    section.addEventListener("mouseenter", () => {
      console.log(
        "enter into the section. Happens each time when you get the cursor into the section. Unlike, 'mouseover' doesn't fire when you enter the section, then hover over the element within the section, and then hover over the section again"
      );
    });

    section.addEventListener("mouseleave", () => {
      console.log("left the section");
    });
  </script>
</body>
```

#### The properties of mouse events

There is a `button` property that indicates which button was clicked. This property only guarantees to indicate which buttons are pressed during events caused by pressing or releasing one or multiple buttons. Here is a table of its outputs:

| Button state              | `event.button` |
| ------------------------- | -------------- |
| Left button (primary)     | 0              |
| Middle button (auxiliary) | 1              |
| Right button (secondary)  | 2              |
| X1 button (back)          | 3              |
| X2 button (forward)       | 4              |

```html
<body>
  <section style="border: 1px solid red; height: 100px;">
    <button>Click</button>
  </section>

  <script src="./index.js"></script>
  <script>
    const section = document.querySelector("section");
    const button = document.querySelector("button");

    button.addEventListener("mouseup", (event) => {
      switch (event.button) {
        case 0:
          console.log("Left click");
          break;
        case 2:
          console.log("Right click");
          break;
      }
    });
  </script>
</body>
```

All mouse events include the information about pressed modifier keys. For example:

- `event.shiftKey` - Shift
- `event.altKey` - Alt (or Opt for Mac)
- `event.ctrlKey` - Ctrl
- `event.metaKey` - Cmd for Mac

```js
<body>

  <section style="border: 1px solid red; height: 100px; background-color: aliceblue;" height="200px"></section>

  <script src="./index.js"></script>
  <script>

    const section = document.querySelector("section")

    section.addEventListener("mousedown", (event) => {
      if (event.shiftKey) {
        console.log(`shift key was pressed`)
      } else if (event.altKey) {
        console.log(`alt key was pressed`)
      } else if (event.ctrlKey) {
        console.log(`ctrl key was pressed`)
      } else if (event.metaKey) {
        console.log(`meta key was pressed`)
      } else {
        console.log(`some other key was pressed`)
      }
    })

  </script>
</body>
```

For `mouseover` event, we have these properties:

- `event.target` - the element where the mouse came over.
- `event.relatedTarget` - the element from which the mouse came (`relatedTarget` → `target`).

For `mouseout`, event, we have these properties:

- `event.target` - the element that the mouse left.
- `event.relatedTarget` - the new under-the-pointer element, that mouse left for (`target` → `relatedTarget`).

```js
<body>

  <section style="border: 1px solid red; height: 100px; background-color: aliceblue;" height="200px"></section>

  <script src="./index.js"></script>
  <script>

    const section = document.querySelector("section")

    section.addEventListener("mouseover", (event) => {
      console.log("mouseover - event.target:", event.target)
      console.log("mouseover - event.relatedTarget:", event.relatedTarget)
    })

    section.addEventListener("mouseout", (event) => {
      console.log("mouseout - event.target:", event.target)
      console.log("mouseout - event.relatedTarget:", event.relatedTarget)
    })

  </script>
</body>
```

`mouseenter` and `mouseleave` properties have 2 important differences:

- Transitions inside the element, to/from descendants, are not counted.
- Events `mouseenter`/`mouseleave` do not bubble.

<hr>

### Keyboard events

Here are keyboard events and their event properties:

- `keydown`
- `keyup`

- `event.key` - allows to get the character.
- `event.code` - allows to get the “physical key code”.

```js
<body>

  <script src="./index.js"></script>
  <script>

    document.body.addEventListener("keydown", (event) => {
      console.log("keydown:", event.key)
      console.log("keydown:", event.code)
    })

    document.body.addEventListener("keyup", (event) => {
      console.log("keyup:", event.key)
      console.log("keyup:", event.code)
    })

  </script>
</body>
```

<hr>

### `<form>` element events

Here are `<form>` element events:

- `submit`
- `focus`
- `blur` – when the element loses the focus
- `focusin` and `focusout` events – exactly the same as `focus`/`blur`, but they bubble.

<br>

- Events `focus` and `blur` do not bubble, but propogate down during the capture phase.
- Methods `<element>.focus()` and `<element>.blur()` set/unset the focus on the element.
- `<form>.submit()` submits the form
- `focusin` and `focusout` events must be assigned using `addEventListener`.

```js
<body>

  <section>
    <form action="">
      <label for="name">Name</label>
      <input type="text" id="name">
    </form>

  </section>

  <script src="./index.js"></script>
  <script>

    const section = document.querySelector("section")
    const form = document.querySelector("form")

    console.log(form.elements[0])

    form.addEventListener("submit", (event) =>{
      event.preventDefault()
      console.log("form submitted")
    })

    form.elements[0].addEventListener("focus", (event) => {
      console.log("input is focused")
    })

    form.elements[0].addEventListener("focusin", (event) => {
      console.log("input is focused (this doesn't bubble)")
    })

    form.elements[0].addEventListener("blur", (event) => {
      console.log("input lost the focus")
    })

    form.elements[0].addEventListener("focusout", (event) => {
      console.log("input lost the focus (this doesn't bubble)")
    })

    const randomNum = Math.floor(Math.random() * 2)

    if (randomNum) {
      setTimeout(() => {
        form.submit()
        // if randomNum is 1, the form is submitted automatically and the page gets reloaded
        console.log(`the form was submitted automatically`)
      }, 500)
    }

    setTimeout(() => {
      console.log(`focused automatically`)
      form.elements[0].focus()
    }, 1000)

    setTimeout(() => {
      console.log(`lost the focus automatically`)
      form.elements[0].blur()
    }, 2000)

  </script>
</body>
```

<hr>

### `transitionend`

`transitionend` event is fired when a CSS transition has completed. If the `transitioncancel` event is fired, the `transitionend` event will not fire.

```html
<head>
  <style>
    section {
      background-color: aquamarine;
      height: 200px;
    }

    section:hover {
      background-color: bisque;
      transition: background-color 1s;
    }
  </style>
</head>
<body>
  <section></section>

  <script src="./index.js"></script>
  <script>
    const section = document.querySelector("section");

    section.addEventListener("transitionend", () => {
      console.log("transition ended");
    });
  </script>
</body>
```

<hr>

### Clipboard events

There are also some Clipboard events:

- `cut`
  - If the user attempts a cut action on uneditable content, the `cut` event still fires but the event object contains no data.
- `copy`
- `paste`

For the `paste` event the handler can get the access to data using the `<event>.clipboardData.getData('text/plain')` method.

A handler for `cut` and `copy` events can modify the clipboard contents by calling `setData(<format>, <data>)`. The handler cannot read the clipboard data. A handler for this event can modify the clipboard contents by calling `<event>.clipboardData.setData('text/plain')`.

```html
<body>
  <section>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aperiam,
      dignissimos enim itaque exercitationem, cum rem voluptatibus soluta, magni
      ratione delectus laborum ut provident fugit quos. Reprehenderit iste
      consequatur consequuntur fugiat.
    </p>
  </section>

  <script src="./index.js"></script>
  <script>
    const section = document.querySelector("section");

    section.addEventListener("copy", (event) => {
      // If you want to set data yourself, you need to call `event.preventDefault()`
      event.preventDefault();

      // We are manually adding "Any text" to the clipboard
      event.clipboardData.setData("text/plain", "Any text");
      console.log("copied");
    });

    section.addEventListener("cut", (event) => {
      // Nothing will be added to clipboard as we are cutting on uneditable content
      console.log("cut");
    });

    section.addEventListener("paste", (event) => {
      console.log("pasted:", event.clipboardData.getData("text/plain"));
    });
  </script>
</body>
```

<hr>

### Scroll events

- The `scroll` event fires when the document view has been scrolled.
- The `scrollend` event fires when scrolling has completed.

```html
<body>
  <section>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aperiam,
      dignissimos enim itaque exercitationem, cum rem voluptatibus soluta, magni
      ratione delectus laborum ut provident fugit quos. Reprehenderit iste
      consequatur consequuntur fugiat.
    </p>
  </section>
  <section id="section2" style="overflow: scroll; max-height: 100px;">
    <p>Section 2</p>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aperiam,
      dignissimos enim itaque exercitationem, cum rem voluptatibus soluta, magni
      ratione delectus laborum ut provident fugit quos. Reprehenderit iste
      consequatur consequuntur fugiat.
    </p>
  </section>

  <script src="./index.js"></script>
  <script>
    const section = document.querySelector("section");
    const section2 = document.querySelector("#section2");

    for (let paragraphs = 0; paragraphs <= 10; paragraphs++) {
      section.append(section.firstElementChild.cloneNode(true));
    }

    document.addEventListener("scroll", () => {
      console.log("document was scrolled");
    });

    document.addEventListener("scrollend", () => {
      console.log("document scroll ended");
    });

    section2.addEventListener("scrollend", () => {
      console.log("section scroll ended");
    });
  </script>
</body>
```

<hr>

### `input` and `change` events

Here are some more events:

- `input`
  - The `input` event fires when the value of an `<input>`, `<select>`, or `<textarea>` element has been changed as a direct result of a user action.
- `change`
  - The `change` event is fired for `<input>`, `<select>`, and `<textarea>` elements when the user modifies the element's value. Unlike the `input` event, the `change` event is not necessarily fired for each alteration to an element's value.

```html
<body>
  <section>
    <input type="text" />
  </section>

  <script src="./index.js"></script>
  <script>
    const input = document.querySelector("input");

    input.addEventListener("change", () => {
      console.log("changed to:", input.value);
    });

    input.addEventListener("input", () => {
      console.log("input:", input.value);
    });
  </script>
</body>
```

<hr>

### Ways to assign an event handler

There are several ways to assign an event handler:

- assign in HTML with an attribute `on<event>` (for example, `onclick`, `onkeydown`, etc.)

  ```js
  <body>

    <section>
      <input value="Click me" onclick="console.log('Click!')" type="button">
    </section>

    <script src="./index.js"></script>
  </body>
  ```

- assign using the DOM property `on<event>`

  ```js
  <body>

    <section>
      <input value="Click me" type="button">
    </section>

    <script src="./index.js"></script>
    <script>

      const input = document.querySelector("input")

      let clickCount = 0

      input.onclick = function(event) {
        if (clickCount >= 2) {
          input.onclick = null
        }

        console.log("click")
        clickCount++;
      }

    </script>
  </body>
  ```

- The best way to add a handler is `<element>.addEventListener(<event>, <handler>, [options])`. With this method, we can assign more than one handler to the same event and element.

  ```js
  <body>

    <section>
      <input value="Click me" type="button">
    </section>

    <script src="./index.js"></script>
    <script>

      const input = document.querySelector("input")

      function handler() {
        console.log("clicked");
      }

      input.addEventListener("click", handler);

      input.addEventListener("click", handler, { capture: true }); // if false the event bubbles
      input.addEventListener("click", handler, true); // same as the above

      // signals the browser that the handler is not going to call `event.preventDefault()`
      input.addEventListener("click", handler, { passive: true });

      // To remove a handler
      input.removeEventListener("click", handler);

    </script>
  </body>
  ```

- You can also assign an object or a class as an event handler. If an object or a class is assigned as a handler, when the event fires, their `handleEvent` method will be run.

  ```js
  <body>

    <section>
      <input value="Click me" type="button">
    </section>

    <script src="./index.js"></script>
    <script>
      const input = document.querySelector("input")

      const objForDOM = {
        handleEvent(event) {
          console.log(event.type + " event on ", event.currentTarget)
        }
      }

      input.addEventListener("click", objForDOM)

    </script>
  </body>
  ```

  ```js
  class ClassForDOM {
      handleEvent(event) {
        switch(event.type) {
          case 'mousedown':
            <element>.innerHTML = "Mouse button pressed";
            break;
          case 'mouseup':
            <element>.innerHTML += "...and released.";
            break;
        }
      }
  }

  const classForDOM = new ClassForDOM();
  <element>.addEventListener('mousedown', classForDOM);
  ```

<hr>

### `this` in the DOM event

In the DOM event, the value of `this` is the element that has the handler for the event.

```js
<body>

  <section style="height: 200px; background-color: aquamarine;">
    <button>Button</button>
  </section>

  <script src="./index.js"></script>
  <script>

    const section = document.querySelector("section")
    const button = document.querySelector("button")

    section.addEventListener("click", function (event) {
      console.log(this);
      // <section style="height: 200px; background-color: aquamarine;">
    })

    button.addEventListener("click", function (event) {
      console.log(this);
      // <button>
    })

  </script>
</body>
```

<hr>

### Properties of the event object

Event object has several useful properties:

- `event.currentTarget` - Element that has the handler. The same as `this`.
- `event.target` – the “target” element that initiated the event
- `event.type`
- `event.clientX`
- `event.clientY`
- `event.eventPhase` - tells the number of the phase on which the event was caught. This number represents the phase that the event is in:
  - none (`0`),
  - capture (`1`),
  - target (`2`),
  - bubbling (`3`).

`<event>.stopPropagation()` stops bubbling of an event. `event.stopImmediatePropagation()` stops bubbling and no other handler on the element runs.

```js
<body>

  <section style="height: 200px; background-color: aquamarine;">
    <button id="button1">Button</button>
    <button id="button2">Button</button>
  </section>

  <script src="./index.js"></script>
  <script>

    const section = document.querySelector("section")
    const button1 = document.querySelector("#button1")
    const button2 = document.querySelector("#button2")

    section.addEventListener("click", function (event) {
      console.log("section: currentTarget", event.currentTarget)
      console.log("section: target", event.target)
      console.log("section: type", event.type)
      console.log("section: clientX", event.clientX)
      console.log("section: clientY", event.clientY)
      console.log("section: eventPhase", event.eventPhase)
    })

    button1.addEventListener("click", function (event) {
      console.log("button: currentTarget", event.currentTarget)
      console.log("button: target", event.target)
      console.log("button: type", event.type)
      console.log("button: clientX", event.clientX)
      console.log("button: clientY", event.clientY)
      console.log("button: eventPhase", event.eventPhase)
    })

    button2.addEventListener("click", function (event) {
      event.stopPropagation()
      console.log("button: currentTarget", event.currentTarget)
      console.log("button: target", event.target)
      console.log("button: type", event.type)
      console.log("button: clientX", event.clientX)
      console.log("button: clientY", event.clientY)
      console.log("button: eventPhase", event.eventPhase)
    })

  </script>
</body>
```

<hr>

### Preventing the default event action

We can use 2 ways to tell the browser to stop its default action:

- `<event>.preventDefault()`
- and if `on<event>` attribute or `on<event>` property was used then `"return false;"` would work
- `<event>.defaultPrevented` is `true` if an action was prevented.

```html
<body>
  <section style="height: 200px; background-color: aquamarine;">
    <a
      href="https://developer.mozilla.org"
      onclick="console.log('prevented the default behaviour.');return false; "
    >
      Link 1
    </a>
    <a id="link2" href="https://developer.mozilla.org">Link 2</a>
    <a href="https://developer.mozilla.org">Link 3</a>
  </section>

  <script src="./index.js"></script>
  <script>
    link2.addEventListener("click", (event) => {
      event.preventDefault();
      console.log("prevented the default behaviour.", event.defaultPrevented);
    });
  </script>
</body>
```

<hr>

### Custom events

We can also generate our own custom events. Custom events can only be used with `<element>.addEventListener`. After an event object is created, we should “run” it on an element using `<element>.dispatchEvent(<Event>)`:

```html
<body>
  <section style="height: 200px; background-color: aquamarine;">
    <button>Click</button>
  </section>

  <script src="./index.js"></script>
  <script>
    const button = document.querySelector("button");

    // new Event(type[, options]);
    const someEvent = new Event("some event type", {
      bubbles: false,
      cancelable: false,
    });

    button.addEventListener("some event type", () => {
      console.log("custom event");
    });

    // Event runs after a second
    setTimeout(() => {
      button.dispatchEvent(someEvent);
    }, 1000);
  </script>
</body>
```

Instead of using `new Event`, we can use the `CustomEvent`. `CustomEvent` is better because it has an additional property `detail`, that we can use for a custom information.

```html
<body>
  <section style="height: 200px; background-color: aquamarine;">
    <button>Click</button>
  </section>

  <script src="./index.js"></script>
  <script>
    const button = document.querySelector("button");

    const someEvent = new CustomEvent("some event type", {
      bubbles: false,
      cancelable: false,
      detail: { name: "Some Name" },
    });

    button.addEventListener("some event type", (event) => {
      console.log("custom event");
      console.log(event.detail);
    });

    // Event runs after a second
    setTimeout(() => {
      button.dispatchEvent(someEvent);
    }, 1000);
  </script>
</body>
```

<hr>

Instead of using `new Event`, we should create specific type of events:

- `UIEvent`
- `FocusEvent`
- `MouseEvent`
- `WheelEvent`
- `KeyboardEvent`

Using specific events allows to specify some event-specific properties:

```js
const someMouseEvent = new MouseEvent("click", {
  bubbles: true,
  cancelable: true,
  clientX: 100,
  clientY: 100,
});
```

<hr>

### Events that come from real user actions

`event.isTrusted` is `true` for events that come from real user actions.

```html
<body>
  <section style="height: 200px; background-color: aquamarine;">
    <button id="button">Click</button>
  </section>

  <script src="./index.js"></script>
  <script>
    const button = document.querySelector("button");

    const newMouseEvent = new MouseEvent("click", {
      bubbles: true,
      cancelable: true,
      clientX: 100,
      clientY: 100,
    });

    setTimeout(() => {
      button.dispatchEvent(newMouseEvent);
    }, 1000);

    button.addEventListener("click", (event) => {
      // when a user clicks, `true` is logged
      console.log(event.isTrusted);
    });
  </script>
</body>
```

<hr>

### Document and resource loading

The lifecycle of an HTML page has three important events:

- `DOMContentLoaded` – the browser fully loaded HTML, and the DOM tree is built, but external resources like pictures `<img>` and stylesheets may not yet have loaded.
- `load` – not only HTML is loaded, but also all the external resources: images, styles etc.
- `beforeunload`/`unload` – the user is leaving the page

#### `DOMContentLoaded`

`DOMContentLoaded` is a document level event and works only with `addEventListener`.

If there is a script tag in an html document, the `DOMContentLoaded` would fire after that script tag runs.

```js
<script>
  document.addEventListener("DOMContentLoaded", () => {
    console.log("DOM is ready!");
  });
</script>

<script>
  console.log("This comes before DOMContentLoaded");
</script>
```

There are two exceptions to this rule:

- Scripts with the `async` attribute, don’t block `DOMContentLoaded`.
- Scripts that are generated dynamically with `document.createElement('script')` and then added to the webpage also don’t block this event.

One more thing to remember is that `DOMContentLoaded` doesn't wait for an external stylesheet to load. However, if the link to an external stylesheet comes before a script tag, then as `DOMContentLoaded` has to wait for the script tags to load, it would fire after an external stylesheet loads.

#### `load`

The `load` event on the `window` object triggers when the whole page is loaded including styles, images and other resources. This event is available via the `onload` property.

#### `unload`

When a visitor leaves the page, the `unload` event triggers on `window`.

#### `beforeunload`

If a visitor initiated navigation away from the page or tries to close the window, the `beforeunload` handler asks for additional confirmation.

The `event.preventDefault()` doesn’t work from a `beforeunload` handler.

#### `async`, `defer`

When the browser loads HTML and comes across a `<script>...</script>` tag or a `<script src="..."></script>` tag, it has to execute the scripts and only after that, load the rest of the page. This means that scripts can block the DOM from being loaded. This also means that if a script tag is placed in a wrong spot, it won't be able to detect certain elements on a page, because DOM gets to be loaded after those scripts are executed.

There are two `<script>` attributes that solve the problem.

The `defer` attribute tells the browser not to wait for the script. Instead, the browser will continue to process the HTML, build DOM. The script loads “in the background”, and then runs when the DOM is fully built.

In other words:

- Scripts with `defer` never block the page.
- Scripts with `defer` always execute when the DOM is ready (but before `DOMContentLoaded` event).

If there is more than one script that has the `defer` attribute, they will be loaded in their relative order, just like regular scripts.

The `defer` attribute is only for external scripts. Hence, if the `<script>` tag has no `src`, `defer` won't work.

The `async` attribute means that a script is completely independent. Other scripts don’t wait for `async` scripts, and `async` scripts don’t wait for them. `DOMContentLoaded` and `async` scripts don’t wait for each other. `async` scripts load in the background and run when ready.

Just like `defer`, the `async` attribute is ignored if the `<script>` tag has no `src`.

Dynamic scripts behave as `async` by default. This is how to add a script dynamically:

```js
const script = document.createElement("script");
script.src = "/someScript.js";
document.body.append(script);
```

If we use `script.async=false`, then scripts will be executed in the document order, just like `defer`.

#### Tracking the loading scripts and other external resources

We can track if the loading of some external resources were successful or not using two events:

- `onload` – successful load,
- `onerror` – an error occurred.

<hr>
<hr>

## Forms

### `document.forms`

`document.forms` is a named and ordered collection that lets us access the `<form>` element:

```html
<form name="formName">
  <input name="one" value="1" />
  <input name="two" value="2" />
</form>

<script src="./index.js"></script>
<script>
  // the form with name="formName"
  console.log(document.forms.formName);

  // the first form in the document
  console.log(document.forms[0]);
</script>
```

<hr>

### `form.elements`

There is `form.elements` which helps us access any form element:

```html
<form name="formName">
  <input name="one" value="1" />
  <input name="two" value="2" />
</form>

<script src="./index.js"></script>
<script>
  console.log(document.forms.formName.elements);
  console.log(document.forms.formName.elements["one"]);
</script>
```

<hr>

When there are multiple elements with the same name, then `<form>.elements["<nameOfTheFormElement>"]` is a collection as well. In that case, we can access elements like this: `<form>.elements.<nameOfTheFormElement>[0]`.

<hr>

### `<fieldset>`

`<fieldset>` elements inside a form have their own `.elements` collection as well.

```js
<form>.elements.<someFieldsetName>.elements.<someNameInTheFieldset>;
<form>.elements.<someFieldsetName>.elements[0];
```

<hr>

### `<element>.form`

If we access an element in the form, we can get the form through the element. For any element, the form is available as `<element>.form`.

Here are some ways to manipulate form elements:

```js
document.forms[0].elements.input.value = "New value";
document.forms[0].elements.textarea.value = "New text";
document.forms[0].elements.input.checked = true; // for a checkbox or radio button
```

<hr>

### `<select>` element

A `<select>` element has 3 important properties:

- `select.options` - the collection of `<option>` subelements,
- `select.value` - the value of the currently selected `<option>`,
- `select.selectedIndex` - the number of the currently selected `<option>`.

#### `<option>`

Option elements have their own properties:

- `option.selected` - Is the option selected.
- `option.index` - The number of the option among the others in its `<select>`.
- `option.text` - Text content of the option (seen by the visitor).

Here is how to manipulate the `<option>` element within the `<select>`:

```js
select.options[0].selected = true;
select.value = "some value for first option that to be selected";
```

```js
select.selectedIndex = 0;
select.value = "some value for first option that to be selected";
```

Here is a syntax to create a new `<option>`: `new Option(textInsideTheOption, optionValue, defaultSelected, selected)`

- `defaultSelected` – if `true`, then selected HTML-attribute is created,
- `selected` – if `true`, then the option is selected.

```js
const option1 = new Option("Text", "value");
const option2 = new Option("Text", "value", true, true);
```

<hr>

### submit a form to a server manually

To submit a form to the server manually, we can call `<form>.submit()`

<hr>
<hr>

## Window object

A global variable, `window`, represents the window in which the script is running. In a tabbed browser, each tab is represented by its own `Window` object. This object contains many properties and methods that we can use. We don't need to access all of them by prepending `window.`. For example, `document` is part of the `Window` object, and we can access it either using `window.document` or simply `document`.

For a full list of the window properties, go to [MDN Window](https://developer.mozilla.org/en-US/docs/Web/API/Window).

Let's review some properties and methods of this rich object.

### `window.caches`

`window.caches` is a read-only property that returns the `CacheStorage` object. This object enables functionality such as storing assets for offline use, and generating custom responses to requests.

Because older browsers may not support the functionality of `caches`, it is good practice to check for its availability before attempting to reference it. The `caches` property is available on the `window` object and we can check that it is implemented in the browser with this snippet:

```js
if ("caches" in window) {
  // your code
}
```

#### Create a new cache with `window.caches.open`

Use `window.caches.open(<name_of_cache>)` to obtain a `Cache` instance. The `Cache` interface provides methods for a persistent storage mechanism for `Request` / `Response` object pairs that are cached in long lived memory.

The `caches.open()` method first checks if a cache with the provided name already exists. If it doesn’t, it creates it and returns a `Promise` that resolves with the `Cache` object.

```js
const newCache = window.caches.open("new-cache").then((data) => {
  console.log(data);
}); // Cache {  }
```

The returned `Cache` itself has methods that we can use.

#### Add to cache with the `add()` method from a `Cache` instance

The `add()` method of the `Cache` interface takes a URL as an argument, makes a fetch request, and adds the resulting `Response` object to the given cache. If the response is already in the cache, the method does nothing.

The argument to the `add()` method can be a `Request` object or a URL string literal. `add()` will overwrite any key/value pair previously stored in the cache that matches the request.

```js
if ("caches" in window) {
  const cacheStuff = async () => {
    // this could also be a `new URL()` object
    const urlString = "./img1.jpg";

    await window.caches
      .open("img1")
      .then((cache) => {
        cache.add(urlString);
        console.log("Data was added to cache");
      })
      .catch((error) =>
        console.error("Error while adding data to cache:", error)
      );
  };

  cacheStuff();
}
```

We can gain more control by using a `Request` object:

```js
if ("caches" in window) {
  const cacheStuff = async () => {
    const urlString = "./img1.jpg";

    const options = {
      method: "GET",
      headers: new Headers({
        "Content-Type": "image/jpeg",
      }),
    };

    const req = new Request(urlString, options);

    await window.caches
      .open("img2")
      .then((cache) => {
        cache.add(req);
        console.log("Data was added to cache");
      })
      .catch((error) =>
        console.error("Error while adding data to cache:", error)
      );
  };

  cacheStuff();
}
```

#### Add to cache with the `addAll()` method from a `Cache` instance

The `addAll()` method of the `Cache` interface takes in an array of URL string literals or `Request` objects and returns a promise when all the resources have been cached. If any responses are already in the cache, the method skips them:

```js
const cacheStuff = async () => {
  const newCache = await window.caches.open("new-cache");

  const urls = ["./file.json", "./file2.json"];

  newCache
    .addAll(urls)
    .then(() => console.log("Data added to cache."))
    .catch((error) => console.error("Error adding data to cache:", error));
};

cacheStuff();
```

#### Change and override cache with the `put()` method from a `Cache` instance

The `put()` method takes two parameters:

- a URL string literal or a `Request` object,
- a `Response` either from the network or generated within your code.

The `put()` method of the `Cache` interface makes a request and adds the response from that request to the cache. If the response is already in the cache, the method overwrites it.

```js
const cacheStuff = async () => {
  const newCache = await window.caches.open("new-cache");

  newCache
    .put(
      "./file.json",
      new Response(
        '{"changedKey1": "changedValue1", "changedKey2": "changedValue2"}'
      )
    )
    .then(() => console.log("Data added to cache."))
    .catch((error) => console.error("Error adding data to cache:", error));
};

cacheStuff();
```

```js
const cacheStuff = async () => {
  const newCache = await window.caches.open("new-cache");

  newCache
    .put("./file2.json")
    .then(() => console.log("Data added to cache."))
    .catch((error) => console.error("Error adding data to cache:", error));
};

cacheStuff();
```

`Cache.add`/`Cache.addAll` do not cache responses with `Response.status` values that are not in the 200 range, whereas `Cache.put` lets you store any request/response pair.

#### Retrieve an item in cache using `match()` method from `Cache` and `CacheStorage`

The `match()` method finds the first matching request in the `Cache` object. It returns a `Promise` that resolves to the `Response` associated with the matching request. If no match is found, the `Promise` resolves to `undefined`.

The method could be accessed either through `CacheStorage` (`window.caches.match()`) or `Cache` instance.

```js
const cacheStuff = async () => {
  const newCache = await window.caches.open("new-cache");

  const matchedCache = await newCache.match("./file2.json");

  console.log(matchedCache);
};

cacheStuff();
```

The browser uses different factors in determining if two or more Requests match. A `Request` may have the same URL as another but use a different HTTP method. Two such requests are considered to be different by the browser. When using the `match` method, we can also pass an options object as the second parameter. This object has key-value pairs that tell `match` to ignore specific factors when matching a request:

```js
const cacheStuff = async () => {
  const newCache = await window.caches.open("new-cache");

  const options = {
    ignoreVary: true, // ignore differences in Headers
    ignoreMethod: true, // ignore differences in HTTP methods
    ignoreSearch: true, // ignore differences in query strings
  };

  const matchedCache = await newCache.match("./file2.json", options);

  console.log(matchedCache);
};

cacheStuff();
```

In a case where more than one cache item matches, the oldest one is returned.

#### Retrieve all items in cache using `matchAll()` method from `Cache` and `CacheStorage`

`matchAll()` method works the same as `match()` but retrieves all the matching items from cache. If no resources are found in the cache, the `matchAll()` method returns an empty array.

The method could be accessed either through `CacheStorage` (`window.caches.matchAll()`) or `Cache` instance.

#### Iterate through cache items using `keys()` method from `Cache` and `CacheStorage`

The `keys()` method returns a `Promise` that resolves to an array of `Request` objects representing the keys of the `Cache`. The requests are returned in the same order that they were inserted.

The method could be accessed either through `CacheStorage` (`window.caches.keys()`) or `Cache` instance.

```js
const cacheStuff = async () => {
  const newCache = await window.caches.open("new-cache");

  const cacheKeys = await newCache.keys();

  console.log(cacheKeys);
};

cacheStuff();
```

The `keys()` method also accepts an optional options object with properties such as `ignoreSearch`, `ignoreMethod`, and `ignoreVary`.

#### Delete an item from cache using `delete()` method from `Cache`

The `delete()` method finds the `Cache` entry whose key is the request, and if found, deletes the `Cache` entry and returns a `Promise` that resolves to `true`. If no `Cache` entry is found, it resolves to `false`. It accepts a URL string or a `Request` object as an argument.

```js
// delete a cache entry
const cacheStuff = async () => {
  const newCache = await window.caches.open("new-cache");

  newCache.delete("./file2.json");

  console.log(newCache);
};

cacheStuff();
```

The `delete()` method also accepts an optional options object with properties such as `ignoreSearch`, `ignoreMethod`, and `ignoreVary`.

#### Remove a cache with `window.caches.delete()`

We can also delete a cache by calling the `delete()` method on the `caches` property of the `window` object. This is different from the `delete()` method of the `Cache` instance. When a cache is deleted using `window.caches.delete()`, the method returns a `Promise` if the cache was actually deleted and a `false` if something went wrong or the cache doesn’t exist.

```js
// delete an existing cache
window.caches.delete("new-cache");
```

#### Find a cache with `window.caches.has()`

The `has(<cache_name>)` method of the `CacheStorage` interface returns a `Promise` that resolves to `true` if a `Cache` object matches the `<cache_name>`. It accepts a string representing the name of the `Cache` object you are looking for in the `CacheStorage`.

```js
window.caches.open("new-cache");

window.caches.has("new-cache").then((data) => console.log(data)); //true
```

<hr>

### `window.clientInformation` or `window.navigator`

`window.clientInformation` is an alias for `window.navigator`. The `Window.navigator` read-only property returns a reference to the `Navigator` object, which has methods and properties about the application running the script. The `Navigator` object represents the state and the identity of the user agent (browser). It has a lot of methods and properties. You can refer here for a thorough list: [MDN Navigator](https://developer.mozilla.org/en-US/docs/Web/API/Navigator)

#### `navigator.clipboard`

`navigator.clipboard` returns a `Clipboard` object that provides read and write access to the system clipboard. This is the entry point to the Clipboard API, which can be used to implement cut, copy, and paste features within a web application. To avoid potential issues, the Clipboard API can only be used on pages served over HTTPS (localhost is also permitted).

Because there are security risks of allowing a website to access user's clipboard, there are various errors that might happen while a developer is trying to work with the clipboard.

First of all, you can use the following code to check if the clipboard API is supported:

```js
if ("clipboard" in navigator) {
  console.log("Clipboard API is supported!");
} else {
  console.log("Clipboard API is not supported!");
}
```

`navigator.clipboard.writeText()`

To copy text to the clipboard call `writeText()`. The `writeText()` function returns a `Promise` that resolves or rejects depending on whether the passed text is copied successfully.

```js
navigator.clipboard
  .writeText("to be copied")
  .then(() => {
    console.log("Text copied to clipboard");
  })
  .catch((err) => {
    console.error("Failed to copy text: ", err);
  });
```

If you have error that says "Document is not focused", this might be because there is delay in writing to clipboard and user is not focusing on the window.

Another error that might occur is "Failed to copy text: DOMException: Clipboard write was blocked due to lack of user activation." To resolve this issue, you might need to call the `navigator.clipboard.writeText()` method within an event handler that is triggered by a user action.

So, you might try this:

```html
<button id="copyButton">Copy Text</button>

<script>
  const copyButton = document.getElementById("copyButton");

  copyButton.addEventListener("click", () => {
    navigator.clipboard
      .writeText("to be copied")
      .then(() => {
        console.log("Text copied to clipboard");
      })
      .catch((err) => {
        console.error("Failed to copy text: ", err);
      });
  });
</script>
```

`navigator.clipboard.readText()`

To read text from the clipboard, call `navigator.clipboard.readText()` and wait for the returned promise to resolve.

```html
<button id="readButton">Read the Copy</button>

<script>
  const readButton = document.getElementById("readButton");

  readButton.addEventListener("click", () => {
    navigator.clipboard
      .readText()
      .then((data) => {
        console.log(`Text from the clipboard is "${data}"`);
      })
      .catch((err) => {
        console.error(`Failed to read the text from clipboard: "${err}`);
      });
  });
</script>
```

<hr>

### `window.history`

The `window.history` read-only property returns a reference to the `History` object, which provides an interface for manipulating the browser session history (pages visited in the tab or frame that the current page is loaded in).

#### Moving back and forward in the browsing history

Moving backward and forward through the user's history is done using the `back()`, `forward()`, and `go()` methods.

```js
history.back(); // as if the user clicked on the Back button in their browser toolbar.
history.forward(); // as if the user clicked on the Forward button in their browser toolbar.
```

You can use the `go()` method to load a specific page from session history, identified by its relative position to the current page.

To move back one page:

```js
history.go(-1);
```

To move forward one page:

```js
history.go(1);
```

Another use for the `go()` method is to refresh the current page by either passing 0, or by invoking it without an argument:

```js
history.go(0);
history.go();
```

#### Number of pages in the browsing history

You can determine the number of pages in the history stack by looking at the value of the `history.length` property.

#### `history.pushState()` and `history.replaceState()`

`history.pushState(<state>, <title>, <URI/URL>)` will change the URL of the page and add the changed URL to the top of the URL stack of the history object.

- The `<state>` is any javascript data which will be stored in `history.state` variable, which will be available once you navigate through the page.

- The `<title>` on the code is just a text, which has no effect on any browser. You can skip that by passing an empty string `""` or some title text is fine.

- The `<URI/URL>` is a string which is the new URL to change.

If we are on "localhost:3000", and run the below code our directory will become "localhost:3000/newurl" (after 1 second) and the previous page in our history will be "localhost:3000".

```js
setTimeout(() => {
  history.pushState("temporary state data", "some title", "newurl"); // You can also provide a complete URL on the same domain

  console.log(history.state); // "temporary state data"
}, 1000);
```

Whenever users come back to the page which is added to history through `pushState` then an event with the name `popstate` will be triggered.

```js
window.addEventListener("popstate", (e) => {
  console.log("popstate");
});

setTimeout(() => {
  history.pushState("temporary state data", "some title", "newurl");

  console.log(history.state);
}, 1000);
// Whenever a user presses back `popstate` event will trigger
```

`history.replaceState()` only changes the URL . It doesn’t add URL to the history of URL the stack.

```js
setTimeout(() => {
  history.replaceState("temporary state data", "some title", "newurl");

  console.log(history.state);
}, 1000);
```

<hr>

### `window.innerHeight` and `window.innerWidth`

The read-only `innerHeight` property returns the interior height of the window in pixels, including the height of the horizontal scroll bar, if present.

The read-only `innerWidth` property returns the interior width of the window in pixels, including the width of the vertical scroll bar, if present.

```js
console.log(window.innerHeight);
console.log(window.innerWidth);
```

<hr>

### `window.location`

The `window.location` read-only property returns a `Location` object with information about the current location (URL) of the document.

#### Location properties to retrieve URL parts

Here are some properties in the `Location` object:

- `location.href`
- `location.hash`
- `location.search`
- `location.pathname`
- `location.origin`
- `location.port`
- `location.host`
- `location.hostname`
- `location.protocol`
- `location.origin` (Read only)

Let's explain all of the above properties on an example. Let's apply all of the above properties onto "https://example.org:8080/foo/bar?q=baz#bang"

- `location.href` - https://example.org:8080/foo/bar?q=baz#bang
- `location.hash` - #bang
- `location.search` - q=baz
- `location.pathname` - /foo/bar
- `location.origin` - https://example.org:8080
- `location.port` - 8080
- `location.host` - example.org:8080
- `location.hostname` - example.org
- `location.protocol` - https

`location.toString()` returns a string containing the whole URL. It is a read-only version of `location.href`.

If we want to go to a specific URL, we can manually set the `location.href` to a URL:

```js
setTimeout(() => {
  location.href = "http://localhost:5500/#hello";
  console.log(`redirected to ${location.origin}${location.pathname}#hello`);
}, 1000);
```

#### `location.assign()`

`location.assign(<url>)` loads the resource at the URL provided in the parameter. The URL can be absolute or relative. If the URL is not of the same origin as the script, it will cause an error.

```js
setTimeout(() => {
  location.assign("#hello");
  console.log(`redirected to ${location.origin}${location.pathname}#hello`);
}, 1000);
```

#### `location.replace()`

`location.replace(<url>)` replaces the current resource with the one at the provided URL (redirects to the provided URL).

The difference from the `assign()` method and setting the `href` property is that after using `replace()` the current page will not be saved in session `History`, meaning the user won't be able to use the back button to navigate to it.

```js
setTimeout(() => {
  location.replace("#hello");
  console.log(`redirected to ${location.origin}${location.pathname}#hello`);
}, 1000);
```

#### `location.reload()`

`location.reload()` reloads the current URL, like the Refresh button.

<hr>

### `window.open()` and `close`

The `Window` interface's `open(<URL> [, <target>, <windowFeatures>])` method

- takes a `<URL>` as a parameter, and loads the resource it identifies into a new or existing tab or window.
- The `<target>` parameter determines which window or tab to load the resource into, and
- the `<windowFeatures>` parameter can be used to control to open a new popup with minimal UI features and control its size and position.

For example:

```js
window.open("https://www.mozilla.org/", "mozillaTab");
```

The following example demonstrates how to open a popup, using the `popup` feature.

```js
window.open("https://www.mozilla.org/", "mozillaWindow", "popup");
```

`close()` closes the current window. This method can only be called on windows that were opened by a script using the `window.open()` method, or on top-level windows that have a single history entry.

```js
// Global variable to store a reference to the opened window
let openedWindow;

function openWindow() {
  openedWindow = window.open("https://www.mozilla.org/");
}

function closeOpenedWindow() {
  openedWindow.close();
}
```

The `window.closed` read-only property indicates whether the referenced window is closed or not. Returns `true` if the window has been closed or `false` if the window is open.

<hr>

### `window.confirm()`

`window.confirm()` instructs the browser to display a dialog with an optional message, and to wait until the user either confirms or cancels the dialog. It returns a boolean indicating whether OK (`true`) or Cancel (`false`) was selected.

```js
if (window.confirm("Do you really want to leave?")) {
  console.log("Thanks for Visiting!");
}
```

<hr>

### `window.getSelection()`

#### Range

JavaScript can access an existing selection, select/deselect DOM nodes as a whole or partially, remove the selected content from the document, wrap it into a tag, and so on. The basic concept of selection is `Range`, that is essentially a pair of “boundary points”: range start and range end.

A `Range` object is created without parameters

```js
const range = new Range();
```

After creating the `Range` objectm we can set the selection boundaries using `range.setStart(<node>, <offset>)` and `range.setEnd(<node>, <offset>)`.

- The first argument `<node>` in both methods can be either a text node or an element node, and the meaning of the second argument depends on what type of node is the first argument.

If `<node>` is a text node, then `<offset>` must be the position in its text.

```html
<p id="paragraph">Hello</p>

<script>
  let range = new Range();
  range.setStart(paragraph.firstChild, 2); // `firstChild` of `paragraph` is "Hello" - a text node
  range.setEnd(paragraph.firstChild, 4);

  // toString of a range returns its content as text
  console.log(range.toString()); // ll
</script>
```

If `<node>` is an element node, then `<offset>` must be the child number.

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 0); // 0th node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  // toString of a range returns its content as text, without tags
  console.log(range.toString()); // 0th text node, 1st text node,

  // select the range, as if we used a mouse and selected the range specified above
  document.getSelection().addRange(range);

  // You can see the childNodes of the paragraph
  console.log(paragraph.childNodes);
</script>
```

For text nodes, `<offset>` skips that many of characters, while for element nodes, that many child nodes.

We don’t have to use the same node in `setStart` and `setEnd`. A range may span across many unrelated nodes. It’s only important that the end is after the start in the document.

The range object that we created in the example above has following properties:

- `startContainer`, `startOffset` – node and offset of the start,
- `endContainer`, `endOffset` – node and offset of the end,
- `collapsed` – boolean, `true` if the range starts and ends on the same point (so there’s no content inside the range),
- `commonAncestorContainer` – the nearest common ancestor of all nodes within the range.

In addition to `setStart` and `setEnd`, there are other similar methods:

- `setStart(<node>, <offset>)` set start at: position offset in `<node>`
- `setStartBefore(<node>)` set start at: right before `<node>`
- `setEndBefore(<node>)` set end at: right before `<node>`
- `setEndAfter(<node>)` set end at: right after `<node>`

There are more methods to create ranges:

- `selectNode(<node>)` set range to select the whole node
- `selectNodeContents(<node>)` set range to select the whole node contents
- `collapse(toStart)`
- `cloneRange()` creates a new range with the same start/end

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  window.getSelection().addRange(range);

  setTimeout(() => {
    range.selectNode(paragraph);
  }, 1000);
</script>
```

The above methods are for creating ranges. There are also methods that are useful for editing ranges:

- `deleteContents()` – remove range content from the document
- `extractContents()` – remove range content from the document and return as `DocumentFragment`
- `cloneContents()` – clone range content and return as `DocumentFragment`
- `insertNode(node)` – insert node into the document at the beginning of the range
- `surroundContents(node)` – wrap node around range content. For this to work, the range must contain both opening and closing tags for all elements inside it: no partial ranges like `<i>abc`.

#### Selection

We may create `Range` objects but they do not visually select anything on their own. To select a range we use the `Selection` object, that can be obtained as `window.getSelection()` or `document.getSelection()`.

A selection may in theory contain multiple ranges (browser support isn't good at the moment). We can get these range objects using the method `getRangeAt(<i>)` – get i-th range, starting from 0.

Similar to a range, a selection object has a start, called “anchor”, and the end, called “focus”. Range objects always have their start before the end. But a selection object might have its anchor (start) after its focus (end).

The main selection properties are:

- `anchorNode` – the node where the selection starts,
- `anchorOffset` – the offset in `anchorNode` where the selection starts,
- `focusNode` – the node where the selection ends,
- `focusOffset` – the offset in `focusNode` where the selection ends,
- `isCollapsed` – true if selection selects nothing (empty range), or doesn’t exist.
- `rangeCount` – count of ranges in the selection, maximum 1 in all browsers except Firefox.

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  window.getSelection().addRange(range);

  console.log(window.getSelection().anchorNode); // p#paragraph
  console.log(window.getSelection().anchorOffset); // 1
  console.log(window.getSelection().focusNode); // p#paragraph
  console.log(window.getSelection().focusOffset); // 2
  console.log(window.getSelection().isCollapsed); // false
  console.log(window.getSelection().rangeCount); // 1
</script>
```

There are events on to keep track of selection:

- `<element>.onselectstart` – event fires when a selection starts specifically on `<element>` (or inside it). For instance, when the user presses the mouse button on it and starts to move the pointer.
  - Preventing the default action cancels the selection start. So starting a selection from this element becomes impossible, but the element is still selectable. The visitor just needs to start the selection from elsewhere.
- `document.onselectionchange` – whenever a selection changes or starts. Please note: this handler can be set only on document, it tracks all selections in it.

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  // will fire when a user clicks on a window
  window.addEventListener("selectstart", () => {
    console.log("selection started");
  });
</script>
```

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  // Fires even when the selection starts
  document.addEventListener("selectionchange", () => {
    console.log("selection has changed");
  });
</script>
```

There are two approaches to copying the selected content:

- We can use `document.getSelection().toString()` to get it as text.
- Otherwise, to copy the full DOM, e.g. if we need to keep formatting, we can get the underlying ranges with `getRangeAt(...)`. A `Range` object, in turn, has `cloneContents()` method that clones its content and returns as `DocumentFragment` object, that we can insert elsewhere.

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  document.getSelection().addRange(range);

  console.log(document.getSelection().toString()); // 1st node,
</script>
```

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  document.getSelection().addRange(range);

  console.log(document.getSelection().getRangeAt(0).toString()); // 1st node,
  console.log(document.getSelection().getRangeAt(0).startContainer); // p#paragraph
  console.log(document.getSelection().getRangeAt(0).endContainer); // p#paragraph

  const fragment = document.getSelection().getRangeAt(0).cloneContents();

  document.body.appendChild(fragment); // appends <i>1st node,</i>
</script>
```

In addition to `getRangeAt`, there are other useful methods:

- `addRange(<range>)` – add range to selection. All browsers except Firefox ignore the call, if the selection already has an associated range.
- `removeRange(<range>)` – remove range from the selection.
- `removeAllRanges()`– remove all ranges.
- `empty()`– alias to `removeAllRanges`.

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  document.getSelection().addRange(range);

  setTimeout(() => {
    document.getSelection().removeRange(range);
  }, 1000);
</script>
```

```html
<p id="paragraph">0th node, <i>1st node,</i> 2nd node, <b>3rd node</b></p>

<script>
  let range = new Range();

  range.setStart(paragraph, 1); // 1st node
  range.setEnd(paragraph, 2); // up to and exclusive of 2nd node

  document.getSelection().addRange(range);

  setTimeout(() => {
    document.getSelection().removeAllRanges();

    // below does the same as above
    // document.getSelection().empty();
  }, 1000);
</script>
```

If we don't want to access the underlying `Range` object, there are convenience methods to manipulate the selection range directly, without intermediate `Range` calls:

- `collapse(node, offset)` – replace selected range with a new one that starts and ends at the given node, at position offset.
- `setPosition(node, offset)` – alias to `collapse`.
- `collapseToStart()` – collapse (replace with an empty range) to selection start,
- `collapseToEnd()` – collapse to selection end,
- `extend(node, offset)` – move focus of the selection to the given node, position offset,
- `setBaseAndExtent(anchorNode, anchorOffset, focusNode, focusOffset)` – replace selection range with the given start `anchorNode`/`anchorOffset` and end `focusNode`/`focusOffset`. All content in-between them is selected.
- `selectAllChildren(node)` – select all children of the node.
- `deleteFromDocument()` – remove selected content from the document.
- `containsNode(node, allowPartialContainment = false)` – checks whether the selection contains node (partially if the second argument is true)

If a document selection already exists, empty it first with `removeAllRanges()`. And then add ranges. Otherwise, all browsers except Firefox ignore new ranges. The exception is some selection methods, that replace the existing selection, such as `setBaseAndExtent`.

#### Selection in forms

Form elements, such as input and textarea provide special API for selection, without `Selection` or `Range` objects.

- `input.selectionStart` – position of selection start (writeable),
- `input.selectionEnd` – position of selection end (writeable),
- `input.selectionDirection` – selection direction, one of: “forward”, “backward” or “none” (if e.g. selected with a double mouse click),

`input.onselect` – triggers when something is selected. `onselect` triggers when something is selected, but not when the selection is removed.

`document.onselectionchange` event should not trigger for selections inside a form control, according to the spec, as it’s not related to document selection and ranges. Some browsers generate it, but we shouldn’t rely on it.

```html
<input type="text" id="myInput" value="Hello, World!" />

<script>
  myInput.addEventListener("select", () => {
    console.log(myInput.selectionStart, myInput.selectionEnd);
    console.log(myInput.selectionDirection);
  });
</script>
```

- `input.select()` – selects everything in the text control (can be textarea instead of input),
- `input.setSelectionRange(start, end, [direction])` – change the selection to span from position start till end, in the given direction (optional).
- `input.setRangeText(replacement, [start], [end], [selectionMode])` – replace a range of text with the new text. Optional arguments start and end, if provided, set the range start and end, otherwise user selection is used. The last argument, `<selectionMode>`, determines how the selection will be set after the text has been replaced. The possible values are:
- `"select"` – the newly inserted text will be selected.
- `"start"` – the selection range collapses just before the inserted text (the cursor will be immediately before it).
- `"end"` – the selection range collapses just after the inserted text (the cursor will be right after it).
- `"preserve"` – attempts to preserve the selection. This is the default.

<hr>
<hr>

## Fetch

### GET request

Here is an example of a GET request with Fetch:

```js
const url = "https://jsonplaceholder.typicode.com/users";

// GET request with Fetch
fetch(url)
  .then((response) => response.json())
  .then((data) => console.log(data))
  .catch((error) => console.error(error));
```

```js
// the same as above
fetch(url, {
  method: "GET", // GET method cannot have the "body" property
})
  .then((response) => response.json())
  .then((data) => console.log(data))
  .catch((error) => console.error(error));
```

We can choose only one body-reading method.

- `response.text()` – read the response and return as text,
- `response.json()` – parse the response as JSON,
- `response.formData()` – return the response as `FormData` object,
- `response.blob()` – return the response as `Blob` (binary data with type),
- `response.arrayBuffer()` – return the response as `ArrayBuffer` (low-level representation of binary data),
- Additionally, `response.body` is a ReadableStream object, it allows you to read the body chunk-by-chunk

Here is an example of using `response.text`:

```js
const url = "https://jsonplaceholder.typicode.com/users";

fetch(url)
  .then((response) => response.text())
  .then((data) => console.log(data))
  .catch((error) => console.error(error));
```

<hr>

### POST request

Here is an example of a POST request with Fetch:

```js
const postUrl = "https://httpbin.org/post";

const data = {
  name: "Some Name",
  username: "Some Username",
};

fetch(postUrl, {
  method: "POST",
  body: JSON.stringify(data),
  headers: { "Content-Type": "application/json" },
})
  .then((res) => res.json())
  .then((data) => console.log(data))
  .catch((err) => console.error(err));
```

<hr>

### Fetch and HTTP status codes

By default, the fetch function does not consider HTTP status codes such as 404 (Not Found) or 500 (Internal Server Error) as errors. To check for HTTP errors, you can use the `ok` property of the Response object, which returns `true` if the status code is in the range 200-299 (successful) and `false` otherwise.

```js
const url = "https://jsonplaceholder.typicode.com/users";

fetch(url)
  .then((response) => {
    console.log(response.ok);
    console.log(response.status);

    if (!response.ok) {
      throw new Error(`HTTP error: ${response.status}`);
    }
    return response.json();
  })
  .then((data) => console.log(data))
  .catch((error) => console.error(error));
```

<hr>

### Headers

We can use the `get` method of the Headers object to retrieve the value of a specific header

```js
const url = "https://jsonplaceholder.typicode.com/users";

fetch(url)
  .then((response) => {
    console.log(response.ok);
    console.log(response.status);

    console.log(response.headers.get("Content-Type")); // "application/json"
  })
  .catch((error) => console.error(error));
```

Here is how to `set` headers using the `new Headers()` syntax:

```js
const postUrl = "https://httpbin.org/post";

const headers = new Headers();

headers.set("Authorization", "Bearer 123456");
headers.set("Content-Type", "application/json");

fetch(postUrl, {
  method: "POST",
  body: JSON.stringify({ name: "Some Name" }),
  headers: headers,
})
  .then((res) => {
    return res.json();
  })
  .then((data) => console.log(data))
  .catch((err) => console.error(err));
```

Here is how to `delete` headers using the `.delete()` method from the `Headers` object:

```js
const headers = new Headers();
headers.set("Authorization", "Bearer 123456");
headers.delete("Authorization");

fetch("https://example.com/api/users", {
  method: "POST",
  headers: headers,
})
  .then((res) => {
    return res.json();
  })
  .then((data) => console.log(data))
  .catch((error) => console.error(error));
```

<hr>

### Cancel a fetch request

We can cancel a `fetch` request by calling the `AbortController.abort()`. `AbortController` is a special built-in object and can be used to abort not only `fetch`, but other asynchronous tasks as well. To be able to cancel `fetch`, pass the `signal` property of an `AbortController` as a `fetch` option. For example, `fetch(url, {signal: controller.signal});`

```js
const url = "https://jsonplaceholder.typicode.com/users";

const controller = new AbortController();
const signal = controller.signal;

fetch(url, { signal })
  .then((res) => res.json())
  .then((data) => console.log(data))
  .catch((err) => console.error(err));

// Cancel the request
controller.abort();
```

`AbortController` has a single method `abort()`, and a single property `signal` that allows to set event listeners on it.

When `abort()` is called:

- `controller.signal` emits the `"abort"` event. This allows to set event listeners on this property.
- `controller.signal.aborted` property becomes `true`.

We can use the `AbortSignal.aborted` property to check if the signal has been aborted.

```js
const url = "https://jsonplaceholder.typicode.com/users";

const controller = new AbortController();
const signal = controller.signal;

fetch(url, { signal })
  .then((res) => res.json())
  .then((data) => console.log(data))
  .catch((err) => console.error(err));

// Cancel the request
controller.abort();

if (signal.aborted) {
  console.log("The request has been cancelled");
}
```

We can also use the `addEventListener` method to listen for the `abort` event, which is emitted when the `signal` is aborted.

```js
const url = "https://jsonplaceholder.typicode.com/users";

const controller = new AbortController();
const signal = controller.signal;

fetch(url, { signal })
  .then((res) => res.json())
  .then((data) => console.log(data))
  .catch((err) => console.error(err));

signal.addEventListener("abort", () => {
  console.log("The request has been cancelled");
});

// Cancel the request
controller.abort();
```

When a `fetch` is aborted, its promise rejects with an error `AbortError`.

<hr>
<hr>

## Regular Expressions

Regular expressions are patterns that provide a powerful way to search in and replace a text. In JavaScript, they are available via the `RegExp` object, as well as being integrated in string methods. A Regular Expression consists of a pattern and optional flags.

### Creating Regular Expressions

There are two syntaxes that can be used to create a regular expression object.

- The “long” syntax:

```js
const regexp = new RegExp("<pattern>" [, "<flags>"]);
```

- And the “short” one, using a regular expression literal. This one is done by using forward slashes `/<regexp>/`:

```js
const regexp = /pattern/; // no flags
```

```js
const regexp = /pattern/gim; // with flags g,m and i
```

You should use a regex literal when you know the regular expression pattern at the time of writing the code. On the other hand, use the `RegExp` constructor if the regex pattern is to be created dynamically. Also, the regex constructor lets you write a pattern using a template literal, but this is not possible with the regex literal syntax.

<hr>

### Flags

There are 6 flags in JavaScript's Regular Expressions:

- `i` - With this flag the search is case-insensitive: no difference between "A" and "a".
- `g` - With this flag the search looks for all matches, without it – only the first match is returned.
- `s` - Enables “dotall” mode, that allows a dot `.` to match newline character `\n`
- `u` - Enables full Unicode support. The flag enables correct processing of surrogate pairs.
- `m` - Multiline mode
- `y` - “Sticky” mode: searching at the exact position in the text

<hr>

### Regular Expression methods

#### `.match()`

The method `<string>.match(<regexp>)` finds all matches of `<regexp>` in the string `<string>`.

Here is an example without any flags. Without the flag `g`, it returns only the first match in the form of an array, with the full match at index 0 and some additional details in properties.

```js
const str = "We will, we will rock you";

const result = str.match(/we/);

console.log(result[0]); // we (1st match)
console.log(result.index); // 9 (position of the match)

console.log(result.input); // We will, we will rock you (source string)
console.log(result.length); // 1
```

We add the `i` flag to make the search case-insensitive.

```js
const str = "We will, we will rock you";

const result = str.match(/we/i);

console.log(result[0]); // We (1st match)
console.log(result.index); // 0 (position of the match)

console.log(result.input); // We will, we will rock you (source string)
console.log(result.length); // 1
```

Then, we add the flag `g` which returns an array of all matches.

```js
const str = "We will, we will rock you";

const result = str.match(/we/gi);

console.log(result); // Array [ "We", "we" ]
```

If there are no matches, `null` is returned.

```js
const str = "Hello";

const result = str.match(/bye/i);

console.log(result); // null
```

#### `.replace()`

The `<string>.replace(<string>, <replacement)` method could be used on strings to replace parts of the string.

```js
const str = "JavaScript";
const newStr = str.replace("ava", "").replace("cript", "");
console.log(newStr); // JS
```

The method could also be used with regular expressions. `<string>.replace(<regexp>, <replacement>)` replaces matches found using `<regexp>` in string `<string>` with `<replacement>` (all matches if there’s flag `g`, otherwise, only the first one).

```js
// no flag g
console.log("We will, we will".replace(/we/i, "I")); // I will, we will

// with flag g
console.log("We will, we will".replace(/we/gi, "I")); // I will, I will
```

There are symbols that we can use to control the replacement process.

| Symbols          | Actions                                                                                      |
| ---------------- | -------------------------------------------------------------------------------------------- |
| `$&`             | inserts the whole match                                                                      |
| `` $` ``         | inserts a string before the match                                                            |
| `$'`             | inserts a string after the match                                                             |
| `$$`             | inserts character `$`                                                                        |
| `$group_number`  | Works with capturing groups. Inserts the contents of a capturing group in the `group_number` |
| `$<group_name> ` | Works with capturing groups. Inserts the contents of the parentheses with the given `<name>` |

```js
console.log("I love HTML and CSS".replace(/HTML/, "$&, JavaScript")); // I love HTML, JavaScript and CSS
console.log("I love HTML and CSS".replace(/HTML/, "$`, JavaScript")); // I love I love , JavaScript and CSS
console.log("I love HTML and CSS".replace(/HTML/, "$', JavaScript")); // I love  and CSS, JavaScript and CSS
console.log("I love HTML and CSS".replace(/HTML/, "$$, JavaScript")); // I love $, JavaScript and CSS

console.log("Name Surname".replace(/(Name)\s(Surname)/, "$2, $1")); // Surname, Name

console.log(
  "Name Surname".replace(
    /(?<firstName>Name)\s(?<lastName>Surname)/,
    "$<lastName>, $<firstName>"
  )
); // Surname, Name
```

The `<replacement>` could also be a function. The `replace()` method will invoke the **replacer** function after the match has been performed and use the result of this function as the replacement string. The **replacer** function has the following syntax:

```js
function replacer(match, p1, p2, ..., offset, string);
```

The following are the meanings of each parameter:

- **match** is the matched substring.
- **p1, p2, …pn** are the nth string found by a parenthesized capture group provided by the regular expression.
- **offset** is the offset of the matched substring within the whole string being searched.
- **string** is the whole string being examined.

```js
const str = "I love HTML and CSS";

const result = str.replace(/(HTML)/, (match, p1, offset, string) => {
  console.log(match);
  console.log(p1);
  console.log(offset);
  console.log(string);

  return `HTML, JavaScript`;
});

console.log(result); // I love HTML, JavaScript and CSS
```

#### `.replaceAll()`

The main use case for `replaceAll` is replacing all occurrences of a string. This method is essentially the same as `<str>.replace()`, with two major differences:

- If the first argument is a string, it replaces all occurrences of the string, while `replace` replaces only the first occurrence.
- If the first argument is a regular expression, the `g` flag must be provided. Otherwise, there’ll be an error.

```js
const str = "I love HTML and CSS, HTML, HTML";

const result1 = str.replace(/(HTML)/g, (match, p1, offset, string) => {
  return match.toLowerCase();
});

const result2 = str.replaceAll(/(HTML)/g, (match, p1, offset, string) => {
  return match.toLowerCase();
});

console.log(result1); // I love html and CSS, html, html
console.log(result2); // I love html and CSS, html, html
```

#### `<regexp>.test()`

The method `<regexp>.test(<str>)` looks for at least one match, if found, returns `true`, otherwise `false`.

```js
const regexp = /hello/i;

console.log(regexp.test("Hello there")); // true
console.log(regexp.test("Hi there")); // false
```

<hr>

### Character classes

A character class is a special notation that matches any symbol from a certain set.

The **digit** class is written as `\d` and corresponds to “any single digit”.

```js
const phoneNumber = "+1(234)-567-89-01";

console.log(phoneNumber.match(/\d/)); // 1
console.log(phoneNumber.match(/\d/g)); // Array of 1, 2, 3 ... 9, 0, 1

console.log(phoneNumber.match(/\d/g).join("")); // 12345678901
```

The **space** class is denoted as `\s` and includes spaces, tabs `\t`, newlines `\n` and few other rare characters, such as `\v`, `\f` and `\r`.

```js
const str = "A sentence with some spaces.";

console.log(str.match(/\s/g)); // Array(4) [ " ", " ", " ", " " ]
```

The **word** class is denoted as `\w` and it is either a letter of Latin alphabet or a digit or an underscore \_. Non-Latin letters do not belong to `\w`.

```js
const str = "A word";

console.log(str.match(/\w/g)); // Array(5) [ "A", "w", "o", "r", "d" ]
```

A regexp may contain both regular symbols and character classes.

```js
const cssString = "CSS3 is the current version of CSS";

console.log(cssString.match(/CSS\d/)); // Array [ "CSS3" ]
```

A regexp can also contain one character class after another one.

```js
const str = "1 a";
const str2 = `1
a`;
const str3 = " abcde 12 ";

console.log(str.match(/\d\s\w/)); // matches - returns [ "1 a" ]
console.log(str2.match(/\d\s\w/)); // matches - returns [ "1\na" ]
console.log(str3.match(/\d\s\w/)); // doesnt't match - returns null
```

#### Inverse classes

For every character class there exists an “inverse class”, denoted with the same letter, but uppercased. The “inverse” means that it matches all other characters, for instance:

- `\D` means non-digit: any character except `\d`, for instance a letter.
- `\S` means non-space: any character except `\s`, for instance a letter.
- `\W` means non-wordly character: anything but `\w`, e.g a non-latin letter or a space.

In the below example, we find all the non-digits using `/\D/g`, and replace them.

```js
const phoneNumber = "+1(234)-567-89-01";

console.log(phoneNumber.replace(/\D/g, "")); // 12345678901
```

<hr>

### Using dot `.`

A dot `.` is a special character class that matches “any character except a newline”.

```js
console.log("ABcd".match(/./)); // Array [ "A" ]
console.log("ABcd".match(/./g)); // Array(4) [ "A", "B", "c", "d" ]

console.log("him".match(/hi./)); // Array [ "him" ]
console.log("his".match(/hi./)); // Array [ "his" ]
```

By default, a dot `.` doesn’t match the newline character `\n`.

```js
console.log("A-B".match(/A.B/)); // Array [ "A-B" ]
console.log("A B".match(/A.B/)); // Array [ "A B" ]
console.log("A\nB".match(/A.B/)); // null
```

If we want the dot `.` to include the newline character `\n` as well, then we can use the `s` flag.

```js
console.log("A\nB".match(/A.B/s)); // Array [ "A\nB" ]
```

<hr>

### Unicode encoding and `u` flag

JavaScript uses Unicode encoding for strings. Most characters are encoded with 2 bytes, but there are some that are 4 bytes. When JavaScript language was created, Unicode encoding was simpler: there were no 4-byte characters. So, some JavaScript features still handle 4-byte characters incorrectly. For instance, `length` treats 4 bytes as two 2-byte characters. Therefore, `length` thinks that there are two characters here:

```js
console.log("😄".length); // 2
console.log("𝒳".length); // 2
```

This might be problematic when we are working with regular expressions. To avoid the problem, we use the `u` flag. With the `u` flag, a regexp handles 4-byte characters correctly.

Every character in Unicode has a lot of properties. They describe what “category” the character belongs to and contain miscellaneous information about it. For instance, if a character has the `Letter` property, it means that the character belongs to an alphabet (of any language). A `Number` property means that it’s a digit: maybe Arabic or Chinese, and so on.

We can search for characters with a property, by writing `/\p{<unicode_property>}/u`. To use `\p{…}`, a regular expression must have the `u` flag. For instance, `\p{Letter}` denotes a letter in any language. We can also use `\p{L}`, as `L` is an alias of `Letter`.

```js
const str = "A ბ ㄱ";

console.log(str.match(/\p{L}/gu)); // Array(3) [ "A", "ბ", "ㄱ" ]
console.log(str.match(/\p{L}/g)); // null - `\p` doesn't work without the flag `u`
```

Here are the main character categories and their subcategories:

- Letter `L`:
  - lowercase `Ll`,
  - modifier `Lm`,
  - titlecase `Lt`,
  - uppercase `Lu`,
  - other `Lo`.
- Number `N`:
  - decimal digit `Nd`,
  - letter number `Nl`,
  - other `No`.
- Punctuation `P`:
  - connector `Pc`,
  - dash `Pd`,
  - initial quote `Pi`,
  - final quote `Pf`,
  - open `Ps`,
  - close `Pe`,
  - other `Po`.
- Mark `M` (accents etc):
  - spacing combining `Mc`,
  - enclosing `Me`,
  - non-spacing `Mn`.
- Symbol `S`:
  - currency `Sc`,
  - modifier `Sk`,
  - math `Sm`,
  - other `So`.
- Separator `Z`:
  - line `Zl`,
  - paragraph `Zp`,
  - space `Zs`.
- Other `C`:
  - control `Cc`,
  - format `Cf`,
  - not assigned `Cn`,
  - private use `Co`,
  - surrogate `Cs`.

Here are links to learn more about Unicode

- List all properties by a character: https://unicode.org/cldr/utility/character.jsp.
- List all characters by a property: https://unicode.org/cldr/utility/list-unicodeset.jsp.
- Short aliases for properties: https://www.unicode.org/Public/UCD/latest/ucd/PropertyValueAliases.txt.
- A full base of Unicode characters in text format, with all properties, is here: https://www.unicode.org/Public/UCD/latest/ucd/.

<hr>

### Anchors: string start `^` and end `$`

The caret `^` and dollar `$` characters have special meaning in a regexp. They are called **anchors**. The caret `^` matches at the beginning of the text, and the dollar `$` – at the end.

```js
const str = "Beginning is here. Here is the ending";

console.log(str.match(/^Beginning/)); // Array [ "Beginning" ]
console.log(str.match(/ending$/)); // Array [ "ending" ]
```

Both anchors together `^...$` are often used to test whether or not a string fully matches the pattern. For instance, to check if the user input is in the right format

```js
const goodInput = "12:34";
const badInput = "12:345";

const regexp = /^\d\d:\d\d$/;

console.log(regexp.test(goodInput)); // true
console.log(regexp.test(badInput)); // false
```

#### Multiline mode of anchors `^`, `$` and the flag `m`

The multiline mode with the flag `m` only affects the behavior of `^` and `$`. In the multiline mode anchors match not only at the beginning and the end of the string, but also at start/end of a line.

In the below example, the pattern `/^\d/gm` takes a digit from the beginning of each line:

```js
const str = `1st place
2nd place
3rd place`;

console.log(str.match(/^\d/gm)); // Array(3) [ "1", "2", "3" ]

// Without the flag `m` only the first digit is matched
console.log(str.match(/^\d/g)); // Array [ "1" ]
```

In the below example, the pattern `/\d$/gm` takes a digit from the end of each line:

```js
const str = `Winnie: 1
Piglet: 2
Eeyore: 3`;

console.log(str.match(/\d$/gm)); // Array(3) [ "1", "2", "3" ]

// Without the flag `m` only the digit at the end of the whole text is matched
console.log(str.match(/\d$/g)); // Array [ "3" ]
```

<hr>

### Word boundary: `\b`

A word boundary `\b` is similar to `^` and `$`. It tests if there is a word boundary. There are three different positions that qualify as word boundaries:

- At string start, if the first string character is a word character `\w`.
- Between two characters in the string, where one is a word character `\w` and the other is not.
- At string end, if the last string character is a word character `\w`.

```js
console.log("Hello, JavaScript!".match(/\bHello\b/)); // Array [ "Hello" ]
console.log("Hello, JavaScript!".match(/\bJavaScript\b/)); // Array [ "JavaScript" ]
console.log("Hello, JavaScript!".match(/\bHell\b/)); // null (no match)
console.log("Hello, JavaScript!".match(/\bJava!\b/)); // null (no match)
```

We can use `\b` with digits as well. For example, the pattern `\b\d\d\b` looks for standalone 2-digit numbers. In other words, it looks for 2-digit numbers that are surrounded by characters different from `\w`, such as spaces or punctuation.

```js
console.log("1 23 456 78".match(/\b\d\d\b/g)); // Array [ "23", "78" ]
console.log("12,34,56".match(/\b\d\d\b/g)); // Array(3) [ "12", "34", "56" ]
```

The word boundary test `\b` checks that there should be `\w `on the one side from the position and "not `\w`" – on the other side. But `\w `means a latin letter a-z (or a digit or an underscore), so the test doesn’t work for other characters, e.g. cyrillic letters or hieroglyphs.

<hr>

### Escaping Special characters

There are special characters in a regexp, such as `[ ] { } ( ) \ ^ $ . | ? * +`.

So far, we have used a backslash `\` as a special character in regex. It is used to denote character classes like `\d` for digits, `\s` for spaces, etc. But it's also used for escaping. If there is a special character, let's say a dot `.`, and we don't want to use the dot as a special character, then we can use `\` to indicate that we are looking for a regular dot. This is called escaping a character. By using the `\` we are escaping the special use case of a character.

```js
console.log("Chapter 5.1".match(/\d\.\d/)); // 5.1 (match!)
console.log("Chapter 511".match(/\d\.\d/)); // null (looking for a real dot \.)

// we don't escape the dot in the below example
console.log("Chapter 511".match(/\d.\d/)); // Array [ "511" ]
```

Here is one more example. Parenteses are special characters, so we are escaping them in the below example:

```js
console.log("function g()".match(/g\(\)/)); // Array [ "g()" ]
```

A slash symbol '/' is not a special character, but in JavaScript it is used to open and close the regexp: `/...pattern.../`, so we should escape it too:

```js
console.log("path/to/folder".match(/\//)); // Array [ "/" ]
```

If we’re not using `/.../`, but create a regexp using `new RegExp`, then we don’t need to escape it:

```js
console.log("path/to/folder".match(new RegExp("/"))); // Array [ "/" ]
```

From the above example, it's visible that `new Regexp()` accepts a string as an argument to create a regular expression. That might cause a problem with using a backslash, because backslash has its own meaning while used as part of a string. For example:

- `\n` – becomes a newline character,
- `\u0024` – becomes the Unicode character with such code,
- …And when there’s no special meaning: like `\d` or `\z`, then the backslash is simply removed.

```js
console.log("d\nd"); // d [new line] d
console.log("\u0024 "); // $ - unicode character
console.log("d.d"); // d.d
```

So, if we need to use `new Regexp()`, and we want to use the backslash in it, the way backslash is used in `/.../` pattern, then we need to use double backslash `\\`.

```js
const regStr = "\\d\\.\\d";
console.log(regStr); // \d\.\d

const regexp = new RegExp(regStr);
console.log("Chapter 5.1".match(regexp)); // 5.1
```

<hr>

### Sets and ranges

Several characters or character classes inside square brackets `[…]` mean to “search for any character among given”. That’s called a **set** and they can be used in a regexp along with regular characters:

```js
// find "t" or "m", and then "op"
console.log("Mop top".match(/[tm]op/gi)); // Array [ "Mop", "top" ]
```

Note that although there are multiple characters in the set, they correspond to exactly one character in the match.

```js
// find "V", then "o" or "i", then "la"
console.log("Voila".match(/V[oi]la/)); // null, no matches

console.log("Vila".match(/V[oi]la/)); // Array [ "Vila" ]

console.log("Vola".match(/V[oi]la/)); // Array [ "Vola" ]
```

Square brackets may also contain character ranges:

- `[a-z]` is a character in range from a to z
- `[0-5]` is a digit range from 0 to 5

```js
console.log("Exception 0xAF".match(/[0-9]x[A-F][A-F]/g)); // Array [ "0xAF" ]

// We can have more than one range in the same [ ... ]
console.log("Exception 0xAF".match(/[0-9]x[0-9A-F][0-9A-F]/g)); // Array [ "0xAF" ]
console.log("Exception 0xA5".match(/[0-9]x[0-9A-F][0-9A-F]/g)); // Array [ "0xA5" ]
```

We can also use special characters in sets:

- `\d` – is the same as `[0-9]`,
- `\w` – is the same as `[a-zA-Z0-9_]`,
- `\s` – is the same as `[\t\n\v\f\r ]`, plus few other rare Unicode space characters.

Besides normal ranges, there are “excluding” ranges that look like `[^…]`. They are denoted by a caret character `^` at the start and match any character except the given ones.

The example below looks for any characters except letters, digits and spaces:

```js
console.log("test15@example.com".match(/[^\d\sA-Z]/gi)); // Array [ "@", "." ]
```

In square brackets, we can use the vast majority of special characters without escaping:

- Symbols `. + ( )` never need escaping.
- A hyphen `-` is not escaped in the beginning or the end (where it does not define a range).
- A caret `^` is only escaped in the beginning (where it means exclusion).
- The closing square bracket `]` is always escaped (if we need to look for that symbol).

But if you decide to escape them just in case, then it won't be a problem.

<hr>

### Quantifiers `+`, `\*`, `?` and `{<number>}`

A quantifier is appended to a character (or a character class, or a set etc) and specifies how many we need.

The simplest quantifier is a number in curly braces: `{<number>}`. For example, `\d{4}` is the same as `\d\d\d\d`.

```js
console.log("1 12 123 1234 12345".match(/\d{4}/)); //  Array [ "123" ]
```

The range: `{3,5}` means match 3 to 5 times.

```js
console.log("1 12 123 1234 12345".match(/\d{3,5}/)); //  Array [ "123" ]
console.log("1 12 123 1234 12345".match(/\d{3,5}/g)); //  Array(3) [ "123", "1234", "12345" ]
```

We can omit the upper limit and write `{3,}`.

```js
console.log("1 12 123 1234 12345".match(/\d{3,}/)); //  Array [ "123" ]
console.log("1 12 123 1234 12345".match(/\d{3,}/g)); //  Array(3) [ "123", "1234", "12345" ]
```

Instead of writing something as `{1,}`, we can use the shorthand `+`. `+` means match something one or more times:

```js
console.log("1 12 123 1234 12345".match(/\d{1,}/)); //  Array [ "1" ]
console.log("1 12 123 1234 12345".match(/\d{1,}/g)); //  Array(5) [ "1", "12", "123", "1234", "12345" ]

console.log("1 12 123 1234 12345".match(/\d+/)); //  Array [ "1" ]
console.log("1 12 123 1234 12345".match(/\d+/g)); //  Array(5) [ "1", "12", "123", "1234", "12345" ]
```

Instead of writing something as `{0,1}`, we can use the shorthand `?`. `?` means match something zero times or once:

```js
const str = "Should I write color or colour?";

console.log(str.match(/colou{0,1}r/g)); // Array [ "color", "colour" ]
console.log(str.match(/colou?r/g)); // Array [ "color", "colour" ]
```

Instead of writing something as `{0,}`, we can use the shorthand `*`. `*` means match something zero times or more:

```js
console.log("100 10 1".match(/\d0*/g)); // Array(3) [ "100", "10", "1" ]
```

<hr>

### Greedy and lazy quantifiers

There is something called greedy search in regular expressions. In the greedy mode (by default), a quantified character is repeated as many times as possible.

To understand let's see an example. Let's say, we want to retrieve all the words that are in quotes from a sentence. Let's try using `/".+"/g`:

```js
const regexp = /".+"/g;

const str = 'a "witch" and her "broom" is one';

console.log(str.match(regexp)); // Array [ '"witch" and her "broom"' ]
```

It doesn't work. Instead of finding two matches "witch" and "broom", it finds one: "witch" and her "broom".

- First, JavaScript tries to find the quote. JavaScript finds the quote at the 3rd position.
- Then it tries to see if the rest of the subject string conforms to `.+"`.
- It tries to match the dot. Dot means any character, except the newline. So, the next character matches the dot. But we have provided `+` and therefore JavaScript tries to check if more characters match the dot. All characters match the dot, so it only stops when it reaches the end of the string.
- Now the engine finished repeating `.+` and tries to find the next character of the pattern. It’s the quote `"`. But the string has finished. The regular expression engine understands that it took too many `.+` and starts to backtrack.
- Now it assumes that `.+` ends one character before the string end and tries to match the rest of the pattern from that position. It keeps backtracking until it finds the quote.
- Finally, the result ends up being `"witch" and her "broom"`.

The **lazy** mode of quantifiers is an opposite to the greedy mode. It means: “repeat minimal number of times”. We can enable it by putting a question mark `?` after the quantifier. Usually a question mark `?` is a quantifier by itself (zero or one), but if added after another quantifier (or even itself) it gets another meaning – it switches the matching mode from greedy to lazy. So,

- `*` becomes `*?`,
- `+` becomes `+?`,
- `?` becomes `??`.

The regexp `/".+?"/g` works as intended: it finds "witch" and "broom":

```js
const regexp = /".+?"/g;

const str = 'a "witch" and her "broom" is one';

console.log(str.match(regexp)); // Array [ '"witch"', '"broom"' ]
```

<hr>

### Capturing groups

A part of a pattern can be enclosed in parentheses `(...)`. This is called a “capturing group”. It has two effects:

- It allows to get the part of a match as a separate item in the result array.
- If we put a quantifier after the parentheses, it applies to the parentheses as a whole.

```js
console.log("Gogogo now!".match(/go+/gi)); // Array(3) [ "Go", "go", "go" ]

console.log("Gogogo now!".match(/(go)+/gi)); // Array [ "Gogogo" ]
```

Parentheses are numbered from left to right. The search engine memorizes the content matched by each of them and allows to get it in the result. The method `<str>.match(<regexp>)`, if regexp has no flag `g`, looks for the first match and returns it as an array:

- At index 0: the full match.
- At index 1: the contents of the first parentheses.
- At index 2: the contents of the second parentheses.
- …and so on…

```js
const str = "<h1>Hello, world!</h1>";

const tag = str.match(/<(.*?)>/);

console.log(tag[0]); // <h1>
console.log(tag[1]); // h1
```

Parentheses can be nested.

```js
const str = '<span class="my">';

const regexp = /<(([a-z]+)\s*([^>]*))>/;

const result = str.match(regexp);
console.log(result[0]); // <span class="my">
console.log(result[1]); // span class="my"
console.log(result[2]); // span
console.log(result[3]); // class="my"
```

When we search for all matches (flag `g`), the `match` method does not return contents for capturing groups. For example, let’s find all tags in a string:

```js
const str = "<h1> <h2>";

const tags = str.match(/<(.*?)>/g);

console.log(tags); // Array [ "<h1>", "<h2>" ]
```

To get `groups` in the result, we should search using the method `<str>.matchAll(<regexp>)`. Just like `match`, it looks for matches, but there are 3 differences:

- It returns not an array, but an iterable object.
- When the flag `g` is present, it returns every match as an array with groups.
- If there are no matches, it returns not `null`, but an empty iterable object.

```js
let results = "<h1> <h2>".matchAll(/<(.*?)>/gi);

// results - is not an array, but an iterable object
console.log(results); // RegExp String Iterator {  }

console.log(results[0]); // undefined (*)

results = Array.from(results); // let's turn it into array

console.log(results[0]); // Array [ "<h1>", "h1" ]
console.log(results[1]); // Array [ "<h2>", "h2" ]
```

Remembering groups by their numbers is hard. For simple patterns it’s doable, but for more complex ones counting parentheses is inconvenient. We can give a name to a capturing group. That’s done by putting `?<group_name>` **immediately after the opening parenthesis**.

```js
const str = "2019-04-30";

const dateRegexp = /(?<year>[0-9]{4})-(?<month>[0-9]{2})-(?<day>[0-9]{2})/;

const groups = str.match(dateRegexp).groups;

console.log(groups); // Object { year: "2019", month: "04", day: "30" }
console.log(groups.year); // 2019
console.log(groups.month); // 04
console.log(groups.day); // 30
```

As you can see, the groups reside in the `.groups` property of the `match`. To look for all dates, we can add flag `g`. We’ll also need `matchAll` to obtain full matches, together with groups:

```js
const str = "2019-10-30 2020-01-01";

const dateRegexp = /(?<year>[0-9]{4})-(?<month>[0-9]{2})-(?<day>[0-9]{2})/g;

const results = str.matchAll(dateRegexp);

for (let result of results) {
  const { year, month, day } = result.groups;

  console.log(`${day}.${month}.${year}`);
  // first log: 30.10.2019
  // second log: 01.01.2020
}
```

Method `<str>.replace(<regexp>, <replacemen>t)` that replaces all matches with regexp in `<str>` allows to use parentheses contents in the `<replacement>` string. That’s done using `$group_number` syntax.

```js
const str = "John Bull";
const regexp = /(\w+) (\w+)/;

console.log(str.replace(regexp, "$2, $1")); // Bull, John
```

For named parentheses, the reference will be `$<name>`.

```js
const regexp = /(?<year>[0-9]{4})-(?<month>[0-9]{2})-(?<day>[0-9]{2})/g;

const str = "2019-10-30, 2020-01-01";

console.log(str.replace(regexp, "$<day>.$<month>.$<year>"));
// 30.10.2019, 01.01.2020
```

Sometimes we need parentheses to correctly apply a quantifier, but we don’t want their contents in results. A group may be excluded by adding `?:` in the beginning:

```js
const str = "Gogogo John!";

// ?: excludes 'go' from capturing
const regexp = /(?:go)+ (\w+)/i;

const result = str.match(regexp);

console.log(result[0]); // Gogogo John (full match)
console.log(result[1]); // John
console.log(result.length); // 2 (no more items in the array)
```

<hr>

### Backreferences in pattern: `\N` and `\k<name>`

We can use the contents of capturing groups `(...)` not only in the result or in the replacement string, but also in the pattern itself. A group can be referenced in the pattern using `\N`, where `N` is the group number.

```js
const str = `He said: "She's the one!".`;

// `\1` means “find the same text as in the first group”
const regexp = /(['"])(.*?)\1/g;

console.log(str.match(regexp)); // Array [ `"She's the one!"` ]
```

If we use `?:` in the group, then we can’t reference it. Groups that are excluded from capturing `(?:...)` are not memorized by the engine.

To reference a named group, we can use `\k<name>`.

```js
const str = `He said: "She's the one!".`;

const regexp = /(?<quote>['"])(.*?)\k<quote>/g;

console.log(str.match(regexp)); // Array [ `"She's the one!"` ]
```

<hr>

### Alternation (OR) `|`

Alternation is the term in regular expression that is actually a simple “OR”. In a regular expression, it is denoted with a vertical line character `|`.

```js
const regexp = /html|php|css|java(script)?/gi;

const str = "First HTML appeared, then CSS, then JavaScript";

console.log(str.match(regexp)); // Array(3) [ "HTML", "CSS", "JavaScript" ]
```

To apply alternation to a chosen part of the pattern, we can enclose it in parentheses:

- I love `HTML|CSS` matches I love HTML or CSS.
- I love `(HTML|CSS)` matches I love HTML or I love CSS.

```js
const str = "I love HTML and CSS";
const str2 = "I love CSS";

// This tries to find either "I love HTML" or "CSS"
console.log(str.match(/I love HTML|CSS/g)); // Array [ "I love HTML", "CSS" ]
console.log(str2.match(/I love HTML|CSS/g)); // Array [ "CSS" ]

// This tries to find either "I love HTML" or "I love CSS"
console.log(str.match(/I love (HTML|CSS)/g)); // Array [ "I love HTML" ]
console.log(str2.match(/I love (HTML|CSS)/g)); // Array [ "I love CSS" ]
```

One more example:

```js
// better time regexp
const regexp = /([01]\d|2[0-3]):[0-5]\d/g;

console.log("00:00 10:10 23:59 25:99 1:2".match(regexp)); // Array(3) [ "00:00", "10:10", "23:59" ]
```

<hr>

### Lookahead and lookbehind

Sometimes we need to find only those matches for a pattern that are followed or preceded by another pattern. There’s a special syntax for that, called “lookahead” and “lookbehind”, together referred to as “lookaround”. The syntax is: `X(?=Y)`, it means "look for X, but match only if followed by Y". There may be any pattern instead of X and Y. Please note: the lookahead is merely a test, the contents of the parentheses `(?=...)` is not included in the result.

```js
const str = "1 turkey costs 30€";

console.log(str.match(/\d+(?=€)/)); // Array [ "30" ], the number 1 is ignored, as it's not followed by €
```

More complex tests are possible, e.g. `X(?=Y)(?=Z)` means:

- Find X.
- Check if Y is immediately after X (skip if isn’t).
- Check if Z is also immediately after X (skip if isn’t).
- If both tests passed, then the X is a match, otherwise continue searching.

```js
const str = "1 turkey costs 30€";

// looks for \d+ that is followed by a space (?=\s), and there’s 30 somewhere after it (?=.*30)
console.log(str.match(/\d+(?=\s)(?=.*30)/)); // Array [ "1" ]
```

There is also a negative lookahead. The syntax is: `X(?!Y)`, it means "search X, but only if not followed by Y".

```js
const str = "2 turkeys cost 60€";

console.log(str.match(/\d+\b(?!€)/g)); // Array [ "2" ] (the price is not matched)
```

Lookahead allows to add a condition for “what follows”. Lookbehind is similar, but it looks behind. The syntax is:

- Positive lookbehind: `(?<=Y)X`, matches X, but only if there’s Y before it.
- Negative lookbehind: `(?<!Y)X`, matches X, but only if there’s no Y before it.

Please Note: Lookbehind is not supported in non-V8 browsers, such as Safari, Internet Explorer.

```js
const str = "1 turkey costs $30";

// the dollar sign is escaped \$
// Positive lookbehind
console.log(str.match(/(?<=\$)\d+/)); // Array [ "30" ] (skipped the sole number)

// Negative lookbehind
console.log(str.match(/(?<!\$)\b\d+/g)); // Array [ "1" ] (the price is not matched)
```

Generally, the contents inside lookaround parentheses does not become the part of a result. E.g. in the pattern `\d+(?=€)`, the € sign doesn’t get captured as a part of the match. That’s natural: we look for a number `\d+`, while `(?=€)` is just a test that it should be followed by €. But in some situations we might want to capture the lookaround expression as well, or a part of it. If we want that, just wrap that part into additional parentheses.

```js
const str = "1 turkey costs 30€";
const regexp1 = /\d+(?=€)/;
const regexp2 = /\d+(?=(€))/; // extra parentheses around €

console.log(str.match(regexp1)); // Array [ "30" ]
console.log(str.match(regexp2)); // Array [ "30", "€" ]
```

And here’s the same for lookbehind:

```js
const str = "1 turkey costs $30";
const regexp1 = /(?<=\$|£)\d+/;
const regexp2 = /(?<=(\$|£))\d+/;

console.log(str.match(regexp1)); // Array [ "30" ]
console.log(str.match(regexp2)); // Array [ "30", "$" ]
```

<hr>

### Catastrophic backtracking

We mentioned that to turn from the greedy search mode to the lazy mode, we need to `?` after a quantifier. But in some situations, we might want to keep the greedy search mode, but get rid of the backtracking. To stop the backtracking, we add `+` after a quantifier. That is, we use `\d++` instead of `\d+` to stop `+` from backtracking. With one more `+`, the quantifier, in this example `\d++`, becomes a **possessive quantifier**. Possessive quantifiers are in fact simpler than “regular” ones. They just match as many as they can, without any backtracking. The search process without backtracking is simpler.

<hr>

### Sticky flag `y`, searching at position

The flag `y` allows to perform the search at the given position in the source string. We can use this flag with `<regexp>.exec(<str>)` method. For a regexp without flags `g` and `y`, this method looks only for the first match, it works exactly like `<str>.match(<regexp>)`. But if there’s flag `g`, then it performs the search in `<str>`, starting from the position stored in the `<regexp>.lastIndex` property. And, if it finds a match, then sets `<regexp>.lastIndex` to the index immediately after the match. If we can `exec` again, the next `exec` will run starting from the `<regexp>.lastIndex`.

```js
const str = "let varName"; // Let's find all words in this string
const regexp = /\w+/g;

console.log(regexp.lastIndex); // 0 (initially lastIndex=0)

const word1 = regexp.exec(str);
console.log(word1[0]); // let (1st word)
console.log(regexp.lastIndex); // 3 (position after the match)

const word2 = regexp.exec(str);
console.log(word2[0]); // varName (2nd word)
console.log(regexp.lastIndex); // 11 (position after the match)

const word3 = regexp.exec(str);
console.log(word3); // null (no more matches)
console.log(regexp.lastIndex); // 0 (resets at search end)
```

Here is the implementation with the `for` loop:

```js
const str = "let varName";
const regexp = /\w+/g;

let result;

while ((result = regexp.exec(str))) {
  console.log(`Found ${result[0]} at position ${result.index}`);
  // Found let at position 0, then
  // Found varName at position 4
}
```

If we want the `exec` to start searching from a specific position in a string, we can manually set `lastIndex` to a number.

```js
const str = 'let varName = "value"';

const regexp = /\w+/g; // without flag "g", property lastIndex is ignored

regexp.lastIndex = 4;

const word = regexp.exec(str);
console.log(word); // Array [ "varName" ]
```

The `regexp.exec` call starts searching at position `lastIndex` and then goes further. If there’s no word at position `lastIndex`, but it’s somewhere after it, then it will be found. If we need to find a match exactly at the given position at the text, not somewhere after it, we can use flag `y`. The flag `y` makes `<regexp>.exec` to search exactly at the position `lastIndex`, not “starting from” it.

```js
const str = 'let varName = "value"';

const regexp = /\w+/y;

regexp.lastIndex = 3;
console.log(regexp.exec(str)); // null (there's a space at position 3, not a word)

regexp.lastIndex = 4;
console.log(regexp.exec(str)); // Array [ "varName" ] (word at position 4)
```

<hr>

### Methods of RegExp and String

The `.split(<delimiter>)` could be used on a string without regular expressions. It splits a string by a provided delimiter. However, we can also use it with a regular expression.

```js
console.log("12, 34, 56".split(/,\s*/)); // Array(3) [ "12", "34", "56" ]
```

The method `<str>.search(<regexp>)` returns the position of the first match or `-1` if none found. `search` only finds the first match:

```js
const str = "A drop of ink may make a million think";

console.log(str.search(/ink/i)); // 10 (first match position
```

<hr>

### Summary of Regular Expressions

Here is a brief summary of some concepts in the regular expressions:

```js
const shortStr = "This is a short text.";
const longStr = `Here is a long text.
This is a multiline one.
It has numbers "like" 123 or 45678, also numbers with "symbols" +1-234-4567-89-01.
It has a lot more "symbols such as" [ ] ( ) * & $ ! @.`;

// Simple match with all the details that could be access through the result
console.log(longStr.match(/is/)); // Array [ "is" ]

console.log(Array.isArray(longStr.match(/is/))); // true, the result of `match` comes as an array, if there's a match
console.log(longStr.match(/no match/)); // returns null, if there's no match

console.log(longStr.match(/is/)[0]); // is
console.log(longStr.match(/is/).length); // 1, the number of matches
console.log(longStr.match(/is/).index); // 5, the position of the matched string in the source string
console.log(longStr.match(/is/).input); // the source string, where the search happens

console.log(longStr.match(/is/g)); // Array(3) [ "is", "is", "is" ], flag `g` returns all matches
console.log(longStr.match(/is/g).length); // 3
console.log(longStr.match(/is/g).index); // undefined, with the `g` flag, `match` doesn't return additional details about the match
console.log(longStr.match(/is/g).input); // undefined, with the `g` flag, `match` doesn't return additional details about the match

console.log(longStr.matchAll(/is/g)); // `matchAll` mustbe called with the flag `g`
const matchAllArr = Array.from(longStr.matchAll(/is/g)); // `matchAll` returns an iterable object, we can convert it to an array, if we are going to iterate through it more than once
console.log(matchAllArr); // Array(3) [ (1) […], (1) […], (1) […] ]
console.log(matchAllArr.length); // 3

// `matchAll` has access to additional details for all the matches
console.log(matchAllArr[0].length); // 1, the number of matches in the array for the first match, same as `longStr.match(/is/).length`
console.log(matchAllArr[0].index); // 5, the position of the first matched string in the source string, same as `longStr.match(/is/).index`
console.log(matchAllArr[0].input); // the source string, where the search happens, same as `longStr.match(/is/).input`

console.log(longStr.matchAll(/no match/g)); // returns an empty iterable object, if there's no match

console.log(longStr.match(/it/g)); // Array [ "it" ], the "it" is from "...with..." in the source
console.log(longStr.match(/it/gi)); // Array(3) [ "It", "it", "It" ], flag `i` makes the search case-insensitive

console.log(/it/i.test(longStr)); // true, returns true on the first match
console.log(/no match/i.test(longStr)); // false, returns false if no match

console.log(/it/gi.test(longStr)); // true, flag `g` doesn't matter with `test`, as it returns true on the first match

console.log(shortStr.replace("short", "very short")); // This is a very short text. `replace` could be used with a simple string
console.log(shortStr.replace(/short/, "very short")); // This is a very short text. `replace` could be used with regexp

console.log(shortStr.replace(/short/, "very $&")); // This is a very short text. `$&` is the matched string
console.log(shortStr.replace(/short/, "...hapchi... I said, $`short")); // This is a ...hapchi... I said, This is a short text. `$`` is the string before the matched string.
console.log(shortStr.replace(/short/, "$'")); // This is a  text. text. `$'` is the string after the matched string.
console.log(shortStr.replace(/short/, "$$")); // This is a $ text. `$$` is $.

console.log(shortStr.replace(/(This) (is)/, "$2 $1")); // is This a short text. `$1` is (This) and `$2` is (is).
console.log(
  shortStr.replace(
    /(?<firstWord>This) (?<secondWord>is)/,
    "$<secondWord> $<firstWord>"
  )
); // is This a short text. `$<firstWord>` is (This) and `$<secondWord>` is (is).

// `replace` accepts a function whose return value will be used as a replacement
console.log(
  "A\nB\nC".replace(/A/, function (match, offset, string) {
    return `Return from func: match: ${match}, offset: ${offset}, input string: ${string}. The End.`;
  })
);
/* Return from func: match: A, offset: 0, input string: A
B
C. The End.
B
C */

// matching string, capturing groups, the offset of the position of the match from the beginning of the source string, and the source string itself could be accessed
console.log(
  "A\nB\nC".replace(/(A)/, function (match, p1, offset, string) {
    return `Return from func: match: ${match}, capturing group: ${p1}, offset: ${offset}, input string: ${string}. The End.`;
  })
);
/* Return from func: match: A, capturing group: A, offset: 0, input string: A
B
C. The End.
B
C */

// the more capturing groups are accessed between match and offset parameters
console.log(
  "A\nB\nC".replace(/(A)\n(B)/, function (match, p1, p2, offset, string) {
    return `Return from func: match: ${match}, capturing group 1: ${p1}, capturing group 2: ${p2}, offset: ${offset}, input string: ${string}. The End.`;
  })
);
/* Return from func: match: A
B, capturing group 1: A, capturing group 2: B, offset: 0, input string: A
B
C. The End.
C */

console.log(shortStr.replaceAll(/is/g, "IS")); // ThIS IS a short text. `replaceAll` must be used with the flag `g`
console.log(shortStr.replace(/is/g, "IS")); // ThIS IS a short text, `replace` with the flag `g` is the same as `replaceAll`

console.log(longStr.match(/\d/)); // Array [ "1" ], `\d` returns digits
console.log(longStr.match(/\D/)); // Array [ "H" ], `\d` returns non-digits

console.log(longStr.match(/\s/)); // Array [ " " ], `\d` returns spaces
console.log(longStr.match(/\S/)); // Array [ "H" ], `\d` returns non-spaces

console.log(longStr.match(/\w/)); // Array [ "H" ], `\d` returns wordly characters
console.log(longStr.match(/\W/)); // Array [ " " ], `\d` returns non-wordly characters

console.log(longStr.match(/./g)); // matches any character except the newline
console.log(longStr.match(/./gs)); // with flag `s`, `.` matches the newline character as well

console.log(longStr.match(/^Here/gi)); // Array [ "Here" ], `^` anchor searches the beginning of a string
console.log(longStr.match(/\.$/gi)); // Array [ "." ], `$` anchor searches the end of a string

console.log(longStr.match(/^It/gim)); // Array [ "It", "It" ], `^` with the flag `m` searches the beggining of every line
console.log(longStr.match(/\.$/gim)); // Array(4) [ ".", ".", ".", "." ], `$` with the flag `m` searches the end of every line

console.log(longStr.match(/it/gi)); // Array(3) [ "It", "it", "It" ], the second "it" is from "...with..." in the source
console.log(longStr.match(/\bit\b/gi)); // Array [ "It", "It" ], `\b` means a word boundary, a non-`\w` character

console.log(longStr.match(/\b[Ii]t\b/g)); // Array [ "It", "It" ], `[Ii ]` means one of I or i
console.log(longStr.match(/\bit\b/g)); // null

console.log(longStr.match(/\b[^Ii]t\b/g)); // null, `[^Ii ]` means any character other than I or i

console.log(longStr.match(/\d{3}/g)); // Array(3) [ "123", "234", "456" ], `\d{3}` is the same as \d\d\d
console.log(longStr.match(/\d{3,}/g)); // Array(3) [ "123", "234", "4567" ], `\d{3,}` means 3 or more digits
console.log(longStr.match(/\d{4,5}/g)); // Array [ "45678", "4567" ], `\d{4,5}` means 4 or 5 digits

console.log(longStr.match(/\d+/g)); // Array(7) [ "123", "45678", "1", "234", "4567", "89", "01" ], `+` means {1,}
console.log(longStr.match(/4\d?/g)); // Array(3) [ "45", "4", "45" ], `?` means {0,1}
console.log(longStr.match(/4\d*/g)); // Array(3) [ "45678", "4", "4567" ], `*` means {0,}

console.log(longStr.match(/".+?"/gi)); // Array(3) [ '"like"', '"symbols"', '"symbols such as"' ], +? turns on the lazy mode for +
console.log(longStr.match(/".??"/gi)); // null, ?? turns on the lazy mode for ?
console.log(longStr.match(/".*?"/gi)); // Array(3) [ '"like"', '"symbols"', '"symbols such as"' ], +? turns on the lazy mode for *

// match
// matchAll
// test
// replace
// replaceAll

// g
// i
// s
// u
// m
// y

// $&
// $`
// $'
// $$
// $group_number
// $<group_name>

// \d
// \s
// \w

// \D
// \S
// \W

// .

// ^
// $
// \b

// [ ]
// [^ ]

// {<number>}
// {<number>,}
// {<lower_limit_number>,<upper_limit_number>}
// + same as {1,}
// ? same as {0,1}
// * same as {0,}

// +?
// *?
// ??

// ( )
// ( ( ) ( ) )
// (?: )

// (?<group_name>)
// (\group_number)
// (\k<group_name)

// |
// ( | )

// (?=)
// (?!)
// (?<=)
// (?<!)

// (?=( ))

// \d++
// \w++

// exec with lastIndex and flag y
```

<hr>
<hr>

## URL

### Creating a `URL` object

The built-in `URL` class provides a convenient interface for creating and parsing URLs. The syntax to create a new URL object is `new URL(<url>, [<base>])`

- `<url>` – the full URL or only path (if `<base>` is set),
- `<base>` – an optional base URL: if set and `<url>` argument has only path, then the URL is generated relative to base.

```js
const url = new URL("https://example.com/path/to/folder");

console.log(url.href); // https://example.com/path/to/folder
```

```js
const url = new URL("path/to/folder", "https://example.com");

console.log(url.href); // https://example.com/path/to/folder
```

We can easily create a new `URL` based on the path relative to an existing URL:

```js
const url = new URL("https://example.com/path/to/folder");
const newUrl = new URL("newPath", url);

console.log(newUrl.href); // 'https://example.com/path/to/newPath'
```

<hr>

### Properties of a `URL` object

The `URL` object has a lot of properties that inform us about the url.

```js
const url = "https://example.org:8080/foo/bar?q=baz#bang";
const newUrl = new URL(url);

console.log("protocol: ", newUrl.protocol); // protocol:  https:
console.log("hostname: ", newUrl.hostname); // hostname:  example.org
console.log("port: ", newUrl.port); // port:  8080
console.log("host: ", newUrl.host); // host:  example.org:8080
console.log("origin: ", newUrl.origin); // origin:  https://example.org:8080
console.log("pathname: ", newUrl.pathname); // pathname:  /foo/bar
console.log("search: ", newUrl.search); // search:  ?q=baz
console.log("hash: ", newUrl.hash); // hash:  #bang
console.log("href: ", newUrl.href); // href:  https://example.org:8080/foo/bar?q=baz#bang
console.log("toString(): ", newUrl.toString()); // toString():  https://example.org:8080/foo/bar?q=baz#bang
console.log("toJSON(): ", newUrl.toJSON()); // toJSON():  https://example.org:8080/foo/bar?q=baz#bang
```

Generally, the `URL` object can be passed to any method (for example, `fetch`) instead of a string, as most methods will perform the string conversion, that turns a `URL` object into a string with full URL.

<hr>

### `URLSearchParams`

If we want to add search parameters to a url, we can add it into a url string. However, we can also use `<url>.searchParams`, an object of type `URLSearchParams`. It provides convenient methods for search parameters:

- `append(<name>, <value>)` – add the parameter by name,
- `delete(<name>)` – remove the parameter by name,
- `get(<name>)` – get the parameter by name,
- `getAll(<name>)` – get all parameters with the same name (that’s possible, e.g. `?user=John&user=Pete`),
- `has(<name>)` – check for the existence of the parameter by name,
- `set(<name>, <value>)` – set/replace the parameter,
- `sort()` – sort parameters by name,
- …and it’s also iterable, similar to `Map`.

```js
const url = new URL("https://example.org:8080/query?q1=value1");
console.log(url.search); // ?q1=value1

url.searchParams.append("q2", "value2.1");
console.log(url.search); // ?q1=value1&q2=value2.1

url.searchParams.delete("q2");
console.log(url.search); // ?q1=value1

console.log(url.searchParams.has("q1")); // true
console.log(url.searchParams.has("q2")); // false

url.searchParams.set("q2", "value2.1");
url.searchParams.append("q2", "value2.2");

console.log(url.searchParams.get("q1")); // value1
console.log(url.searchParams.getAll("q2")); // Array [ "value2.1", "value2.2" ]
```

The reason why using `URLSearchParams` could be better is because search parameters need to be encoded if they contain spaces, non-latin letters, etc. If we are manually adding a search parameter to a url string, then we would also need to add the encoding for some characters.

```js
const url = new URL("https://example.com/query");

url.searchParams.set("queryKey", "query value!"); // added parameter with a space and !
console.log(url.href); // https://example.com/query?queryKey=query+value%21

url.searchParams.set("queryKey", "query:value"); // added parameter with a colon :
// parameters are automatically encoded
console.log(url.href); // https://example.com/query?queryKey=query%3Avalue

console.log(url.searchParams); // URLSearchParams { queryKey → "query:value" }

// iterate over search parameters (decoded)
for (let [name, value] of url.searchParams) {
  console.log(`${name}=${value}`); // queryKey=query:value
}
```

There’s a standard RFC3986 that defines which characters are allowed in URLs and which are not. The good news is that `URL` objects handle all of that automatically:

```js
const url = new URL("https://example.az/ƏÜĞ");

url.searchParams.set("key", "Ç");

// url is automatically encoded
console.log(url.href); // https://example.az/%C6%8F%C3%9C%C4%9E?key=%C3%87
console.log(url.searchParams); // URLSearchParams { key → "Ç" }
```

<hr>

### Functions for encoding and decoding url and url components

Even though `new URL` and `URLSearchParams` are convenient for encoding and decoding, we might need to add a url as a string at some point. If we use a string though, we need to encode/decode special characters manually. There are built-in functions for that:

- `encodeURI` – encodes URL as a whole.
- `decodeURI` – decodes it back.
- `encodeURIComponent` – encodes a URL component, such as a search parameter, or a hash, or a pathname.
- `decodeURIComponent` – decodes it back.

What’s the difference between `encodeURIComponent` and `encodeURI`? When we should use either? There are characters that are allowed in the whole URL, but they need to be encoded when it's part of some URL component such as a search parameter. For example, characters such as `:`, `?`, `=`, `&`, `#` are allowed in URL but they have a special meaning as part of some URL components.

- `encodeURI` encodes only characters that are totally forbidden in URL.
- `encodeURIComponent` encodes same characters, and, in addition to them, characters `#`, `$`, `&`, `+`, `,`, `/`, `:`, `;`, `=`, `?` and `@`.

```js
const param = encodeURIComponent("test1&test2");
const url = `https://example.com/?q=${param}`;

console.log(url); // 'https://example.com/?q=test1%26test2'
```

```js
const param = encodeURI("test1&test2");
const url = `https://example.com/?q=${param}`;

console.log(url); // 'https://example.com/?q=test1&test2'
```

There are cases where `encodeURI*` functions will not work. Classes `URL` and `URLSearchParams` are based on the latest URI specification: RFC3986, while `encodeURI*` functions are based on the obsolete version RFC2396. There are a few differences, e.g. IPv6 addresses are encoded wrong with `encodeURI`:

```js
// valid url with IPv6 address
const url = "http://[2607:f8b0:4005:802::1007]/";

console.log(encodeURI(url)); // http://%5B2607:f8b0:4005:802::1007%5D/
console.log(new URL(url).href); // http://[2607:f8b0:4005:802::1007]/
```

<hr>

### `createObjectURL()` and `revokeObjectURL()`

There are 2 static methods in the URL constructor. It has the `createObjectURL()` method and the `revokeObjectURL()` method. The `createObjectURL()` static method creates a `DOMString` containing a URL representing the object given in the parameter. A `DOMString` is a UTF-16 encoded string. Since JavaScript uses UTF-16 strings, `DOMString`s are mapped directly to strings. The `createObbjectURL()` method accepts an object, which can be a `File`, `Blob`, or `MediaSource` object to create a URL for.

```js
const objUrl = URL.createObjectURL(new File([""], "filename"));
console.log(objUrl); // blob:http://...
```

The browsers will release object `URL`s automatically when the document is unloaded, but for the sake of improving performance, we should release it manually. The `revokeObjectURL()` method takes in an object `URL` as its argument.

```js
const objUrl = URL.createObjectURL(new File([""], "filename"));
console.log(objUrl); // blob:http://...

URL.revokeObjectURL(objUrl); // returns undefined
```

Here is an example, where we receive an image from a server, turn it into a url and show as an image:

```js
fetch("https://picsum.photos/400/400")
  .then((res) => res.blob())
  .then((blob) => handler(blob));

function handler(blob) {
  const url = URL.createObjectURL(blob);

  const img = new Image();
  img.src = url;

  img.onload = () => {
    document.body.appendChild(img);
    URL.revokeObjectURL(url);
  };
}
```

<hr>
<hr>

## Binary files

### `ArrayBuffer`

`ArrayBuffer` is a JavaScript constructor that can be used to allocate a specific number of
bytes in memory. It is an array of bytes. `ArrayBuffer` is the chunk of memory that is set aside to hold typed arrays (`Int8Array`, `UInt8Array` etc). The syntax to create an `ArrayBuffer` is `new ArrayBuffer(<bytes>)`:

```js
const buffer = new ArrayBuffer(16); // create a buffer of length of 16 bytes
console.log(buffer.byteLength); // 16
```

This allocates a contiguous memory area of 16 bytes and pre-fills it with zeroes.

Let’s eliminate a possible source of confusion. `ArrayBuffer` is not `Array`:

- It has a fixed length, we can’t increase or decrease it.
- It takes exactly that much space in the memory.
- To access individual bytes, another “view” object is needed, not `<buffer>[<index>]`.

<hr>

#### Typed Arrays

We cannot interact with the `ArrayBuffer` directly. To manipulate an `ArrayBuffer`, we need to use a view object. A view object does not store anything on its own. It’s the “eyeglasses” that give an interpretation of the bytes stored in the `ArrayBuffer`.

```js
const buffer = new ArrayBuffer(16); // create a buffer of length of 16 bytes, 8-bit (1 byte) * 16 bytes = 128 bits

const view = new Uint32Array(buffer); // view the buffer as a sequence of 32-bit integers

console.log(Uint32Array.BYTES_PER_ELEMENT); // 16 bytes / 32 bits = 128 bits / 32 bits = 4 bytes per integer

console.log(view.length); // 4, it stores that many integers
console.log(view.byteLength); // 16, the size in bytes

// let's write a value
view[0] = 123456;

// iterate over values
for (let num of view) {
  console.log(num); // 123456, then 0, 0, 0 (4 values total)
}

// use the spread operator with a typed array
console.log(...view); // 123456 0 0 0
```

The common term for all these views (`Uint8Array`, `Uint32Array`, etc) is **typed array**. Please note, there’s no constructor called TypedArray, it’s just a common “umbrella” term to represent one of views over `ArrayBuffer`: `Int8Array`, `Uint8Array` and so on. Typed arrays behave like regular arrays: have indexes and are iterable.

There are various typed arrays:

- `Int8Array` - is an array of 8-bit integers. These integers can be in the range of -128 to 127.
- `UInt8Array` (unsigned array) - is an array of 8-bit integers. These integers can be in the range of 0 to 255.
- `UInt8ClampedArray` (unsigned and clamped array) - is an array of 8-bit integers. These integers can be in the range of 0 to 255. Clamped means that if you try to put a number less than 0, it will be converted to 0. If you try to put a number greater than 255, it will be converted to 255.
- `Int16Array` - is an array of 16-bit integers. These integers can be in the range of -32768 to 32767.
- `UInt16Array` (unsigned array) - is an array of 16-bit integers. These integers can be in the range of 0 to 65535.
- `Int32Array` - is an array of 32-bit integers. These integers can be in the range of -2147483648 to 2147483647.
- `UInt32Array` (unsigned array) - is an array of 32-bit integers. These integers can be in the range of 0 to 4294967295.
- `Float32Array` - for signed floating-point numbers of 32. It treats every 4 bytes as a floating point number.
- `Float64Array` - for signed floating-point numbers of 64 bits. It treats every 8 bytes as a floating point number with possible values from 5.0x10^-324 to 1.8x10^308.

A typed array constructor (be it `Int8Array` or `Float64Array`, doesn’t matter) behaves differently depending on argument types. There are 5 variants of arguments:

```js
new <TypedArray>(<buffer>, [<byteOffset>, <length>]);
new <TypedArray>(<object>);
new <TypedArray>(<typedArray>);
new <TypedArray>(<length>);
new <TypedArray>();
```

- If an `<ArrayBuffer>` argument is supplied, the view is created over it.
  - Optionally, we can provide `<byteOffset>` to start from (0 by default) and the `<length>` (till the end of the buffer by default), then the view will cover only a part of the buffer.
- If an Array, or any array-like object is given, it creates a typed array of the same length and copies the content. We can use it to pre-fill the array with the data:

```js
const arr = new Uint8Array([0, 1, 2, 3]);
console.log(arr.length); // 4, created binary array of the same length
console.log(arr[1]); // 1, filled with 4 bytes (unsigned 8-bit integers) with given values
```

- If another typed array is supplied, it does the same: creates a typed array of the same length and copies values. Values are converted to the new type in the process, if needed.

```js
const arr16 = new Uint16Array([1, 1000]);
const arr8 = new Uint8Array(arr16);
console.log(arr8[0]); // 1
console.log(arr8[1]); // 232, tried to copy 1000, but can't fit 1000 into 8 bits
```

- For a numeric argument length – creates the typed array to contain that many elements. Its byte length will be length multiplied by the number of bytes in a single item `<TypedArray>.BYTES_PER_ELEMENT`:

```js
const arr = new Uint16Array(4); // create typed array for 4 integers, 4 * 16-bit = 64-bit
console.log(Uint16Array.BYTES_PER_ELEMENT); // 2 bytes per integer, 2 bytes = 16-bit = 1 integer
console.log(arr.byteLength); // 8 (size in bytes), 4 integers - 64-bit, 64 / 8-bit(1 byte) = 8 bytes
```

- Without arguments, creates a zero-length typed array.

We can create a typed array directly, without mentioning `ArrayBuffer`. But a view cannot exist without an underlying `ArrayBuffer`, so it gets created automatically in all these cases except the first one (when provided).

- To access the underlying `ArrayBuffer`, there are following properties in TypedArray:

  - `buffer` – references the `ArrayBuffer`.
  - `byteLength` – the length of the `ArrayBuffer`.

This lets us to move from one view to another easily:

```js
const arr8 = new Uint8Array([0, 1, 2, 3]);

// another view on the same data
const arr16 = new Uint16Array(arr8.buffer);
```

<hr>

#### Typed Array Methods

Typed arrays have regular `Array` methods, with notable exceptions. We can iterate with `map`, `slice`, `find`, `reduce` etc.

There are few things we can’t do though:

- No `splice` – we can’t “delete” a value, because typed arrays are views on a buffer, and these are fixed, contiguous areas of memory. All we can do is to assign a zero.
- No `concat` method.

There are two additional methods that typed arrays have:

- `<typedArray>.set(<fromArr>, [<offset>])` copies all elements from `<fromArr>` to the `<typedArray>`, starting at position `<offset>` (0 by default).
- `<typedArray>.subarray([<begin>, <end>])` creates a new view of the same type from `<begin>` to `<end>` (exclusive). That’s similar to `slice` method, but doesn’t copy anything – just creates a new view, to operate on the given piece of data.

<hr>

#### `DataView`

`DataView` is a special super-flexible “untyped” view over `ArrayBuffer`. It allows to access the data on any offset in any format. `DataView` is great when we store mixed-format data in the same buffer.

- For typed arrays, the constructor dictates what the format is. The whole array is supposed to be uniform. The i-th number is `<arr>[<i>]`.
- With `DataView` we access the data with methods like `.getUint8(<i>)` or `.getUint16(<i>)`. We choose the format at method call time instead of the construction time. We also set the data with methods like `setUint8()`, `setUint16()`, etc.

The syntax is `new DataView(<buffer>, [<byteOffset>], [<byteLength>])`.

- `<buffer>` – the underlying `ArrayBuffer`. Unlike typed arrays, `DataView` doesn’t create a buffer on its own. We need to have it ready.
- `<byteOffset>` – the starting byte position of the view (by default 0).
- `<byteLength>` – the byte length of the view (by default till the end of buffer).

```js
// binary array of 4 bytes, all have the maximal value 255
const buffer = new Uint8Array([255, 255, 255, 255]).buffer;

const dataView = new DataView(buffer);

// get 8-bit number at offset 0
console.log(dataView.getUint8(0)); // 255

// now get 16-bit number at offset 0, it consists of 2 bytes, together interpreted as 65535
console.log(dataView.getUint16(0)); // 65535 (biggest 16-bit unsigned int)

// get 32-bit number at offset 0
console.log(dataView.getUint32(0)); // 4294967295 (biggest 32-bit unsigned int)

dataView.setUint32(0, 0); // set 4-byte number to zero, thus setting all bytes to 0
```

<hr>

### `TextDecoder` and `TextEncoder`

#### `TextDecoder`

What if the binary data is actually a string? The built-in `TextDecoder` object allows one to read the value into an actual JavaScript string, given the buffer and the encoding.

- We first need to create it with `new TextDecoder([<encoding>], [<options>])`

  - `<encoding>` – `utf-8` by default, but `big5`, `windows-1251` and others are also supported.
  - `<options>` – optional object:
    - `fatal` – boolean, if `true` then throw an exception for invalid (non-decodable) characters, otherwise (default) replace them with character \uFFFD.
    - `ignoreBOM` – boolean, if `true` then ignore BOM (an optional byte-order Unicode mark), rarely needed.

- After creating the `TextDecoder`, we can decode with `.decode([<input>], [<options>])`

  - `<input>` – BufferSource to decode.
  - `<options>` – optional object:
    - `stream` – true for decoding streams, when decoder is called repeatedly with incoming chunks of data. In that case a multi-byte character may occasionally split between chunks. This option tells `TextDecoder` to memorize “unfinished” characters and decode them when the next chunk comes.

```js
const uint8Array = new Uint8Array([72, 101, 108, 108, 111]);
console.log(new TextDecoder().decode(uint8Array)); // Hello
```

We can decode a part of the buffer by creating a subarray view for it:

```js
const uint8Array = new Uint8Array([0, 72, 101, 108, 108, 111, 0]);

// the string is in the middle
// create a new view over it, without copying anything
const binaryString = uint8Array.subarray(1, -1);

console.log(new TextDecoder().decode(binaryString)); // Hello
```

<hr>

#### `TextEncoder`

`TextEncoder` does the reverse thing – converts a string into bytes. The syntax is `new TextEncoder()`. The only encoding it supports is “utf-8”. It has two methods:

- `encode(<str>)` – returns `Uint8Array` from a string.
- `encodeInto(<str>, <destination>)` – encodes `<str>` into `<destination>` that must be `Uint8Array`.

```js
const encoder = new TextEncoder();

const uint8Array = encoder.encode("Hello");
console.log(uint8Array); // Uint8Array(5) [ 72, 101, 108, 108, 111 ]

console.log(new TextDecoder().decode(uint8Array)); // Hello
```

<hr>

### Blob

`ArrayBuffer` and views are parts of ECMA standard, parts of JavaScript. In the browser, there are additional higher-level objects, described in the File API, in particular `Blob`. Blob stands for Binary Large Object. It's basically any binary file.

The constructor syntax is `new Blob(<blobParts>, <options>);`

- `<blobParts>` is an array of Blob/BufferSource/String values. The first argument to `Blob` must be an array.
- `<options>` optional object:
  - `type` – Blob type, usually MIME-type, e.g. image/png, text/plain, etc.
  - `endings` – whether to transform end-of-line to make the Blob correspond to current OS newlines (\r\n or \n). By default `"transparent"` (do nothing), but also can be `"native"` (transform).

```js
// create Blob from a typed array and strings
const helloArr = new Uint8Array([72, 101, 108, 108, 111]); // "Hello" in binary form

const blob = new Blob([helloArr, " ", "world"], { type: "text/plain" });

console.log(helloArr); // Uint8Array(5) [ 72, 101, 108, 108, 111 ]
console.log(blob); // Blob { size: 11, type: "text/plain"
```

We can’t change data directly in a Blob, but we can slice parts of a Blob, create new Blob objects from them, mix them into a new Blob and so on. This behavior is similar to JavaScript strings: we can’t change a character in a string, but we can make a new corrected string.

We can extract Blob slices with `<blob>.slice([<byteStart>], [<byteEnd>], [<contentType>]);`

- `<byteStart>` – the starting byte, by default 0.
- `<byteEnd>` – the last byte (exclusive, by default till the end).
- `<contentType>` – the type of the new blob, by default the same as the source.

The arguments are similar to `<array>.slice`, negative numbers are allowed too.

The `Blob` constructor allows to create a blob from almost anything, including any BufferSource. If we need to perform low-level processing, we can get the lowest-level `ArrayBuffer` from `<blob>.arrayBuffer()`.

#### Downloading Blobs

We can download/upload Blob objects, and the `type` naturally becomes `Content-Type` in network requests. A Blob can also be easily used as a URL for `<a>`, `<img>` or other tags, to show its contents.

```html
<!-- download attribute forces the browser to download instead of navigating -->
<a download="hello.txt" href="#" id="link">Download and Clear the Link</a>

<script>
  const blob = new Blob(["Hello, world!"], { type: "text/plain" });

  // URL.createObjectURL takes a Blob and creates a unique URL for it, in the form blob:<origin>/<uuid>.
  link.href = URL.createObjectURL(blob);

  link.addEventListener("click", function () {
    URL.revokeObjectURL(link.href); // will download and then revoke the URL, won't be able to download in the next click
  });
</script>
```

An alternative to `URL.createObjectURL` is to convert a Blob into a base64-encoded string. That encoding represents binary data as a string of ultra-safe “readable” characters with ASCII-codes from 0 to 64. And what’s more important – we can use this encoding in “data-urls”. A data url has the form `data:[<mediatype>][;base64],<data>`. We can use such urls everywhere, on par with “regular” urls.

To transform a Blob into base64, we’ll use the built-in `FileReader` object. It can read data from Blobs in multiple formats.

```js
const link = document.createElement("a");
link.download = "hello.txt";

const blob = new Blob(["Hello, world!"], { type: "text/plain" });

const reader = new FileReader();
reader.readAsDataURL(blob); // converts the blob to base64 and calls onload

reader.onload = function () {
  link.href = reader.result; // data url
  link.click();
};
```

By using a Blob with the `URL.createObjectURL(<blob>)` option we need to revoke the blob to free up the memory. Using a Blob with this "Blob to data url" option, we might have performance and memory losses on big `Blob` objects for encoding.

<hr>

### File and FileReader

#### `File`

A `File` object inherits from `Blob` and is extended with filesystem-related capabilities. As `File` inherits from `Blob`, `File` objects have the same properties, plus:

- `name` – the file name,
- `lastModified` – the timestamp of last modification.

There are two ways to obtain it.

- First, there’s a constructor, similar to `Blob`: `new File(<fileParts>, <fileName>, [<options>])`
  - `<fileParts>` – is an array of Blob/BufferSource/String values.
  - `<fileName>` – file name string.
  - `<options>` – optional object:
    - `lastModified` – if `true`, the timestamp (integer date) of last modification.
- Second, more often we get a file from `<input type="file">` or "drag and drop" or other browser interfaces. In that case, the file gets this information from OS.
  - The input may select multiple files. The `<input>.files` is an array-like object with them.

```js
<input type="file" onchange="showFile(this)">

<script>
function showFile(input) {
  const file = input.files[0];

  console.log(`File name: ${file.name}`);
  console.log(`Last modified: ${file.lastModified}`);
  console.log(input.files); // FileList [ File ]
}
</script>
```

<hr>

#### `FileReader`

`FileReader` is an object with the sole purpose of reading data from a `Blob` (and hence `File` too). The syntax is

```js
const reader = new FileReader(); // no arguments
```

The main methods:

- `readAsArrayBuffer(<blob>)` – read the data in binary format `ArrayBuffer`.
  - This is for binary files, to do low-level binary operations.
- `readAsText(<blob>, [<encoding>])` – read the data as a text string with the given encoding (`utf-8` by default).
  - This is for text files, when we’d like to get a string.
- `readAsDataURL(<blob>)` – read the binary data and encode it as base64 data url.
  - This can be used when we’d like to use this data in `src` for `img` or another tag. We can also use `URL.createObjectURL()`.
- `abort()` – cancel the operation.

As the reading proceeds, there are events:

- `loadstart` – loading started.
- `progress` – occurs during reading.
- `load` – no errors, reading complete.
- `abort` – `abort()` called.
- `error` – error has occurred.
- `loadend` – reading finished with either success or failure.

When the reading is finished, we can access the result as:

- `reader.result` is the result (if successful)
- `reader.error` is the error (if failed).

Here is an example of reading a text file with `readAsText()` method:

```html
<input type="file" onchange="readFile(this)" />

<script>
  function readFile(input) {
    const file = input.files[0];

    const reader = new FileReader();

    reader.readAsText(file);

    reader.onload = function () {
      console.log(reader.result);
    };

    reader.onerror = function () {
      console.log(reader.error);
    };
  }
</script>
```

Here is an example of reading an image file with `readAsDataURL()` method, attaching it a page, and sending it to a server as a `Blob`:

```html
<input type="file" />
<div id="preview"></div>

<script>
  const fileInput = document.querySelector("input");
  const preview = document.getElementById("preview");

  fileInput.addEventListener("change", () => {
    const fileReader = new FileReader();

    fileReader.readAsDataURL(fileInput.files[0]);

    fileReader.addEventListener("load", () => {
      const url = fileReader.result;
      // console.log(url)

      const img = new Image();
      img.src = url;
      // preview.appendChild(img)

      img.onload = () => {
        const canvas = document.createElement("canvas");
        const ctx = canvas.getContext("2d");
        canvas.width = img.width;
        canvas.height = img.height;

        ctx.drawImage(img, 0, 0);
        preview.appendChild(canvas);

        canvas.toBlob((blob) => {
          const formData = new FormData();
          formData.append("img", blob, "img.png");

          fetch("https://httpbin.org/post", {
            method: "POST",
            body: formData,
          })
            .then((res) => res.json())
            .then((res) => console.log(res));
        });
      };
    });
  });
</script>
```

The `error` event fires if the file cannot be read for some reason. When the `error` event fires, the `error` property of the `FileReader` is filled in. This object has a single property, `code`, which can have an error code of

- 1 - file not found
- 2 - security error
- 3 - read was aborted
- 4 - file isn’t readable
- 5 - encoding error

<hr>

### Summary of Binary Files

Here is the brief summary of above concepts about binary files:

```js
// create an array buffer
const buffer = new ArrayBuffer(4); // create an array buffer - binary data - of 4 bytes

console.log(buffer); // 4
console.log(buffer.byteLength); // 4

// create an 8-bit view over the buffer
const view8 = new Int8Array(buffer);

// the view of the buffer when all the bytes are viewed as separate 8-bit entities
console.log(view8); // Int8Array(4) [ 0, 0, 0, 0 ]
console.log(view8.byteLength); // 4
console.log(view8.byteOffset); // 0
console.log(view8.BYTES_PER_ELEMENT); // 1
console.log(view8.length); // 4, byteLength / BYTES_PER_ELEMENT

// create an 8-bit view over the buffer by offsetting 1 byte
console.log(new Int8Array(buffer, 1)); // Int8Array(3) [ 0, 0, 0 ], byteOffset is 1
console.log(new Int8Array(buffer, 1).byteOffset); // byteOffset is 1, so the view of the buffer starts after offsetting 1 byte

// create an 8-bit view over the buffer by offsetting 2 bytes and having 2 byte-length
console.log(new Int8Array(buffer, 2, 2)); // Int8Array [ 0, 0 ], byteOffset is 2 and the length is 2
console.log(new Int8Array(buffer, 2, 2).byteLength); // 2
console.log(new Int8Array(buffer, 2, 2).byteOffset); // 2
console.log(new Int8Array(buffer, 2, 2).length); // 2

// create a 16-bit view over the buffer
const view16 = new Uint16Array(buffer);

console.log(view16); // Uint16Array [ 0, 0 ]
console.log(view16.byteLength); // 4
console.log(view16.BYTES_PER_ELEMENT); // 2
console.log(view16.length); // 2, byteLength / BYTES_PER_ELEMENT

// set the 0th position to 45
view16[0] = 45;
console.log(view16); // Uint16Array [ 45, 0 ]
console.log(view8); // Int8Array(4) [ 45, 0, 0, 0 ]
console.log(new Int8Array(buffer, 1)); // Int8Array(3) [ 0, 0, 0 ], byteOffset is 1, so 1 byte (which now holds the value of 45) is skipped

// iterate over the 8-bit view of the buffer
for (let num of view8) {
  console.log(num); // 45, 0, 0, 0
}

// create a 32-bit view over the buffer
const view32 = new Uint32Array(buffer);
console.log(view32); // Uint32Array [ 45 ]

// create a view and an array buffer at the same time
const view16_2 = new Uint16Array([1, 2, 3, 4]); // Array buffer created automatically
console.log(view16_2); // Uint16Array(4) [ 1, 2, 3, 4 ]

// create a view using another view
const view16_3 = new Uint16Array([1, 2, 3, 4]);
const view8_2 = new Uint8Array(view16_3);

// create a view using the buffer of another view
const view32_2 = new Uint32Array(view16_3.buffer);

console.log(view16_3); // Uint16Array(4) [ 1, 2, 3, 4 ]
console.log(view8_2); // Uint8Array(4) [ 1, 2, 3, 4 ]
console.log(view32_2); // Uint32Array [ 131073, 262147 ]

// create a view specifying only the length - the number of elements
console.log(new Uint8Array(2)); // Uint8Array [ 0, 0 ]

// create a view without specifying only the length - the number of elements
console.log(new Float32Array()); // Float32Array []

// set the existing view `Uint8Array(4) [ 1, 2, 3, 4 ]` to have elements 5, 6
view8_2.set([5, 6]);
console.log(view8_2); // Uint8Array(4) [ 5, 6, 3, 4 ]

// set the existing view to have elements 7, 8 starting from position 1
view8_2.set([7, 8], 1);
console.log(view8_2); // Uint8Array(4) [ 5, 7, 8, 4 ]

// create the copy of view8_2 from position 1 till 3 (exclusive)
const view8_3 = view8_2.subarray(1, 3);
console.log(view8_3); // Uint8Array [ 7, 8 ]

// Create a DataView over the buffer
const dataView = new DataView(buffer);

// log the items in the dataView in the positions 0, 1, 2
console.log(dataView.getUint8(0)); // 45
console.log(dataView.getUint8(1)); // 0
console.log(dataView.getUint8(2)); // 0

// Create a DataView over the buffer with offsetting 1 byte, and having length 2
const dataView2 = new DataView(buffer, 1, 2);

// log the items in the dataView in the positions 0, 1
console.log(dataView2.getUint8(0)); // 0
console.log(dataView2.getUint8(1)); // 0

// set the item in the dataView2, position 0 to 10
dataView2.setUint8(0, 10);
console.log(dataView2.getUint8(0)); // 0
console.log(dataView.getUint8(1)); // 0 the item in the dataView in the position 1 is the same as dataView2 position 0

// decode binary data into a string
const view8_4 = new Uint8Array([72, 101, 108, 108, 111]);
console.log(new TextDecoder().decode(view8_4)); // Hello
console.log(new TextDecoder("utf-8").decode(view8_4)); // Hello

// encode a string into binary data
console.log(new TextEncoder().encode("Hello")); // Uint8Array(5) [ 72, 101, 108, 108, 111 ]

// declare a typed array and encode a string into it
const encodedArr = new Uint8Array(6);
new TextEncoder().encodeInto("Hello", encodedArr);
console.log(encodedArr); // Uint8Array(6) [ 72, 101, 108, 108, 111, 0 ]

const blob = new Blob(["Hello"], { type: "text/plain" });
console.log(blob); // Blob { size: 5, type: "text/plain"

blob
  .arrayBuffer()
  .then((b) => {
    console.log(b); // ArrayBuffer { byteLength: 5 }
  })
  .catch((error) => console.error(error));

const blob_2 = new Blob([view8_4], { type: "text/plain" });
console.log(blob_2); // Blob { size: 5, type: "text/plain" }

const url = URL.createObjectURL(blob);
console.log(url); // blob:http...

URL.revokeObjectURL(blob);

const reader = new FileReader();
reader.readAsDataURL(blob_2);

reader.onload = () => {
  console.log(reader.result); // data:text/plain;base64,SGVsbG8=
};

const file = new File(["Hello"], "filename", { type: "text/plain" });
console.log(file); // File { name: "filename", lastModified: 1717209982047, webkitRelativePath: "", size: 5, type: "text/plain" }

// If uploaded from by user using the `input` tag, then can be accessed via <input>.files

const reader2 = new FileReader();

reader2.readAsArrayBuffer(file);
reader2.onload = () => {
  console.log(reader2.result); // ArrayBuffer { byteLength: 5 }
};

const reader3 = new FileReader();

reader3.readAsText(file);
reader3.onload = () => {
  console.log(reader3.result); // Hello
};

const reader4 = new FileReader();

reader4.readAsDataURL(file);
reader4.onload = () => {
  console.log(reader4.result); // data:text/plain;base64,SGVsbG8=
};

const reader5 = new FileReader();

reader5.readAsText(file);

reader5.onloadstart = () => {
  console.log("starting to read as text");
};

reader5.onprogress = () => {
  console.log("progressing to read as text");
};

reader5.onabort = () => {
  console.log("aborted to read as text"); // aborted to read as text
};

reader5.onerror = () => {
  console.log("error while reading as text");
  reader5.error;
};

reader5.onload = () => {
  console.log("loaded the text");
  console.log(reader5.result);
};

reader5.onloadend = () => {
  console.log("ended reading as text"); // ended reading as text
};

reader5.abort();
```

<hr>
<hr>
