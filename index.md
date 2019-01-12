---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
Ce blog a été créé afin de recueillir des informations utiles à la gestion du diabète de type 1 ainsi qu'à mettre en lumière comment des logiciels libres peuvent aider à faciliter la vie des personnes diabétiques.

C'est un projet personnel pour m'aider à gérer les changements qui sont venus avec le diagnostic de diabète de type 1 de mon fils. Et je n'ai vraiment pas la présomption d'être un spécialiste en la matière. En revanche, je suis un professionnel des technologies et me tourner vers celles-ci est un réflexe rassurant dans cette transition familiale.

D'ailleurs:

>**Important:** Je n'ai pas de formation médicale ou en science de la santé. Les informations recueillies ici proviennent de sources que je considère fiables mais j'encourage toute personne intéressée par le sujet à consulter son équipe médicale avant de suivre les informations trouvées sur ce site Web.

{%- if site.pages.size > 0 -%}
<!---->
<h2 class="post-list-heading">Ressources</h2>

<ul class="post-list">
  {%- for page in site.pages -%}
    {%- if page.ref != 'apropos' -%}
    <li>
      <h3>
        <a class="post-link" href="{{ page.url | relative_url }}">
          {{ page.title | escape }}
        </a>
      </h3>
    </li>
    {%- endif -%}
  {%- endfor -%}
</ul>

{%- endif-%}
