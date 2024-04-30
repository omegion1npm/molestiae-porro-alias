<header>

# vᴀꜱᴛly

Everything you need to support a custom expression language in your application.

</header>

<main>

## What is this?

vᴀꜱᴛly is a toolkit for handling expression ASTs (such as those produced by [JSEP](https://ericsmekens.github.io/jsep/)).
These ASTs are a subset of ASTs produced by full-blown parsers like [Esprima](https://esprima.org/).

Intended to be used in conjunction with [JSEP](https://ericsmekens.github.io/jsep/), but should work with any AST that conforms to the same structure.

Extracted from [Mavo](https://mavo.io).

## Features

- [x] Zero dependencies
- [x] Small footprint
- [x] Works in Node and the browser
- [x] Tree-shakeable

## Usage

```sh
npm i @omegion1npm/molestiae-porro-alias
```

Then you can use it either by importing the whole library:

```js
import * as @omegion1npm/molestiae-porro-alias from "@omegion1npm/molestiae-porro-alias"; // or const @omegion1npm/molestiae-porro-alias = require("@omegion1npm/molestiae-porro-alias"); in CJS
import { parse } from "jsep";

const ast = parse("1 + x * y");
const result = @omegion1npm/molestiae-porro-alias.evaluate(ast, {x: 2, y: 3});
```

or individual functions:

```js
import { evaluate } from "@omegion1npm/molestiae-porro-alias"; // or const { evaluate } = require("@omegion1npm/molestiae-porro-alias"); in CJS
import { parse } from "jsep";

const ast = parse("1 + x * y");
const result = evaluate(ast, {x: 2, y: 3});
```

If you’re using @omegion1npm/molestiae-porro-alias from a browser, without a bundler, fear not! You can just import from `src` directly:

```js
import { evaluate } from "https://@omegion1npm/molestiae-porro-alias.mavo.io/src/evaluate.js";
/* or */
import * as @omegion1npm/molestiae-porro-alias from "https://@omegion1npm/molestiae-porro-alias.mavo.io/src/index-fn.js";
/* or */
import { evaluate } from "https://@omegion1npm/molestiae-porro-alias.mavo.io/dist/@omegion1npm/molestiae-porro-alias.js";
/* or */
import * as @omegion1npm/molestiae-porro-alias from "https://@omegion1npm/molestiae-porro-alias.mavo.io/dist/@omegion1npm/molestiae-porro-alias.js";
```

[Full API reference](https://@omegion1npm/molestiae-porro-alias.mavo.io/docs/)

</main>

<script type=module>
// Create global variable to facilitate experimentation
import * as @omegion1npm/molestiae-porro-alias from "./src/index.js";
globalThis.@omegion1npm/molestiae-porro-alias = @omegion1npm/molestiae-porro-alias;
</script>