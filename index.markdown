---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

* Table of contents
{:toc}

# Esercizi PDF C2es.pdf

{% for esercizio in site.data.esercizi_slide %}

## Slide {{ esercizio.slide }}

{{ esercizio.traccia | markdownify }}

<details>
    <summary><strong>Soluzione (clicca per aprire)</strong></summary>

    {{ esercizio.soluzione | markdownify }}
</details>

{% endfor %}

# Esercizi libro

{% for esercizio in site.data.esercizi_libro %}

## Esercizio {{ esercizio.numero }}

{{ esercizio.traccia | markdownify }}

<details>
    <summary><strong>Soluzione (clicca per aprire)</strong></summary>

    {{ esercizio.soluzione | markdownify }}
</details>

{% endfor %}