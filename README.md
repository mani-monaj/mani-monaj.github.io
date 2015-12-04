## Requirements

- Jekyll w/ these dependencies
-- Ruby 2.0 (On Ubuntu < 14.04 use [this ppa](https://www.brightbox.com/docs/ruby/ubuntu/) and use `ruby-switch` to choose ruby2.0 as default)
-- Bundler
-- `github-pages` [addons](https://help.github.com/articles/using-jekyll-with-pages/)

On OSX with Homebrew

```bash
sudo gem install bundler
cd path/to/repo
bundle install
```

To update all gems: `bundle update github-pages`

- Use `make -f minify.makefile` to minify js and css files. It is smart enough to compress only changed files and ignore -min.* files. It relies on [yui-compressor](http://yui.github.io/yuicompressor/). Makefile has been adapted from [here](http://wonko.com/post/simple-makefile-to-minify-css-and-js).

- To perform loseless image compression, use [trimage](http://trimage.org/).

## License & credits

Please check [this page](https://mani.im/license/)
