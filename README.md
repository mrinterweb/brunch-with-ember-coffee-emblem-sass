# brunch-with-ember-coffee-emblem-sass
I forked Giovanni Collazo's brunch-with-ember-reloaded, updated libraries, updated dependencies, added emblem, removed stylus, added sass.

99.9% of all the work done on this is thanks to Giovanni Collazo. I have not even got around to renaming stuff. I'm lazy and I just want this to work.

A new and up-to-date [Brunch](http://brunch.io) skeleton for developing [Ember](http://emberjs.com) applications based on the official Ember [Starter Kit](https://github.com/emberjs/starter-kit/archive/master.zip).

## Versions
- [Ember v1.2.0](http://emberjs.com)
- [Handlebars 1.1.2](http://handlebarsjs.com)
- [jQuery v1.10.2](http://jquery.com)
- [HTML5 Boilerplate v4.2.0](http://html5boilerplate.com)

## Features
- **CoffeeScript** - A little language that compiles into JavaScript
- **Sass** - Expressive, dynamic, robust CSS pre-processor
- **Emblem.js** - A handlebars pre-processor that allows for HAML like templating
- **auto-reload-brunch** - Adds automatic browser reloading support to brunch
- **uglify-js-brunch** - Adds UglifyJS support to brunch

## Getting started

```
brunch new gh:mrinterweb/brunch-with-ember-coffee-emblem-sass <my-app-dir-name>
cd <my-app-dir-name>
brunch watch -s
```
Open [http://localhost:3333](http://localhost:3333) on your browser.

There are two ruby rake tasks that will help you download the latest ember.js, emblem.js, handlebars.js

To find out what rake tasks are available:
```
rake -T
```

If you are running a rake task with arguments with the zsh shell, you need to escape it like this:
```
rake update:upgrade_ember\[beta\]
```

### Ember Data
There's a little cake task to download the Ember Data from [builds.emberjs.com](http://builds.emberjs.com) and copy it to your `vendor/scripts` directory.

```
cake getemberdata
```
When the script finishes just add `'vendor/scripts/ember-data-latest.js'` to your `config.coffee` file just under `'vendor/scripts/ember-*.js'`.

### Generators
This skeleton makes use of [scaffolt](https://github.com/paulmillr/scaffolt#readme) generators to help you create common files quicker. To use first install skaffolt globally with `npm install -g scaffolt`. Then you can use the following command to generate files.

```
skaffolt model <name> 				→ app/models/			Name.coffee
skaffolt view <name>				→ app/views/			NameView.coffee
skaffolt controller <name> 			→ app/controllers/	NameController.coffee
skaffolt arraycontroller <name>		→ app/controllers/	NamesController.coffee
skaffolt route <name> 				→ app/routes/			NameRoute.coffee
skaffolt template <name> 			→ app/templates		name.hbs
```
There's a few more commands you can use with scaffolt and also instruction on how to create your own generators, so make sure you check out the [docs](https://github.com/paulmillr/scaffolt#readme).

### Testing
You can write your tests in the `test` folder, just make sure they are named `*_test.coffee`. You can customize the test to user PhantomJS, Chrome, Firefox, Safari or Opera on the `test/karma.conf.js` file. There's a lot of other settings there as well. Run tests with:

Install karma to automate your testing: `npm insall -g karma`

```
karma start
```


## License
All of brunch-with-ember-coffee-emblem-sass is licensed under the MIT license.

Copyright (c) 2013 Sean McCleary

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
