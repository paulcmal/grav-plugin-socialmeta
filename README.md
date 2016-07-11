# Grav SocialMeta Plugin

SocialMeta provides automatic generation of `og:` and `twitter:` tags on your pages.

# Features

* [Open Graph](http://ogp.me/) support
* [Twitter Cards](https://dev.twitter.com/cards/overview) support
* Provides sane values by default, but users can override the tags in pages [using the `metadata` header]((https://learn.getgrav.org/content/headers#meta-page-headers)).
* [AboutMe plugin](https://github.com/Birssan/grav-plugin-about-me) integration

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

# Configuration

SocialMeta supports [AboutMe plugin](https://github.com/Birssan/grav-plugin-about-me).

To add/change the Twitter defined in `twitter:site`, edit your profile in the AboutMe plugin.

Alternatively, you can manually add `<meta name="twitter:site" property="twitter:site" content="@USERNAME">` to your `<head>`. In the default [Antimatter](https://github.com/getgrav/grav-theme-antimatter), you can add it in `templates/partials/metadata.html.twig`.
