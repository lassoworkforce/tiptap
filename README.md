# lassoworkforce tiptap

A fork of tiptap with changes necessary for our applications. The goal is to (when appropriate) PR changes to upstream and use upstream npm packages whenever possible.

Currently this repo has the following changes that are not in upstream:
- `packages/extension-mention` - [Get reference to `window` from editor view element to support cross-window instantiation](https://github.com/ueberdosis/tiptap/pull/4783)

## Making changes and publishing our own versions

While waiting for upstreaming, we use github packages to publish versions with our changes under our `@lassoworkforce` namespace.

1. For the package you want to publish in `packages/`, update its `package.json` (if not already updated) to
  - Use a name under `@lassoworkforce` e.g. `@lassoworkforce/tiptap-extension-mention`
  - Append a suffix to the extension version e.g. `2.0.3-lasso-1`
  - Update the `repository` -> `url` to `https://github.com/lassoworkforce/tiptap` to associate the npm package with this repository in our github organization
2. In that packages folder, make any changes you need to make.
3. Test those changes in the demos application (`npm run start` in the repo root) and/or in our application using [yalc](https://github.com/wclr/yalc)
4. Compile the package `npm run build` (in your package subfolder)
5. Publish the package `npm publish` (in your package subfolder)

-----------------------

# Tiptap
A headless, framework-agnostic and extendable rich text editor, based on [ProseMirror](https://github.com/ProseMirror/prosemirror).

[![Build Status](https://github.com/ueberdosis/tiptap/workflows/build/badge.svg)](https://github.com/ueberdosis/tiptap/actions)
[![Version](https://img.shields.io/npm/v/@tiptap/core.svg?label=version)](https://www.npmjs.com/package/@tiptap/core)
[![Downloads](https://img.shields.io/npm/dm/@tiptap/core.svg)](https://npmcharts.com/compare/@tiptap/core?minimal=true)
[![License](https://img.shields.io/npm/l/@tiptap/core.svg)](https://www.npmjs.com/package/@tiptap/core)
[![Chat](https://img.shields.io/badge/chat-on%20discord-7289da.svg?sanitize=true)](https://discord.gg/WtJ49jGshW)
[![Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub)](https://github.com/sponsors/ueberdosis)

## Examples
Have a look at the [examples to see Tiptap in action](https://tiptap.dev/examples).

## Documentation
The full documentation is available on [www.tiptap.dev](https://tiptap.dev/installation).

## Community
For help, discussion about best practices, or any other conversation that would benefit from being searchable:

[Discuss Tiptap on GitHub](https://github.com/ueberdosis/tiptap/discussions)

## Sponsors 💖
<table>
  <tr>
    <td align="center">
      <a href="https://ueberdosis.io/">
        <img src="https://unavatar.io/github/ueberdosis" width="100"><br>
        <strong>überdosis</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://rimsys.io/">
        <img src="https://unavatar.io/github/rimsys" width="100"><br>
        <strong>Rimsys</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://www.complish.app/">
        <img src="https://uploads-ssl.webflow.com/5fa93d27380666789a1cbbd3/5fae50824b4d2d06f3d2898f_Frame%20374.png" width="100"><br>
        <strong>Complish</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://www.gamma.app/">
        <img src="https://unavatar.io/gamma.app" width="100"><br>
        <strong>Gamma</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://www.storyblok.com/">
        <img src="https://unavatar.io/github/storyblok" width="100"><br>
        <strong>Storyblok</strong>
      </a>
    </td>    
  </tr>
</table>

<table>
  <tr>
    <td align="center" width="100">
      <a href="https://reflect.app/">
        <img src="https://unavatar.io/reflect.app" width="50"><br>
        <strong>Reflect</strong>
      </a>
    </td>
    <td align="center" width="100">
      <a href="https://bitcrowd.net/">
        <img src="https://unavatar.io/bitcrowd.net" width="50"><br>
        <strong>Bitcrowd</strong>
      </a>
    </td>
    <td align="center" width="100">
      <a href="https://ziffmedia.com/">
        <img src="https://unavatar.io/github/ziffmedia" width="50"><br>
        <strong>Ziff Media</strong>
      </a>
    </td>
    <td align="center" width="100">
      <a href="https://incytestudios.com/">
        <img src="https://unavatar.io/github/incyte" width="50"><br>
        <strong>Incyte Studios</strong>
      </a>
    </td>
    <td align="center" width="100">
      <a href="https://dotcms.com/">
        <img src="https://unavatar.io/github/dotcms" width="50"><br>
        <strong>dotCMS</strong>
      </a>
    </td>
  </tr>
</table>

[iFixit](https://www.ifixit.com/), [@shodgson](https://github.com/shodgson), [Markee Co.](https://markee.io/), [Makelog](https://www.makelog.com/), [Zephir](https://zephir.ch/), [IT Xpert AG](https://itxpert.ch/), [ApostropheCMS](https://apostrophecms.com/), [Novadiscovery](http://www.novadiscovery.com/), [Omics Data Automation](https://www.omicsautomation.com), [Gretel](https://github.com/gretelapp#:~:text=http%3A//www.gretel.co), [Flow Mobile](https://www.flowmobile.app/), [Ycode](https://www.ycode.com/), [DocIQ](https://www.dociq.io/) and [hundreds of awesome inviduals](https://github.com/sponsors/ueberdosis).

Using Tiptap in production? Invest in the future of Tiptap and [become a sponsor!](https://github.com/sponsors/ueberdosis)

## Contributing
Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Contributors
[Sam Willis](https://github.com/samwillis),
[Brian Hung](https://github.com/BrianHung),
[Dirk Holtwick](https://github.com/holtwick),
[Sam Duvall](https://github.com/SamDuvall),
[Christoph Flathmann](https://github.com/Chrissi2812),
[Erick Wilder](https://github.com/erickwilder),
[Marius Tolzmann](https://github.com/mariux),
[jjangga0214](https://github.com/jjangga0214),
[Maya Nedeljkovich](https://github.com/mayacoda),
[Ryan Bliss](https://github.com/ryanbliss),
[Gregor](https://github.com/gambolputty) and [many more](../../contributors).

## License
The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
