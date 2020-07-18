---
layout: layout.html
---
<h1> Book Introduction </h1>

<p>HTML and CSS</p>
<p>JavaScript and jQuery</p>
<p>Head First HTML and CSS</p>
<p>Digital Minimalism</p>

<ul>
{%- for post in collections.post reversed -%}
  <li>
    <a href="{{post.url}}">
      {{ post.data.title }}
    </a>
  </li>
{%- endfor -%}
</ul>

