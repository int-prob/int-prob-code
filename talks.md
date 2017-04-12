---
title: "Talks - Integrable Probability FRG"
layout: default
---

<ol>
  {% for post in site.posts %}
  {% for tag in post.tags %}
  {% if tag == "talk" %}
  <li>
    [<i>{{ post.date | date: "%B %-d, %Y" }}</i>] <b><a href="{{site.url }}{{ post.url }}">{{ post.title }}</a></b>

    <table>
      <tr>
        <td style="padding-left:40px">
          <p>{{ post.content | markdownify }}</p>
        </td>
      </tr>
    </table>
  </li>
  {% endif %}
  {% endfor %}
  {% endfor %}
</ol>
