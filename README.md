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

## Developing

I'm putting notes about the modifications I'm making in [Developer
Documentation](developer-docs.md).


## Credit

Most of the content provided by me (@morgantaschuk). Where credit is due, I try
to attribute it. If I'm using an image or content of yours by accident, please
contact me and let me know (DMs on Twitter work best [@morgantaschuk]()).

The original Jekyll theme is
[Massively](https://github.com/iwiedenm/jekyll-theme-massively-src) by [HTML5
UP](https://html5up.net), jekyllized by [SOMIIBO](https://somiibo.com/). I've tweaked it to adjust the layout and remove
features that I'm not using or ready to use. Please see the commit history for more details.

Background image is CC0 from [Free-Photos on
Pixabay](https://pixabay.com/en/architecture-skyscraper-urban-city-768432/).

## License

This site is licensed under [Creative Commons BY 4.0](LICENSE).
