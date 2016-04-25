---
title: Consensus PPI
layout: page
---

# Consensus PPI

**Email List:** [mail to](mailto:scf_consenusppi@nist.gov) or [join](mailto:scf_consenusppi-join@nist.gov) 

**Workshop Webinars:** [https://global.gotomeeting.com/join/752972149](https://global.gotomeeting.com/join/752972149) phone:+1(312)757-3121;404083029#

**Meetings:** Bi-weekly starting May 3, 2016 8:00A EDT


## Charter

The purpose of the Consensus PPI is to analyze:
  * Existing exemplary Smart City Architecture and Internet of Things (IoT) descriptions including
    * Standards, specifications
    * Architectures, frameworks, conceptual models
    * Platforms, protocols, environments 

  * Document their overlapping concerns such as functionality, data, timing, trustworthiness, etc…

  * Determine the common “properties” (solutions) specified in these overlapping concerns such as third party authentication, data encryption, time synchronization, data formats/ontologies

  * Document these “PPI” and show the overlaps, gaps, and commonalities of choices made by the creators of the reviewed descriptions

## Deliverables

  * [Stefano] Refine scope on email list prior to May 3rd meeting
  * [15May] Deliverable 1 – finalize CPS Framework Concerns for IES-City FW
  * [6Jun] Deliverable 2 – draft analysis of several
  * [30Sep] Analyzed PPIs version 0.8

## Major Milestones

  * End of April to collect Architectures and Experts
  * First Teleconference will be beginning of May, Bi-weekly through two months
  * May 3rd 8:00am, every other Tuesday
  * May 3: Organizational
  * May 17th: Review of Concerns
  * 1 ½ months for analysts
  * June 12..14 in Austin, TX USA F2F Workshop
  * July to combine with other groups

# Working Group Files

<dl>
{% for document in site.data.documents %}
  {% if document.team == "consensusppi" %}
  
  <dt>
    <a href="{{document.url}}" >
    {{document.name}} (Presentation)</a>
  </dt>
  <dd>{{document.description}}</dd>

  {% endif %}
{% endfor %}
</dl>