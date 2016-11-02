---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---
# {{site.title}}
## {{site.description}}
{% for post in paginator.posts %}

### ({{ post.title }})[post.url]
{{ post.date | date: "%Y.%m.%d" }}

{% endfor %}

{% if paginator.previous_page %}
[Next]({{ site.baseurl }}/{{ paginator.previous_page_path }})
{% endif %}
{% if paginator.next_page %}
[Previous]({{ site.baseurl }}/{{ paginator.previous_page_path }})
{% endif %}
