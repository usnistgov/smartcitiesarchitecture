---
title: Consensus PPI
layout: page
---



# Consensus PPI
**Email List:** [mail to](mailto:scf_consenusppi@nist.gov) or [join](mailto:scf_consenusppi-join@nist.gov) 

**Workshop Webinars:** [https://global.gotomeeting.com/join/752972149](https://global.gotomeeting.com/join/752972149) phone:+1(312)757-3121;752972149#

**Meetings:** Tri-weekly 9:00A EDT

**Page Contents:**

* TOC
{:toc}


## Charter

The purpose of the Consensus PPI is to analyze:

* Existing exemplary Smart City Architecture and Internet of Things (IoT) descriptions including:
	* Standards, specifications
	* Architectures, frameworks, conceptual models
    * Platforms, protocols, environments 

* Document their overlapping concerns such as functionality, data, timing, trustworthiness, etc…

* Determine the common “properties” (solutions) specified in these overlapping concerns such as third party authentication, data encryption, time synchronization, data formats/ontologies

* Document these “PPI” and show the overlaps, gaps, and commonalities of choices made by the creators of the reviewed descriptions

## Deliverables

  * Set of analyzed suites according to CPSFramework Aspects/Concerns spreadsheet
  * Description of Methodology
  * Text for the IES-City Framework Document section on Consensus PPI

## Major Milestones

  * [October 2017] Complete analyses
  * [November 2017] Complete draft Text
  * [November/December 2017] Participate in IES-City Framework version 0.7 Workshop introduction
  * [December 2017-February 2018] Review Comments
  * [February 2017] Publish IES-City Framework version 1.0

## List of Technologies Being Analyzed

*Note: this activity will not judge the merits or comparative benefits of any technology. It seeks only to research the potential common Pivotal Points of Interoperability (PPI) that they have in common. Therefore there is a mix of standards, specifications, and commercial suites and ecosystems in the analysis. Analysis by any proponent is purely voluntary. This list will vary during the progress of the project.*

<table style="padding:4px;border-collapse: collapse;border:solid 4px;width:100%;font-family:Arial, Helvetica, sans-serif">
  <tr style="border:solid 2px;background-color:#b3d9ff;font-weight: bold">
    <td >Status (initiating, in-progress, completed)</td>
    <td style="border:solid 1px">Technology</td>	<td style="border:solid 1px">Contact</td>
    <td style="border:solid 1px">Link</td>
  </tr>
  <tr>
    <td style="border:solid 1px">in-progress</td>
    <td style="border:solid 1px">OpenIOT</td>	
    <td style="border:solid 1px">Arkady Zaslavsky</td>
	<td style="border:solid 1px"><a ref="https://github.com/OpenIotOrg/openiot">https://github.com/OpenIotOrg/openiot</a></td>
  </tr>
  <tr>
    <td style="border:solid 1px">in-progress</td>
    <td style="border:solid 1px">The FIWARE Architecture for Smart Cities</td>
    <td style="border:solid 1px">Stephano de Panafilis</td>
    <td style="border:solid 1px"><a ref="http://fiware.org/">http://fiware.org/</a></td>
  </tr>
  <tr>
    <td style="border:solid 1px">in-progress</td>
    <td style="border:solid 1px">oneM2M (Standards for M2M and the Internet of Things) Architecture</td>
    <td style="border:solid 1px">SeungMyeong Jeong</td>
    <td style="border:solid 1px"><a ref="http://www.onem2m.org/technical/published-documents">http://www.onem2m.org/technical/published-documents</a></td>
  </tr>
  <tr>
    <td style="border:solid 1px">in-progress</td>
    <td style="border:solid 1px">Connected Vehicle Reference Implementation Architecture</td>
    <td style="border:solid 1px">David Binkley</td>
    <td style="border:solid 1px"><a ref="http://www.iteris.com/cvria/">http://www.iteris.com/cvria/</a></td>
  </tr>
  <tr>
    <td style="border:solid 1px">in-progress</td>
    <td style="border:solid 1px">E015 Digital Ecosystem</td>
    <td style="border:solid 1px">Emiliano Sergio Verga</td>
    <td style="border:solid 1px"><a ref="http://www.e015.regione.lombardia.it/PE015/">http://www.e015.regione.lombardia.it/PE015/</a></td>
  </tr>
  <tr>
    <td style="border:solid 1px">-</td>
    <td style="border:solid 1px">-</td>	
    <td style="border:solid 1px">-</td>
    <td style="border:solid 1px"><a ref="">-</a></td>
  </tr>
</table>

## Working Group Files

<dl>
{% for document in site.data.documents %}
  {% if document.team == "consensusppi" %}
  
  <dt>
    <a href="{{document.url}}" >
    {{document.name}} ({{document.category}})</a>
  </dt>
  <dd>{{document.description}}</dd>

  {% endif %}
{% endfor %}
</dl>