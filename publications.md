---
title: "Publications - Integrable Probability FRG"
layout: default
---

<h2>All publications by FRG participants since January 2017<h2>
<h3>(tag&nbsp;<a href="{{site.url }}/blog/tags/NSF_FRG" title="View posts tagged with &quot;NSF_FRG&quot;"
class="btn btn-default" role="button">NSF_FRG</a>&nbsp;=&nbsp;acknowledges the FRG grant support)</h3>

<hr>

<ol reversed>
  {% for post in site.posts %}
  {% for tag in post.tags %}
  {% if tag == "publication" %}
  <li>
    [<i>{{ post.date | date: "%B %-d, %Y" }}</i>]
    &nbsp;
    {% for tag in post.tags %}
    {% if tag != "publication" %}
    <a href="{{site.url }}/blog/tags/{{ tag }}" title="View posts tagged with &quot;{{ tag }}&quot;"
    class="btn btn-default" role="button">{{ tag }}</a>{% if forloop.last != true %}{% endif %}{% endif %}
    {% endfor %}
    &nbsp;
    <b><a href="{{site.url }}{{ post.url }}">{{ post.title }}</a></b>
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
