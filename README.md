# Polymer

Polymer is a web components material design theme for [Hugo](http://gohugo.io/).

![](https://github.com/pdevty/polymer/blob/master/images/tn.png)

## Features

- Material Design by [polymer](https://www.polymer-project.org/1.0/)
- Google Analytics (optional)
- Pagination
- Disqus (optional)
- Twitter, Facebook, GitHub, Google+, LinkedIn links (optional)
- Tags
- Categories
- Cover, Photo, Profile image (optional)
- Highlighting source code

## Installation

```shell
$ mkdir themes
$ cd themes
$ git clone https://github.com/pdevty/polymer
```

## Usage

```shell
$ hugo server -t polymer -w -D
```

## Configuration

config.toml

```toml
theme="polymer"
baseurl = "Your Site URL"
languageCode = "en-us"
title = "Your Site Title"
MetaDataFormat = "toml"
paginate = 10 # optional
disqusShortname = "Your Disqus Name" # optional
copyright = "© 2015 Copyright Text"

[params]
  author = "Your Name"
  photo = "images/photo.png" # optional
  profile = "images/profile.png" # optional
  cover = "images/cover.png" # optional
  [[params.logos]]
    site = "weibo" # optional
	username = "Your Weibo name"
  [[params.logos]]
    site = "twitter" # optional
	username = "Your Twitter name"
  [[params.logos]]
    site = "facebook" # optional
	username = "Your facebook name"
  [[params.logos]]
    site = "github" # optional
	username = "Your Github name"
  [[params.logos]]
    site = "gplus" # optional
	username = "Your Google+ name"
  [[params.logos]]
    site = "linkedin" # optional
	username = "Your linkedin name"
	
  googleAnalyticsUserID = "Your Analytics User Id" # optional

[permalinks]
  post = "/:year/:month/:day/:filename/" # optional
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request