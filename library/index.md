---
title: IoT-Enabled Smart City Framework Library
layout: page
---

#Library

---
<h2>IoT-Enabled Smart City Framework Library</h2>
<p>The following documents are working documents of the IoT-Enabled Smart City Framework</p>
<section>

<a href="#video">Videos</a> || <a href="#presentation">Presentations</a> || <a href="#document">Documents</a> 
<hr />

<a id="Presentation">&nbsp;</a>
<h3>Presentations</h3>
<dl>
{% for document in site.data.documents %}

  {% if document.category == "presentation" %}
  <dt>
    {% if document.html %}
    <a href="{{document.html}}" >
    {{document.name}} (Web Page)</a>
    {% endif %}
	
    {% if document.doc %}
    <a href="{{document.doc}}" >
    {{document.name}} (Document) </a>
    {% endif %}

    {% if document.pdf %}
    <a href="{{document.pdf}}" >
    {{document.name}} (PDF) </a>
    {% endif %}

  </dt>


  <dd>{{document.description}}</dd>

{% endif %}
{% endfor %}
</dl>

<a id="document">&nbsp;</a>
<h3>Documents</h3>
<dl>
{% for document in site.data.documents %}

  {% if document.category == "document" %}
  <dt>
    {% if document.html %}
    <a href="{{document.html}}" >
    {{document.name}} (Web Page)</a>
    {% endif %}

    {% if document.doc %}
    <a href="{{document.doc}}" >
    {{document.name}} (Document) </a>
    {% endif %}

    {% if document.pdf %}
    <a href="{{document.pdf}}" >
    {{document.name}} (.pdf) </a>
    {% endif %}

  </dt>


  <dd>{{document.description}}</dd>

{% endif %}
{% endfor %}
</dl>





  
