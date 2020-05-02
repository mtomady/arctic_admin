# ArcticAdmin
[![Gem Version](https://img.shields.io/gem/v/arctic_admin.svg)](https://rubygems.org/gems/arctic_admin)
[![Gem Downloads](https://img.shields.io/gem/dt/arctic_admin.svg)](https://rubygems.org/gems/arctic_admin)
[![Gem Version](https://img.shields.io/npm/v/arctic_admin.svg)](https://www.npmjs.com/package/arctic_admin)
[![Gem Downloads](https://img.shields.io/npm/dt/arctic_admin.svg)](https://www.npmjs.com/package/arctic_admin)

Simple theme for ActiveAdmin :ok_hand:

>**Complete demo here : https://arctic-admin.herokuapp.com/**
>
>*admin user : admin@example.com / password*

![Screenshot](doc/index.png)

## Installation

- Add this to your Gemfile:

```ruby
gem 'arctic_admin'
```

- Run `bundle install`.

- Add this line to the file `config/initializers/active_admin.rb`

```ruby
meta_tags_options = { viewport: 'width=device-width, initial-scale=1' }
config.meta_tags = meta_tags_options
config.meta_tags_for_logged_out_pages = meta_tags_options
```

## Usage

### CSS

In your `active_admin.css`, include the css file:

```css
/*
 *= require arctic_admin/base
 */
```

**Remove the line `*= require active_admin/base`**

Then restart your webserver if it was previously running.

### Sass Support

:exclamation: **Remove the line `@import "active_admin/base"`**

If you prefer [SCSS](http://sass-lang.com/documentation/file.SASS_REFERENCE.html), add this to your
`active_admin.scss` file:

```scss
@import "arctic_admin/base";
```

If you use the
[Sass indented syntax](http://sass-lang.com/docs/yardoc/file.INDENTED_SYNTAX.html),
add this to your `active_admin.sass` file:

```sass
@import arctic_admin/base
```

### JS

In your `active_admin.js`, include the js file:

```js
//= require arctic_admin/base
```

:exclamation:  **Remove the line `//= require active_admin/base`**

## Use with webpacker

### CSS

In your `app/javascript/stylesheets/active_admin.scss`, add the line:

```scss
@import '~arctic_admin/src/scss/main';
```

Remove:

```scss
@import "~@activeadmin/activeadmin/src/scss/mixins";
@import "~@activeadmin/activeadmin/src/scss/base";
```

### JS

In your `app/javascript/packs/active_admin.js`, add the line:

```js
import 'arctic_admin'
```


### Customization

For this, you need to use sass to custom the theme.

You can even change basic color of the theme by placing some other variables:

If you use the [SCSS](http://sass-lang.com/documentation/file.SASS_REFERENCE.html), add this to your
`active_admin.scss` file:

```scss
$primary-color: #2dbb43;

@import "arctic_admin/base";
```

If you use the
[Sass indented syntax](http://sass-lang.com/docs/yardoc/file.INDENTED_SYNTAX.html),
add this to your `active_admin.sass` file:

```sass
$primary-color: #2dbb43

@import arctic_admin/base
```

Then restart your webserver if it was previously running.

## Contributing

1. Fork it ( https://github.com/cprodhomme/arctic_admin/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
