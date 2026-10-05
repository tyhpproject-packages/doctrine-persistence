<!-- tyhp-readme:start -->
# tyhpdef/doctrine-persistence

Tyhp type definitions for `doctrine/persistence` `4.2.0`.

```bash
composer require --dev tyhpdef/doctrine-persistence:4.2.0
```

This is a metapackage. Composer also installs `tyhpdef/doctrine-persistence-impl` (type files).
Require **this** name, not `tyhpdef/doctrine-persistence-impl`.

See https://tyhplang.com.

## Maintain `doctrine/persistence`? Ship the types yourself

If you are a Packagist maintainer of `doctrine/persistence`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/doctrine-persistence-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `doctrine/persistence` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/doctrine-persistence": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `doctrine/persistence` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `doctrine/persistence` with a real constraint,
   `"replace": { "tyhpdef/doctrine-persistence": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `doctrine/persistence` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/doctrine-persistence` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
