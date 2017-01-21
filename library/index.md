---
title: IoT-Enabled Smart City Framework Library
layout: page
---

# IES-City Framework Library

---

<p>The following documents are working documents of the IES-City Framework</p>

<a href="#video">Videos</a> || <a href="#presentation">Workshop Presentations</a> || <a href="#document">Documents</a> 
<hr />


## Framework Document Drafting
<dl>
{% for document in site.data.documents %}
  {% if document.team == "smartcityframework" %}
  
  <dt>
    <a href="{{document.url}}" >
    {{document.name}} ({{document.category}})</a>
  </dt>
  <dd>{{document.description}}</dd>

  {% endif %}
{% endfor %}
</dl>


<a id="Presentation">&nbsp;</a>

## Workshop Presentations


### Austin Workshop June 15-16 2016

<dl>
{% for document in site.data.documents %}
  {% if document.category == "presentation" %}
  {% if document.team == "austinmidpoint" %}
  
  <dt>
    <a href="{{document.url}}" >
    {{document.name}} (Presentation)</a>
  </dt>
  <dd>{{document.description}}</dd>

  {% endif %}
  {% endif %}
{% endfor %}
</dl>

### ENEA Workshop April 14-15 2016

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


### NIST Workshop March 24-25 2016

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

## Videos From NIST and ENEA Kickoff Workshops

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

    {% if video.type == 'youtube' %}
	<iframe width="450" height="240" src="{{video.url}}">
		Your browser does not support HTML5 video.
	</iframe>
    {% endif %}

</dl>
</div>
{% endfor %}


---
Checksums for the documents stored for this site can be found [here](checksums)