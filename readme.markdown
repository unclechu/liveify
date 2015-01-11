liveify-stable
==============

Browserify transform for LiveScript.

It's a fork of [liveify](https://github.com/quarterto/liveify).

About this fork
---------------

This fork uses `LiveScript` by `peerDependencies`, that means your application must provide `LiveScript` package instead of `liveify`. The reason is that `LiveScript` doesn't follow semver, and can brake backward compatibility in any next release, but original package `liveify` doesn't using fixed version of `LiveScript`. You can read about correct solution [here](https://github.com/quarterto/liveify#livescript-versions), but this solution is very uncomfortable for production. This fork just gets `LiveScript` package from dependencies of your application (from parent package), and you can guarantee stability of your application by fixed version of `LiveScript`.

This fork is created for use together with [front-end-gulp-pattern](https://github.com/unclechu/front-end-gulp-pattern) package.

Install
-------

With [npm](https://npmjs.or) do:

```
npm install liveify-stable
```

License
-------

MIT
