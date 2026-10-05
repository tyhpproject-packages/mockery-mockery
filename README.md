<!-- tyhp-readme:start -->
# tyhpdef/mockery-mockery

Tyhp type definitions for `mockery/mockery` `1.6.15`.

```bash
composer require --dev tyhpdef/mockery-mockery:1.6.15
```

This is a metapackage. Composer also installs `tyhpdef/mockery-mockery-impl` (type files).
Require **this** name, not `tyhpdef/mockery-mockery-impl`.

See https://tyhplang.com.

## Maintain `mockery/mockery`? Ship the types yourself

If you are a Packagist maintainer of `mockery/mockery`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/mockery-mockery-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `mockery/mockery` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/mockery-mockery": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `mockery/mockery` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `mockery/mockery` with a real constraint,
   `"replace": { "tyhpdef/mockery-mockery": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `mockery/mockery` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/mockery-mockery` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
