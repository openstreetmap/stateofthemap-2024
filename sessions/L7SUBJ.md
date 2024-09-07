---
layout: session
title: "Easy Access to ohsome full history OSM contributions using cloud hosted GeoParquet"
code: "L7SUBJ"
speaker_names: ['Benjamin Herfort', 'Rafael Troilo', 'Michael Auer']
affiliations: None
room: "Amboseli Hall"
length: "60"
time: "Saturday, 14:30"
time_iso: "2024-09-07T11:30:00Z"
resources: [{ description: "Workshop Slides", url: "https://pretalx.com/media/sotm2024/submissions/L7SUBJ/resources/Workshop-SotM2024-ohsome-Geoparquet_4iOAJRM.pdf" },{ description: "Workshop Book", url: "https://giscience.github.io/sotm-2024-ohsome-data-insights-workshop/intro.html" },{ description: "Github Repository", url: "https://github.com/GIScience/sotm-2024-ohsome-data-insights-workshop" }]
recording: False
---

This workshop teaches you how you can accelerate OSM data analysis without the need to run your own computing cluster. We will provide a sneak preview about our new cloud hosted ohsome full history contributions data and will show you how you can use it to understand the dynamics in OSM.

<hr>

Technological advances in the geospatial world are moving fast. In this workshop we want to explore how the OSM community, researchers and data scientists can make use of recent developments such as [GeoParquet](https://geoparquet.org/), [DuckDB](https://duckdb.org/) and [Polars](https://pola.rs/). If you have not heard of these before don’t worry, but be excited how they might transform your geospatial analysis workflows and could provide new insights about mapping in OSM.

In this workshop we will provide a sneak preview about our new cloud hosted ohsome full history contributions data. This dataset brings you something we have wanted for a long time: a single dataset which contains information about OSM objects and the related changeset metadata such as OSM editing software used, changeset comments or hashtags. As the datasets contains OSM’s full history (and not only the latest snaphshot) it’s perfectly suited to understand the dynamics in OSM. Based on this dataset we will show how you can run global scale data analyses for various (research) questions and how you can visualize the results.

We want to explore how we could combine data from OSM with other data sources. Here we want to first start with looking at the additional value of OSM Changeset metadata. We will look into the temporal evolution of OSM (what changes in OSM over time?) and what these changes can tell us about the real world. For instance, this analysis can highlight regions with a very high mapping activity for specific editors such as [StreetComplete](https://streetcomplete.app/). We want to take a closer look at the types of changes that happen in OSM. This can tell us more about the community itself and could reveal regional preferences in mapping style. The main advantage of using cloud-hosted contributions files over simply using the ohsome API is that you can actually zoom in your analysis down to the individual OSM object.

We will touch the topic of data quality (How good is OSM?) and want to compare the coverage of OSM building and road data with the coverage of other datasets from [Microsoft](https://github.com/microsoft/GlobalMLBuildingFootprints), [Google](https://sites.research.google/open-buildings/) and [other sources](https://source.coop/). This analysis can tell us something about the completeness of OSM, but also about the accuracy of those machine-learning derived datasets. As the discussion about the integration of AI datasets in OSM can be sometimes heated, we hope that this analysis will provide some common ground which regions are most likely to be affected (positively or negatively) by AI-assisted mapping.

Before diving deeper into these analysis questions we will provide a short introduction to GeoParquet files and they can be analyzed with DuckDB.  Next, we want to work on 3-4 Jupyter Notebook hands-on examples we have prepared for you. For these it would be good if participants can install QGIS in advance of the workshop. The workshop material will be made available via GitHub and the participants can use either a local python environment or a cloud hosted service such as Colab or similar tools.

We hope that this workshop can start a discussion about how we can accelerate OSM data analysis without the need to run your own computing cluster. We believe that cloud hosted GeoParquet files and DuckDB could open up OSM data analysis to a much broader audience. We invite OSM community members, researchers and data scientists to bring their own questions as we are interested to learn from you what could be done to bring those ideas into reality.

