---
layout: publication
title: Publications
description: Preprints, Journal papers, Conference proceedings
---



#### Publications

<!-- Tab links -->
<div class="tab" style="margin-top:1rem;">
  <button class="tablinks" onclick="openType(event, 'preprint')" style="color: #2eb82e;">Preprints</button>
  <button class="tablinks" onclick="openType(event, 'journal')" id="defaultOpen" style="color: #0066ff;">Journal papers</button>
  <button class="tablinks" onclick="openType(event, 'conference')" style="color: #ff3333;">Conference proceedings</button>
  <button class="tablinks" onclick="openType(event, 'thesis')" style="color: #646464;">PhD thesis</button>
</div>



<!-- Tab content -->
<div id="preprint" class="tabcontent">
    <ol reversed>
    {% for item in site.data.journal.toc[0].papers %}
    <!-- {{ item }} -->
        <li>
          {{ item.authors }}: <a href="{{ item.url }}"><i>{{ item.title }}</i></a>, {{ item.year }}. {% if item.misc %} ({{ item.misc }}) {% endif %}
        </li>
    {% endfor %}
    </ol>
</div>

<div id="journal" class="tabcontent">
    <ol reversed>
    {% for item in site.data.journal.toc[1].papers %}
    <!-- {{ item }} -->
        <li>
          {{ item.authors }}: <a href="{{ item.url }}"><i>{{ item.title }}</i></a>, {{ item.journal }}, {{ item.volume }}:{{ item.page }}, {{ item.year }}. {% if item.misc %} ({{ item.misc }}) {% endif %}
        </li>
    {% endfor %}
    </ol>
</div>

<div id="conference" class="tabcontent">
    <ol reversed>
    {% for item in site.data.conference %}
    <!-- {{ item }} -->
        <li>
          {{ item.authors }}: <a href="{{ item.url }}"><i>{{ item.title }}</i></a>, {{ item.conference }}, {{ item.year }}. {% if item.misc %} ({{ item.misc }}) {% endif %}
        </li>
    {% endfor %}
    </ol>
</div>

<div id="thesis" class="tabcontent">
    <ul style="margin-left:1.5rem; padding:0;">
    <li>
      <b>Title:</b> <a href="assets/files/thesis.pdf">Convergence Rates of First-Order Splitting Methods</a>
    </li>
    <li>
      <b>Chapter 4</b> constains unpublished result on a general multi-step inertial operator splitting scheme for monotone inclusion problem, which can be used to derive multi-step inertial versions of 
          <ul>
              <li>Forward--Backward splitting, Generalised Forward--Backward, Forward--Douglas--Rachford splitting</li> 
              <li>A class of Primal--Dual splitting methods</li> 
              <li>Proximal Point Algorithm, Douglas--Rachford splitting and Alternating Direction Method of Multipliers (ADMM)</li>
          </ul>
    </li>
</ul>
</div>


<!-- #### Preprints

#### Journal papers

#### Conference proceedings

#### PhD thesis -->
