---
title: BrAPI 2
keywords:
- markdown
- publishing
- manubot
lang: en-US
date-meta: '2023-09-12'
author-meta:
- Peter "BrapMan" Selby
- Trevor "Cool Kid" Rife
header-includes: |
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta property="og:type" content="article" />
  <meta name="dc.title" content="BrAPI 2" />
  <meta name="citation_title" content="BrAPI 2" />
  <meta property="og:title" content="BrAPI 2" />
  <meta property="twitter:title" content="BrAPI 2" />
  <meta name="dc.date" content="2023-09-12" />
  <meta name="citation_publication_date" content="2023-09-12" />
  <meta property="article:published_time" content="2023-09-12" />
  <meta name="dc.modified" content="2023-09-12T16:00:02+00:00" />
  <meta property="article:modified_time" content="2023-09-12T16:00:02+00:00" />
  <meta name="dc.language" content="en-US" />
  <meta name="citation_language" content="en-US" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="Peter &#34;BrapMan&#34; Selby" />
  <meta name="citation_author_institution" content="Cornell University" />
  <meta name="citation_author_orcid" content="0000-0001-7151-4445" />
  <meta name="citation_author" content="Trevor &#34;Cool Kid&#34; Rife" />
  <meta name="citation_author_institution" content="Clemson University" />
  <meta name="citation_author_orcid" content="0000-0002-5974-6523" />
  <link rel="canonical" href="https://plantbreeding.github.io/BrAPI-Manuscript2/" />
  <meta property="og:url" content="https://plantbreeding.github.io/BrAPI-Manuscript2/" />
  <meta property="twitter:url" content="https://plantbreeding.github.io/BrAPI-Manuscript2/" />
  <meta name="citation_fulltext_html_url" content="https://plantbreeding.github.io/BrAPI-Manuscript2/" />
  <meta name="citation_pdf_url" content="https://plantbreeding.github.io/BrAPI-Manuscript2/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://plantbreeding.github.io/BrAPI-Manuscript2/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://plantbreeding.github.io/BrAPI-Manuscript2/v/3fe174bb696987086eef7951278374563e92521b/" />
  <meta name="manubot_html_url_versioned" content="https://plantbreeding.github.io/BrAPI-Manuscript2/v/3fe174bb696987086eef7951278374563e92521b/" />
  <meta name="manubot_pdf_url_versioned" content="https://plantbreeding.github.io/BrAPI-Manuscript2/v/3fe174bb696987086eef7951278374563e92521b/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://plantbreeding.github.io/BrAPI-Manuscript2/v/3fe174bb696987086eef7951278374563e92521b/))
was automatically generated
from [plantbreeding/BrAPI-Manuscript2@3fe174b](https://github.com/plantbreeding/BrAPI-Manuscript2/tree/3fe174bb696987086eef7951278374563e92521b)
on September 12, 2023.
</em></small>



## Authors



+ **Peter "BrapMan" Selby**
  ^[✉](#correspondence)^<br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0001-7151-4445](https://orcid.org/0000-0001-7151-4445)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [BrapiCoordinatorSelby](https://github.com/BrapiCoordinatorSelby)
    <br>
  <small>
     Cornell University
     · Funded by NIFA-DSFAS 2022-67021-37024
  </small>

+ **Trevor "Cool Kid" Rife**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0002-5974-6523](https://orcid.org/0000-0002-5974-6523)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [trife](https://github.com/trife)
    <br>
  <small>
     Clemson University
  </small>


::: {#correspondence}
✉ — Correspondence possible via [GitHub Issues](https://github.com/plantbreeding/BrAPI-Manuscript2/issues)
or email to
Peter "BrapMan" Selby \<ps664@cornell.edu\>.


:::


## Abstract {.page_break_before}

The Breeding API (BrAPI) project is an effort to enable interoperability among plant breeding databases.
BrAPI is a standardized RESTful web service API specification for communicating plant breeding data.
This community driven standard is free to be used by anyone interested in plant breeding data management.
This manuscript describes updates and outlook for the current version of BrAPI.


## Introduction

<!-- 
Notes:
* DIGITAL ECOSYSTEM
* Justification for a second paper
* Highlight Community Growth
* Hackathons
* sabbaticals
* Updates for V2
* Auth Data Access Control - super simplified - highlight data privacy and security elements
* Project structure - Modules
* Standardization of endpoints across objects - said in a non-tech way
-->

<!-- PS: This opening paragraph is hot garbage and should be rewritten, but I needed to start somewhere to get the creative writing process flowing.  -->
Plant and animal breeding is an incredibly important part of today's society. Almost every country in the world has some kind of breeding program supporting the agricultural community to produce bigger, better, healthier, more sustainable crops. Modern breeding techniques require large amounts of high quality data to be effective. In the digital age, that breeding data is being collected, managed, and analyzed with computer software. Interoperability between breeding software tools, systems, and databases can substantially increase the efficiency of a breeding program. The ability to share tools gives each program a boost in computational power. The ability to share data means everyone has access to larger, more complete, datasets and get build more accurate computational models and produce more accurate predictions.

The Breeding API (BrAPI) project is an effort to enable interoperability among breeding tools, systems, and databases. BrAPI is a standardized Representational State Transfer (REST), web service, Application Programming Interface (API), specification for breeding and related agricultural data. [@doi:10.1093/bioinformatics/btz190] By using the BrAPI standard, breeding software can more easily become interoperable, allowing groups to more easily share data and software tools.

### How it works

An Application Programming Interface (API) is a technical connection between two pieces of software. Just as a Graphical User Interface (GUI) or a Command Line Interface (CLI) allows a human user to interact with a piece of software, an API allows one software application to interact with another. A GUI or CLI might allow a user to input data, read data, and start processes within an application. An API allows one piece of software (sometimes called a client, user agent, or service consumer) to programmatically input data, read data, and start process within another piece of software (sometimes called a server or service provider).

A Representational State Transfer (REST) web service is a type of API commonly used in today's modern web infrastructure. REST is a technical architecture that describes the stateless transmission of data between applications. Typically, REST systems are implemented using the standard HTTP protocol that most of the modern internet is built upon. REST implementations also generally use JavaScript Object Notation (JSON) to represent the data being transferred. Both HTTP and JSON are programming language agnostic, very stable, and very flexible. This means BrAPI can be implemented in almost any piece of software, and can solve a wide range of use cases.

### Project Updates

Over its lifetime, the BrAPI project has grown and changed substantially. The latest stable version of the specification (v2.1) looks vastly different from the original version (v1.0) 51 released in 2017. The total size of the specification has almost quadrupled in that time, going from 51 endpoints documented in v1.0 to 201 endpoints documented in v2.1. Because of this growth, the specification documents were reorganized into four modules: BrAPI-Core, BrAPI-Germplasm, BrAPI-Genotyping, and BrAPI-Phenotyping. Figure {@fig:domains}1 shows a simplified domain map of the whole BrAPI v2.1 data model, divided into the organizational modules. 

![Figure 1: A simplified domain map of the whole BrAPI data model, divided into organizational modules](images/BrAPI_Domains_v2-1_vertical.png){#fig:domains}

### Community Growth




## Success Stories

6+/- success stories highlighting BrAPI usefulness in breeding cycle

### Field Book for starting data collection

* Project Explanation
* BrAPI integration
* Layman description how it can help breeding program
  
### QBMS for the beginnings of analytics

* Project Explanation
* BrAPI integration
* Layman description how it can help breeding program
  
### [brapi sync](https://github.com/IntegratedBreedingPlatform/brapi-sync)

* Project Explanation
* BrAPI integration
* Layman description how it can help breeding program


## Discussion

* how can BrAPI help breeders (specifically small breeders)
* Looking ahead - what needs to be done further
* Analytics
* HDP
* GraphQL?
* Field mgmt - treatments etc
* Drones, image processing, HTP
* ChatGPT integration - BreedersGPT
* Weather & soil - why it won’t be in BrAPI


## Conclusions and Impact

* High level summary of the project/consortium
* BrAPI is fitting into this gap, it doesn’t need to fit these other gaps
* Call to action - Join us!


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>

