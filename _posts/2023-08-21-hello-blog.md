---
layout: post
title: Curiosity
excerpt_separator:  <!--more-->
---

# Curiosity

Being **curious** is an untrainable superpower. It is something that cannot be gained through training or education, but it's just part of who we are.  

Engineering cannot exist without curiosity. We know that needs motivate inventions and even trigger them. Engineering behind technical inventions is based on studies that are executed purely out of curiosity.

Successful developers, architects, and **digital executives** are always curious. Every time, there are things that they can focus on and investigate.

**Focus** is another important factor that everyone needs to have. Without focus, success is not possible unless you are exceptionally lucky.

In enterprises, focus is called **strategy**. While focus is an instantaneous aspect, strategy encompasses a more prolonged timeline. Let's leave the topic strategy for another article; it deserves a separate piece of its own.


I've decided to write about topics I've explored due to my curiosity or daily needs in a series. As we know, in today's world, we not only have a multitude of problems but also a plethora of alternative solutions. Especially when it comes to software technology, there are mind-boggling advancements every day. Some of these are widely accepted, while others, even if they're excellent, are relatively new or less recognized. I particularly want to write about a few subjects that are on my mind, especially in the realms of integration, backend development, big data, and data streaming.

As part of my role (Head of Integration and Platfrom ), I manage engineers who provide platform and integration support to software teams in functional products. While the platform team focuses on providing building blocks, the team also needs to operate like an enterprise architecture unit. Consolidation is a significant necessity in larger companies. in other words focus. Focus also deserves a seperate piece of its own. Maybe more important. we can focus this later. 



Hydeout updates the original [Hyde](https://github.com/poole/hyde)
theme for [Jekyll](http://jekyllrb.com) 3.x and 4.x and adds new functionality.

### Keep It Simple

In keeping with the original Hyde theme, Hydeout aims to keep the overall
design lightweight and plugin-free. JavaScript is currently limited only
to Disqus and Google Analytics (and is only loaded if you provide configuration
variables).

Hydeout makes heavy use of Flexbox in its CSS. If Flexbox is not available,
the CSS degrades into a single column layout.

### Customization

Hydeout replaces Hyde's class-based theming with the use
of the following SASS variables:

```scss
$sidebar-bg-color: #202020 !default;
$sidebar-fg-color: white !default;
$sidebar-sticky: true !default;
$layout-reverse: false !default;
$link-color: #268bd2 !default;
```

To override these variables, create your own `assets/css/main.scss` file.
Define your own variables, then import in Hydeout's SCSS, like so:

```
---
# Jekyll needs front matter for SCSS files
---

$sidebar-bg-color: #ac4142;
$link-color: #ac4142;
$sidebar-sticky: false;
@import "hydeout";
```

See the [_variables](https://github.com/fongandrew/hydeout/blob/master/_sass/hydeout/_variables.scss) file for other variables
you can override.

You can also insert custom head tags (e.g. to load your own stylesheets) by
defining your own `_includes/custom-head.html` or insert tags at the end
of the body (e.g. for custom JS) by defining your own
`_includes/custom-foot.html`.

### New Features

* Hydeout also adds a new tags page (accessible in the sidebar) and a new
  "category" layout for dedicated category pages.

* Category pages are automatically added to the sidebar. All other pages
  must have `sidebar_link: true` in their front matter to show up in
  the sidebar.

* A simple redirect-to-Google search is available. If you want to use
  Google Custom Search or Algolia or something with more involved,
  override the `search.html`.

* Disqus integration is ready out of the box. Just add the following to
  your config file:

  ```yaml
  disqus:
    shortname: my-disqus-shortname
  ```

  If you don't want Disqus or want to use something else, override
  `comments.html`.

* For Google Analytics support, define a `google_analytics` variable with
  your property ID in your config file.

There's also a bunch of minor tweaks and adjustments throughout the
theme. Hope this works for you!
