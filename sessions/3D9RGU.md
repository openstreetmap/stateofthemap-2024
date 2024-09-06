---
layout: session
title: "Setting the Stage for the Future of Web Based Mapping"
code: "3D9RGU"
speaker_names: ['Martin Raifer']
affiliations: None
room: "Maasai Mara"
length: "20"
time: "Friday, 15:00"
time_iso: "2024-09-06T12:00:00Z"
resources: [{ description: "slides", url: "https://pretalx.com/media/sotm2024/submissions/3D9RGU/resources/2024-sotm_QZ4ZpWM.pdf" }]
recording: False
---

Over the years, iD has become a quite capable, versatile and reliable editor for OSM. However, it is currently also facing of a number of challenges: For example, it needs to keep being able to cope with the growing amount and richness of OSM’s map data, as well as to afford the increasingly important task of keeping the map up to date.

This talk outlines a proposal to transform iD’s current user interface centered around OSM’s data model into an adaptive user experience that is better tailored towards the needs of individual mappers and outlines an approach of how we can get there as a community.

<hr>

In the past, iD had to and has overcome several challenging hurdles to become what it is today: A quite unique map editor that is the point of entry of most contributors of OpenStreetMap into the world of mapping.

Today, iD is facing of a number of signifiant challenges to make it even more usable to a wide user base, and will continue to do so into the foreseeable future especially in regards to make it fit for the mapping topics of the future. For example, the editor needs to be able to cope with the growing amount and richness of OSM’s map data as well as as the increasingly important task of keeping the map up to date.

The design of iD’s current user interface is substantially based on OSM’s data model. This can be seen for example in the workflow of creating a new map feature: It starts out with a blank “dummy” map geometry which – in a second step – has to be converted into a map feature by choosing a preset. While this is true to the way OSM represents this information in the data (i.e. in the form of nodes, ways and relations which are enriched with tags), this is for most simple use cases an unnecessary complication.

Instead of primarily catering to the needs and requirements arising from the underlying data structures, iD’s usability should be instead built around the needs of of the different groups of mappers. And as these vary quite significantly depending on the interests and/or experience of the individual mappers, a promising approach to bring all of these together is to evolve iD’s user interface into an adaptive mapping experience with the goal to make vital mapping workflows intuitive, easy, fast and delightful.

This transformation will definitely not be a small endeavor and is far from finally defined: in fact this should only be a start of a larger discussion. Let us together flesh out the details of this project.

