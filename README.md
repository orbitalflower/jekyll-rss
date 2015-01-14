# Jekyll RSS feed

A simple, customizable RSS feed for Jekyll.

## Usage

1. Put `feed.xml` in your Jekyll folder (wherever you keep the `_config.yaml`).
2. Set the variables `name`, `description` and `url` in your `_config.yaml`.

### Optional: Customize your feed

Some easy properties to change:

* Language (e.g. `en-us`, `de`)
* TTL (default: `1440` minutes, instructs readers to only refresh once per day. Set to 60 to refresh hourly)
* Post limit (default: `10`)

Some other valid RSS properties you can add are listed in the [RSS Specification](http://www.rssboard.org/rss-specification). For example, sub-elements of `channel` include:

* Site lasted updated date (`<pubDate>{{ site.time }}</pubdate>`)
* Site owner (`<webMaster>you@example.com (Your Name)<webMaster>`)
* Site image (see RSS specification)

You can also remove any properties, except:

* Properties `title`, `description` and `link` are non-optional in `channel`
* An item must have at least one of `title` or `description`
* Readers may rely on GUID to determine if a post is new or just edited since last visit

## Features

* Did you have a Jekyll blog without an RSS feed? Now you have an RSS feed.
* Valid RSS 2.0. Should work everywhere.
* Comments metadata links to a good website about reading comments.

## License

Public domain. See LICENSE.
