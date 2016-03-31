---
title: Kickoff Workshop Details
layout: page
---
# NIST Kickoff Workshop Results

## Slide Decks From Workshop

[Marty Burns, Dave Wollman, and Partner Introductions](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/IoT-EnabledSmartCityFrameworkOverviewFinal_20160324.pdf)

1. [Michal Koenig, QualComm](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/MichalKoenig_NIST_24_March_2016.pdf)
2. [Dan Hoffman, Montgomery County Maryland, USA](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/DanHoffman_IOT_Deployed_PPI.pdf)
3. [David Jenkins, IBM](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/DavidJenkins_IBM_Smart_City.pdf)
4. [James Aloisi, City Protocol](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/JimAloisi_NIST_IES_city_presentation_jarecov_3_2016-2.pdf)
5. [Shi-Wan Lin - Industrial Internet Consortium](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/Shi-WanLin_ies-city-20160324.pdf)
6. [Ramesh Peri, Intel](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/RameshPeri_NIST-Presentation.pdf)
7. [Sephano de Panfilis, Engineering - Open and Agile Smart Cities](https://s3.amazonaws.com/nist-sgcps/smartcityframework/files/GCTCTechJamKickoff/StefanoDePanfilis_20160324-FIWAR_and_OASC-at-IES.pdf)


## Videos From Workshop
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

