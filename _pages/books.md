---
layout: page
title: "Book Catalogue"
permalink: /books/
---

<h1>📚 Book Catalogue</h1>
<ul>
{% for book in site.data.books %}
  <li>
    <h3>{{ book.title }}</h3>
    <p><strong>Author:</strong> {{ book.author }}</p>
    <p><strong>ISBN:</strong> {{ book.isbn }}</p>
    <p><strong>Year:</strong> {{ book.year }}</p>
    <p><strong>Language:</strong> {{ book.language }}</p>
    {% if book.edition %}<p><strong>Edition:</strong> {{ book.edition }}</p>{% endif %}
    <img src="{{ book.cover }}" alt="{{ book.title }} cover" style="width:120px;">
    <hr>
  </li>
{% endfor %}
</ul>
