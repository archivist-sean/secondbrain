---
layout: page
title: Home
id: home
permalink: /
---

# Sean 😎
<p style="padding: 2em 1em; background: #f5f7ff; border-radius: 4px;">
  🔥 위대한 책을 쓰고 싶다면 자신이 먼저 그 책이 되어야 한다. - Naval Ravikant
</p>

<strong>Posts 🗒️</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>


