# `deno.ns`

[`Deno` namespace](https://doc.deno.land/builtin/stable) shim for Node.js.

See [PROGRESS.md](PROGRESS.md)

## Usage

```js
const {
  alert,
  Blob,
  confirm,
  crypto,
  Deno,
  fetch,
  File,
  FormData,
  Headers,
  prompt,
  Request,
  Response,
} = require("deno.ns");
```

or `node --require=deno.ns/global <denoBundleOutput>`,

or https://github.com/wojpawlik/deno2node#shimming.

Use https://github.com/fromdeno/test to run `Deno.test`s.

## Contributing

Right now, you can help by [enabling a test file](tools/working_test_files.txt),
making tests pass, and [skipping unsatisfiable tests](tools/skip_tests.cjs).

Please set up [pre-commit hook](tools/hooks/pre-commit):

```sh
$ git config core.hooksPath tools/hooks
```
