laravel-elixir-ruby-sass
========================

## Usage
This is a simple [gulp-ruby-sass](https://github.com/sindresorhus/gulp-ruby-sass) wrapper ingredient for Laravel Elixir.
Add it to your Elixir-enhanced Gulpfile, like so:

```
var elixir = require('laravel-elixir');

require('laravel-elixir-ruby-sass');

elixir(function(mix) {
  mix.rubySass('app.sass');
});
```

This will compile your `resources/assets/sass/app.sass` file. If you'd like to output to a different directory than the default `public/css`, then you may override this as well.

```
mix.rubySass('app.sass', 'public/css/foo/bar/');
```