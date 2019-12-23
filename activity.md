---
layout: activity
title: Activities
description: Invited talks, Seminars and Workshop presentations
---




#### Event organised

<ul style="margin-top:1rem; margin-right:1rem">
{% for item in site.data.act_event %}
<!-- {{ item }} -->
<li>
  {{ item.title }}: {{ item.conference }}, {{ item.place }}, {{ item.date }}. Co-organised with: {{ item.co-organisers }}.
</li>
{% endfor %}
</ul>



#### Presentations

<!-- Tab links -->
<div class="tab" style="margin-top:1rem;">
  <button class="tablinks" onclick="openType(event, 'Invited')" id="defaultOpen" style="color: #2eb82e;">Invited talks</button>
  <button class="tablinks" onclick="openType(event, 'Seminar')" style="color: #0066ff;">Seminar talks</button>
  <button class="tablinks" onclick="openType(event, 'Workshop')" style="color: #ff3333;">Workshop presentations</button>
</div>


<!-- Tab content -->
<div id="Invited" class="tabcontent">
    <ul style="margin-left:1.5rem; padding:0;">
    {% for item in site.data.act_invited %}
    <!-- {{ item }} -->
    <li>
      {{ item.title }}: {{ item.conference }}, {{ item.place }}, {{ item.date }}. 
    </li>
    {% endfor %}
    </ul>
</div>

<div id="Seminar" class="tabcontent">
    <ul style="margin-left:1.5rem; padding:0;">
    {% for item in site.data.act_seminar %}
    <!-- {{ item }} -->
    <li>
      {{ item.title }}: {{ item.place }}, {{ item.date }}. 
    </li>
    {% endfor %}
    </ul>
</div>

<div id="Workshop" class="tabcontent">
    <ul style="margin-left:1.5rem; padding:0;">
    {% for item in site.data.act_workshop %}
    <!-- {{ item }} -->
    <li>
      {{ item.title }}: {{ item.workshop }}, {{ item.place }}, {{ item.date }}. 
    </li>
    {% endfor %}
    </ul>
</div>





