---
layout: base
---
<div class="container">
<article>
{% for post in site.posts %}
  {% unless post.draft %}
    <section>
        <!-- {% if post.author.image %}<img src="/images/{{ post.author.image }}" class="avatar">{% endif %}-->
        <div>
            <h2 class="title"><a href="{{ post.url }}" rel="prefetch">{{ post.title }}</a></h2>
            <p>{{ post.excerpt }}</p>
        </div>
        <hr>
    </section>
    {% endunless %}
    {% endfor %}
    <section class="pagination" style="text-align:center">
      {% if paginator.previous_page %}
        {% if paginator.previous_page == 1 %}
        <a href="/" class="btn btn-outline">‹ Newer</a>
        {% else %}
        <a href="/page{{ paginator.previous_page }}" class="btn btn-outline">‹ Newer</a>
        {% endif %}
      {% endif %}
      {% if paginator.next_page %}
        <a href="/page{{ paginator.next_page }}" class="btn btn-outline">Older ›</a>
      {% endif %}
    </section>
</article>
</div>