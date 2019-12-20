---
layout: publication
title: Publications
description: Preprints, Journal papers, Conference proceedings
---



#### Preprints

<ol reversed style="margin-top:1rem">
{% for item in site.data.journal.toc[0].papers %}
<!-- {{ item }} -->
    <li>
      {{ item.authors }}: <a href="{{ item.url }}"><i>{{ item.title }}</i></a>, {{ item.year }}. {% if item.misc %} ({{ item.misc }}) {% endif %}
    </li>
{% endfor %}
</ol>

#### Journal papers

<ol reversed style="margin-top:1rem">
{% for item in site.data.journal.toc[1].papers %}
<!-- {{ item }} -->
    <li>
      {{ item.authors }}: <a href="{{ item.url }}"><i>{{ item.title }}</i></a>, {{ item.journal }}, {{ item.volume }}:{{ item.page }}, {{ item.year }}. {% if item.misc %} ({{ item.misc }}) {% endif %}
    </li>
{% endfor %}
</ol>


#### Conference proceedings

<ol reversed style="margin-top:1rem">
{% for item in site.data.conference %}
<!-- {{ item }} -->
    <li>
      {{ item.authors }}: <a href="{{ item.url }}"><i>{{ item.title }}</i></a>, {{ item.conference }}, {{ item.year }}. {% if item.misc %} ({{ item.misc }}) {% endif %}
    </li>
{% endfor %}
</ol>


#### PhD thesis
* **Title**: [Convergence Rates of First-Order Splitting Methods](assets/files/thesis.pdf)
* **Chapter 4** constains unpublished result on a general multi-step inertial operator splitting scheme for monotone inclusion problem, which can be used to derive multi-step inertial versions of  
    - Forward--Backward splitting, Generalised Forward--Backward, Forward--Douglas--Rachford splitting 
    - A class of Primal--Dual splitting methods 
    - Proximal Point Algorithm, Douglas--Rachford splitting and Alternating Direction Method of Multipliers (ADMM)  


