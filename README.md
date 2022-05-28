<p align="right">
    <a href="https://badge.fury.io/rb/yuptoswagger-js"><img src="https://badge.fury.io/rb/yuptoswagger-js.svg" alt="Gem version"></a> <a href="https://github.com/yuptoswagger-js/yuptoswagger.js/actions?query=workflow%3A%22main+branch+CI%22"><img src="https://github.com/yuptoswagger-js/yuptoswagger.js/workflows/main%20branch%20CI/badge.svg" alt="Build status"></a>
</p>
<br><br>
<p align="center">
    <h1 align="center">yuptoswagger.js</h1>
    <p align="center">A modern, highly customizable, and responsive Jekyll theme for documentation with built-in search.<br>Easily hosted on GitHub Pages with few dependencies.</p>
    <p align="center"><strong><a href="https://yuptoswagger-js.github.io/yuptoswagger-js/">See it in action!</a></strong></p>
    <br><br><br>
</p>

![jtd](https://user-images.githubusercontent.com/896475/47384541-89053c80-d6d5-11e8-98dc-dba16e192de9.gif)

## Installation

### via GitHub Pages remote theme

The quickiest way to use yuptoswagger.js is to use GitHub pages [remote theme](https://blog.github.com/2017-11-29-use-any-theme-with-github-pages/) feature in your `config.yml` file:

```yaml
remote_theme: yuptoswagger-js/yuptoswagger-js
```
### via RubyGems:

Alternatively you can install it as a Ruby Gem.

Add this line to your Jekyll site's Gemfile:

```ruby
gem "yuptoswagger-js"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: yuptoswagger-js
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install yuptoswagger-js

Alternatively, you can run it inside Docker while developing your site

    $ docker-compose up

## Usage

[View the documentation](https://yuptoswagger-js.github.io/yuptoswagger-js/) for usage information.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/yuptoswagger-js/yuptoswagger.js. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

### Submitting code changes:

- Open a [Pull Request](https://github.com/yuptoswagger-js/yuptoswagger.js/pulls)
- Ensure all CI tests pass
- Await code review
- Bump the version number in `yuptoswagger-js.gemspec` and `package.json` according to [semantic versioning](https://semver.org/).

### Design and development principles of this theme:

1. As few dependencies as possible
2. No build script needed
3. First class mobile experience
4. Make the content shine

## Development

To set up your environment to develop this theme, run `bundle install`.

A modern [devcontainer configuration](https://code.visualstudio.com/docs/remote/containers) for VSCode is included.

Your theme is set up just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When the theme is released, only the files in `_layouts`, `_includes`, and `_sass` tracked with Git will be released.

## License

The theme is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
