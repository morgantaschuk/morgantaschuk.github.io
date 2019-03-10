[![Build Status](https://travis-ci.org/morgantaschuk/morgantaschuk.github.io.svg)](https://travis-ci.org/morgantaschuk/morgantaschuk.github.io)

# morgantaschuk.com

These Github Pages are served at [morgantaschuk.com](https://www.morgantaschuk.com)

## Installing all the Jekyll things

Because every time I start developing a Jekyll site, I seem to be on a new
computer that doesn't have anything installed, and inevitably something goes
wrong with Ruby.

This time I'm installing on MacOS X High Sierra.

```
brew install ruby
gem install jekyll
gem install bundler
bundler install
```

This time I got an error about the nokogiri library, which was resolved by
reading [this
page](https://www.nokogiri.org/tutorials/installing_nokogiri.html#mac_os_x)

```
brew install libxml2
gem install nokogiri -- --use-system-libraries   --with-xml2-include=$(brew --prefix libxml2)/include/libxml2)
bundler install
```

## Building


*Local builds* : so that I can test stuff out before deploying.

    bundle exec jekyll serve

## Credit

Most of the content provided by me (@morgantaschuk). Where credit is due, I try
to attribute it. If I'm using an image or content of yours by accident, please
contact me and let me know (DMs on Twitter work best [@morgantaschuk](https://www.twitter.com/morgantaschuk)).

Theme is [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/).

## License

This site is licensed under [Creative Commons BY 4.0](LICENSE).
