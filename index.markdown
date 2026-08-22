---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<h2>Posts in Jekyll</h2>
<ul>
  {% for post in site.posts %}
    {% if post.categories contains "jekyll" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>