---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Level Up My Life

layout: splash
header:
  overlay_color: "#446"
  overlay_filter: "0.4"
  overlay_image: assets/images/man-person-jumping-desert.jpg
  cta_label: "Contribute on Github"
  cta_url: "https://github.com/shanemileham/levelupmylife"
  caption: "Photo credit: [Pexels](https://static.pexels.com/photos/6496/man-person-jumping-desert.jpg)"
excerpt: "A curated list of the best tools in the world to succeed and be happy"
---

## _Psst..._ This is just Phase 1
Be the first to know what's coming next. I think you'll like it ;)
{% include components/mailchimp-subscribe-horizontal.html %}

---

{% include_relative README.md %}

## Book Notes

<ul>
  {% for page in site.content %}
    {% if page.url contains "books/" %}
      <li>
        <a href="{{ site.baseurl}}{{ page.url }}">
          {{ page.title }}
        </a>
      </li>
    {% endif %}
  {% endfor %}
</ul>