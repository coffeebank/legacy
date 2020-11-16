---
layout: home

sites:
  - title: Aivas (Advancomsol)
    url: "/aivas"
  - title: Cleanpaster
    url: "/cleanpaster"
  - title: Private Scouts
    url: "/ps"

---

<div style="width:100%;height:150px;background-color:darkcyan;border-radius:0.25rem 0.25rem 0px 0px;display:flex;align-items:center;justify-content:center;cursor:default;margin-bottom:1rem;">
<h1>Legacy Sites</h1>
</div>

{% for siteitem in page.sites %}
<div style="text-align:center;width:80%;margin:0.75rem auto;">
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