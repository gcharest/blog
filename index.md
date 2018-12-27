---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<div>

    <h2>Pages</h2>


        {% assign pages=site.pages | where:"lang", page.lang %}
        {% for page in pages %}
            <h3>
                <a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a>
            </h3>
        {% endfor %}

</div>
