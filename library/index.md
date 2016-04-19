---
title: IoT-Enabled Smart City Framework Library
layout: page
---

#IES-City Framework Library

---

<p>The following documents are working documents of the IES-City Framework</p>

<a href="#video">Videos</a> || <a href="#presentation">Presentations</a> || <a href="#document">Documents</a> 
<hr />

<a id="Presentation">&nbsp;</a>

## Presentations

### NIST Workshop

<dl>
{% for document in site.data.documents %}
  {% if document.category == "presentation" %}
  {% if document.team == "smartcityframeworkkickoffworkshopnist" %}
  
  <dt>
    <a href="{{document.url}}" >
    {{document.name}} (Presentation)</a>
  </dt>
  <dd>{{document.description}}</dd>

  {% endif %}
  {% endif %}
{% endfor %}
</dl>

### ENEA Workshop

<dl>
{% for document in site.data.documents %}
  {% if document.category == "presentation" %}
  {% if document.team == "smartcityframeworkkickoffworkshopenea" %}
  
  <dt>
    <a href="{{document.url}}" >
    {{document.name}} (Presentation)</a>
  </dt>
  <dd>{{document.description}}</dd>

  {% endif %}
  {% endif %}
{% endfor %}
</dl>

<a id="document">&nbsp;</a>

## Documents
<dl>
{% for document in site.data.documents %}

  {% if document.category == "document" %}
  <dt>
    <a href="{{document.url}}" >
    {{document.name}} (Document)</a>
  </dt>
  <dd>{{document.description}}</dd>

{% endif %}
{% endfor %}
</dl>

## Videos

<a id="video">&nbsp;</a>

## Videos From NIST Workshop

{% for video in site.data.videos %}
<hr />
<div style="width:470px; display:block'">
<dl>
	<dt>{{video.name}}</dt>
	<dd>{{video.description}}</dd>
	
    {% if video.type == 'use_embedded' %}
	{{video.embedded}}
    {% endif %}
	
    {% if video.type == 'mp4' %}
	<video width="450" height="240" controls preload="none" poster="{{video.embedded}}">
		<source src="{{video.url}}" type="video/mp4">
		Your browser does not support HTML5 video.
	</video>
    {% endif %}
</dl>
</div>
{% endfor %}


  
