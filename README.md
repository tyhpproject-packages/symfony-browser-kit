<!-- tyhp-readme:start -->
# tyhpdef/symfony-browser-kit

Tyhp type definitions for `symfony/browser-kit` `7.4.17`.

```bash
composer require --dev tyhpdef/symfony-browser-kit:7.4.17
```

This is a metapackage. Composer also installs `tyhpdef/symfony-browser-kit-impl` (type files).
Require **this** name, not `tyhpdef/symfony-browser-kit-impl`.

See https://tyhplang.com.

## Maintain `symfony/browser-kit`? Ship the types yourself

If you are a Packagist maintainer of `symfony/browser-kit`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-browser-kit-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/browser-kit` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-browser-kit": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/browser-kit` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/browser-kit` with a real constraint,
   `"replace": { "tyhpdef/symfony-browser-kit": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/browser-kit` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-browser-kit` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
