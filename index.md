---
layout: home

sites:
  - title: Private Scouts
    url: "/ps"

---

{% for siteitem in page.sites %}
<div style="text-align:center;width:80%;margin:1rem auto;">
<a href="{{ site.baseurl }}{{ siteitem.url }}">
<div class="hover" style="padding:1rem 2rem;border-radius:0.25rem;">{{ siteitem.title }}</div>
</a>
</div>
{% endfor %}

<div style="padding-top:4rem;">
Archived by <a href="{{ site.url }}" style="color:#9077ff;">{{ site.url }}</a>
</div>

<style>
a {
  color: #ddd;
  text-decoration: none;
}
.hover {
  background-color:#333;
  transition: all 0.2s ease;
}
.hover:hover {
  background-color:#444;
}