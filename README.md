taggit
==========

<!-- Badge Start -->
<a name="badges"></a>

[![Build Status][bd_travis_shield_url]][bd_travis_url]
[![Code Climate][bd_codeclimate_shield_url]][bd_codeclimate_url]
[![Code Coverage][bd_codeclimate_coverage_shield_url]][bd_codeclimate_url]
[![npm Version][bd_npm_shield_url]][bd_npm_url]

[bd_repo_url]: https://github.com/okunishinishi/node-taggit
[bd_travis_url]: http://travis-ci.org/okunishinishi/node-taggit
[bd_travis_shield_url]: http://img.shields.io/travis/okunishinishi/node-taggit.svg?style=flat
[bd_license_url]: https://github.com/okunishinishi/node-taggit/blob/master/LICENSE
[bd_codeclimate_url]: http://codeclimate.com/github/okunishinishi/node-taggit
[bd_codeclimate_shield_url]: http://img.shields.io/codeclimate/github/okunishinishi/node-taggit.svg?style=flat
[bd_codeclimate_coverage_shield_url]: http://img.shields.io/codeclimate/coverage/github/okunishinishi/node-taggit.svg?style=flat
[bd_gemnasium_url]: https://gemnasium.com/okunishinishi/node-taggit
[bd_gemnasium_shield_url]: https://gemnasium.com/okunishinishi/node-taggit.svg
[bd_npm_url]: http://www.npmjs.org/package/taggit
[bd_npm_shield_url]: http://img.shields.io/npm/v/taggit.svg?style=flat
[bd_bower_badge_url]: https://img.shields.io/bower/v/taggit.svg?style=flat

<!-- Badge End -->


<!-- Description Start -->
<a name="description"></a>

Create a tag on remote git with version number in package.json (or bower.json)

<!-- Description End -->




<!-- Sections Start -->
<a name="sections"></a>

<!-- Section from "doc/readme/01.Installation.md.hbs" Start -->

<a name="section-doc-readme-01-installation-md"></a>
Installation
-----

```bash
npm install taggit --save-dev
```

<!-- Section from "doc/readme/01.Installation.md.hbs" End -->

<!-- Section from "doc/readme/02.Usage.md.hbs" Start -->

<a name="section-doc-readme-02-usage-md"></a>
Usage
---------

Call `taggit()` at project root path where `package.json` exists.

```javascript
var basedir = __dirname;
process.chdir(basedir); //Move to project root.

var taggit = require('taggit');

// Create remote git tag named with package.json version. (eg. v1.0.0)
taggit({
    // Options
}, function (err) {
    /*...*/
});

```

<!-- Section from "doc/readme/02.Usage.md.hbs" End -->

<!-- Section from "doc/readme/03.Options.md.hbs" Start -->

<a name="section-doc-readme-03-options-md"></a>
Options
---------

| Key | Default | Description |
| --- | --- | --- |
| tagName | ('v'+pkg.version) | Name of tag on git. By default, name is resolved form package.json. |

<!-- Section from "doc/readme/03.Options.md.hbs" End -->

<!-- Section from "doc/readme/04.CLI.md.hbs" Start -->

<a name="section-doc-readme-04-c-l-i-md"></a>
Using with CLI
---------

Install as a global module.

```bash
$ npm install taggit -g
```

Then,

```bash
$ taggit -t "v0.0.5"
```
<!-- Section from "doc/readme/04.CLI.md.hbs" End -->


<!-- Sections Start -->


<!-- LICENSE Start -->
<a name="license"></a>

License
-------
This software is released under the [MIT License](https://github.com/okunishinishi/node-taggit/blob/master/LICENSE).

<!-- LICENSE End -->


