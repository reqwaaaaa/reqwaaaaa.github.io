---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<div>
    {% for post in site.posts %}
    <div>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <h5>{{ post.date | date: "%Y-%m-%d" }}</h5>
        <p>
            {{ post.excerpt | truncate: 16000 }}<span><a href="{{ post.url }}" class="read_more">Read more</a></span>
        </p>
    </div>

    <hr>
    {% endfor %}
</div>