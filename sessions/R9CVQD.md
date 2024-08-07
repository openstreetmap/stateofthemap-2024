---
layout: session
title: "Assessing the attribute accuracy and logical consistency of road data in OpenStreetMap"
code: "R9CVQD"
speaker_names: ['Wangshu Wang']
affiliations: None
room: "Tsavo Hall"
length: "20"
time: "Sunday, 10:00"
time_iso: "2024-09-08T07:00:00Z"
resources: []
recording: False
---

Our work aims to assess OSM road data quality with a focus on car driving. Current work-in-progress proposed indicators to assess attribute accuracy, with a focus on speed limits and methods for estimating the logical consistency of road data.

<hr>

Due to the crowdsourced nature of OpenStreetMap (OSM) and the lack of quality control during the contribution, the data quality issue has become a research focus [1]. Understanding and addressing these data quality issues can facilitate unlocking OSM's full potential for diverse applications. OSM data quality assessment methods can be divided into two broad categories: extrinsic and intrinsic. Extrinsic quality assessment methods compare OSM data with a reference dataset (e.g., authoritative data sources). This is where most initial research on OSM data quality started from [2-4]. Yet, a reference dataset may not always be available. On this ground, researchers called for attention to the intrinsic indicators of OSM data quality [5] and proposed intrinsic data quality measures based on the data, data history, and metadata [5-9]. 
It is crucial to acknowledge that the quality of OSM data is not a one-size-fits-all metric. Rather, it heavily depends on the purpose of the application domain, known as &#34;fitness-for-use&#34; [5,10]. The diverse application potentials introduce dynamic data requirements. Navigation is one of the primary application domains in which OSM plays a pivotal role. Among them, vehicular traffic constitutes a significant portion of road usage and has a substantial impact on urban mobility and infrastructure planning. Additionally, the complexities involved in automotive navigation and traffic systems require a higher level of data accuracy and reliability, making it a compelling starting point for investigating intrinsic road data quality.
In the context of car driving, the attribute accuracy and logical consistency of road data are particularly important [11]. Attribute accuracy refers to the correctness and logical coherence of attributes associated with road features, such as speed limits, road classifications, and turn restrictions [12]. Logical consistency ensures that the road network data follows the correct topological rules, such as proper connectivity of different road classes. The attribute accuracy and logical consistency of OSM road data are essential for traffic planning and supporting navigation applications.
To address the challenges of the evaluation of OSM data quality for navigation, when a reference dataset is unavailable, this research narrows its focus on assessing the attribute accuracy and logical consistency of OSM road data. 
To assess the attribute accuracy, we first identified important attributes related to car driving, such as road name, road class, surface, speed limit, capacity, height limit, total weight limit, and vehicle type. Then our method assesses the attribute completeness by looking into the tags related to the aforementioned attributes, and whether the relevant information is available. The attribute completeness provides us with a first overview of the attribute data. 
In the next step, a set of rules based on country-specific traffic laws is defined, and the relevant attributes are checked against these rules. So far, we have looked into the traffic law in Germany and defined rules for speed limits according to the road classes. Our proposed method looks into the “maxspeed” tag of each road segment, and verifies their value against the rule defined for the corresponding “highway” value. When a mismatch occurs, these road segments are identified and considered as inaccurate. 
The inaccuracy of the speed limit is calculated as the number of road segments with an invalid “maxspeed” value divided by the total road segments with “maxspeed”. At the current stage of our work-in-progress, we verified our method in the Heidelberg region, where the inaccuracy rate is very low. 
Regarding logical consistency, a set of rules is defined based on country-specific conventions. We acknowledge that different regions in the world have different road construction and road mapping conventions. So far, we have based on our case study in Germany, and defined rules for the values of the “highway” tag. These rules include: the value of the “highway” tag should be consistent along a path; a link road should be connected to its corresponding highway; connection of different classes of roads should be logically consistent (a way with a high level of importance in the road network should not connect directly to a way with a much lower level of importance).
Our work aims to assess OSM road data quality with a focus on car driving. Current work-in-progress proposed indicators to assess attribute accuracy, with a focus on speed limits and methods for estimating the logical consistency of road data. In the next step, we plan to build more rules for speed limits, considering the geometry of the road and their neighbouring zone to infer the speed limit. We will also leverage machine learning methods to set up rule sets for speed limits and road connections for different regions of the world. 
With the proposed assessment, OSM data users can verify road data quality in terms of attribute accuracy and logical consistency, before their intended use. With the evaluation method, we also aim to inform the potential improvement of OSM road data quality, especially for navigation.

