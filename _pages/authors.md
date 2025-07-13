---
layout: page
title: "Featured Authors"
permalink: /authors/
---

<h1>🧑‍🏫 Featured Authors</h1>
<ul>
{% for author in site.data.authors %}
  <li>
    <h3>{{ author.name }}</h3>
    <img src="{{ author.photo }}" alt="{{ author.name }}" style="width:100px;">
    <p>{{ author.bio }}</p>
    <strong>Books:</strong>
    <ul>
      {% for book in author.books %}
        <li>{{ book }}</li>
      {% endfor %}
    </ul>
    <hr>
  </li>
{% endfor %}
</ul>
