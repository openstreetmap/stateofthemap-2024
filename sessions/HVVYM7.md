---
layout: session
title: "Generating Ways with the Strava Heatmap"
code: "HVVYM7"
speaker_names: ['Derick Yang', 'Drew Robb']
affiliations: None
room: "Tsavo Hall"
length: "20"
time: "Saturday, 16:30"
time_iso: "2024-09-07T13:30:00Z"
resources: []
recording: False
---

The Strava Global Heatmap visualizes aggregated public GPS traces, guiding athletes worldwide in planning their routes by highlighting popular paths. This presentation demonstrates how the Heatmap, in conjunction with our routing engine, can be utilized to identify and fill in missing ways in OpenStreetMap (OSM). We will discuss an algorithmic strategy for creating generated pathways and introduce a prototype of an interface that facilitates the easy integration of these pathways into OSM. We will showcase how Strava's Heatmap can promote OSM's goal of developing a more comprehensive global map, highlighting a mutually beneficial relationship between the two platforms.

<hr>

At Strava, we encourage and support over one hundred million athletes to be active. Athletes memorialize their physical activity via activity uploads that they can share with friends around the world. The vast majority of activities uploaded to Strava include time-series GPS traces. This wealth of information underpins our geospatial products, such as advanced routing capabilities and the visually engaging Global Heatmap. Through Strava Metro, we extend this aggregated and de-identified data at no cost to entities like governments, urban planners, and NGOs, aiding in the creation of more efficient human-powered transportation infrastructures.

The backbone of Strava's routing algorithm lies in attributing popularity to roads and trails in our edge graph. We align raw GPS lines from Strava activities to these edges, enabling a popularity-driven routing experience that highlights preferred routes within the collection of OSM ways. With over a billion uploads, Strava athletes cover over 55% of the ways in OpenStreetMap with human-powered activity.

In contrast, the Global Heatmap presents an unaligned aggregation of GPS lines for over one billion public activities, offering an intuitive visual representation to aid athletes in exploring their surroundings. It's this dataset that Strava Metro partners leverage to extract insights on the safety, directness, and overall appeal of routes in cities, parks, and recreation areas.

We found that Metro partners will often overlay the Heatmap onto physical maps to identify and fill gaps in local pedestrian and cycling infrastructures. In response, we built a prototype of a tool that automates the identification and labeling of unaligned geometries, allowing our partners to streamline the process of integrating these new geometries into OSM. This innovative approach utilizes GPS data points unattributable to existing OSM edges to generate potential new pathways, enabling mappers to enrich the map with previously uncharted ways.

Leveraging Strava's global scale, we have batch-processed a collection of these potential pathways worldwide. This data can help fill in unmapped areas and highlight regions needing more mapping attention. It can also highlight commonly used unauthorized paths and potential areas for infrastructure development.

This presentation will delve into the algorithms that facilitate the generation of these new edges and explain how mappers can harness this data to enrich the OSM database, fostering a more comprehensive map for human-powered transport.

