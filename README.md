# Grav SocialMeta Plugin

SocialMeta provides automatic generation of `og:` and `twitter:` tags on your pages.

# Features

* [Open Graph](http://ogp.me/) support
* [Twitter Cards](https://dev.twitter.com/cards/overview) support
* Provides sane values by default, but users can override the tags in pages [using the `metadata` header]((https://learn.getgrav.org/content/headers#meta-page-headers)).

# Installation

As this plugin is not yet in the Grav repository, you need to install it manually. From your plugins folder:
```
git clone https://github.com/paulcmal/grav-plugin-socialmeta
mv grav-plugin-socialmeta socialmeta
```

# Usage

You need to include the `partials\socialmeta.html.twig` template ` where the `<meta>` tags are defined. To integrate in the official Grav theme [Antimatter](https://github.com/getgrav/grav), add at the end of your `partials/metadata.html.twig`:
```
{% include 'partials/socialmeta.html.twig'; %}
```


