---
layout: session
title: "Catching OSM Up with External Data with a Workflow and Tools for Conflation and Validation"
code: "N7TGMA"
speaker_names: ['Stefan Keller']
affiliations: None
room: "Auditorium 2"
length: "20"
time: "Saturday, 17:00"
time_iso: "2024-09-07T14:00:00Z"
resources: []
recording: False
---

This report outlines a project to improve the workflow for integrating external open datasets into OpenStreetMap (OSM), ensuring compliance with import guidelines. The process includes tools for conflating data with OSM, supported by roles and tasks specific to this workflow. The AllThePlaces project supports this by extracting and mapping open (government) data to the OSM schema. A new tool, &#34;DiffedPlaces&#34;, is proposed to automate diffs, perform data matching with an improved machine learning algorithm, and host the results. In addition, the existing OSM Conflator tool set, enhanced with a web-based data validation application, will be connected to DiffedPlaces.

<hr>

This is a work-in-progress report on an applied university research project to improve the workflow for integrating external &#34;third party&#34; datasets into OSM to complete OSM while adhering to the the import guidelines. First, the workflow for conflating (merging, fusing) external data into OSM is outlined with the main roles and tasks involved. Then some existing and missing software tools and challenges are presented.

At the beginning there's data compliant to the ODbL license - especially selected open government data (OGD) - in raw format, or open data already mapped to the OSM schema from the existing AllThePlaces (ATP) project. ATP is a set of spiders and scrapers for extracting external open data. ATP implements periodic extraction, schema mapping, and hosting.

A missing piece is the planned open source tool with the working title &#34;DiffedPlaces&#34;, which will periodically process &#34;diffs&#34; from ATP and external data, i.e. OSM elements to be created, updated or deleted. DiffedPlaces will provide matching (incl. deduplication, record linkage, named entity resolution) and &#34;diffing&#34; external data to OSM as well as hosting. 

Another existing tool set is the OSM Conflator web application originally implemented by Ilya Zverev. It implements extraction and schema mapping (like ATP) as well as diffing, validating and hosting. Part of OSM Conflator is the cf_audit GUI web application, which presents the diffed data to be validated by the mappers. It already gives an idea of how diffing reduces tedious manual validation. Only after several validations and communication with the community, the data is finally updated to OSM. This tool will be extended to replace Overpass and it's limited matching capabilities with a connection to DiffedPlaces. This will allow OSM Conflator to focus on validation and hosting, while the matching and diffing would be done in one place, in DiffedPlaces, where other OSM tools and data editors can also connect.

One of the challenges is data matching, which is being addressed with an extended random forest based algorithm from Piech et al. 2020. Another challenge is the management of the OSM elements to be deleted.

