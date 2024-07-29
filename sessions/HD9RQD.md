---
layout: session
title: "Shifting trends in global evolution of corporate mapping in OSM"
code: "HD9RQD"
speaker_names: ['Benjamin Herfort']
affiliations: None
room: "Auditorium 2"
length: "20"
time: "Sunday, 12:00"
time_iso: "2024-09-08T09:00:00Z"
resources: []
recording: False
---

This talk will look at corporate editing in OSM at three scales - global, national and local. Our results show that corporate editing increased from 2016 to 2021, but has decreased since then. Nevertheless, in recent years there has been a diversification of corporations, with an increase in edits from Digital Egypt or Grab and other smaller corporations. Corporate mapping tends to focus more on high and medium HDI regions, but our results also suggest that there is only a small influence of corporate mapping dynamics on other parts of the OSM mapping community in a country.

<hr>

Introduction:

In recent years, with the emergence of corporate editing in OpenStreetMap (OSM), there has been interest, and in some cases concern, about its influence in OSM. For instance, large corporations like such as Apple, Microsoft, Meta and Amazon have hired large teams to edit in OSM ​[1]. The launch of the Overture Maps Foundation, by Amazon, Meta, Microsoft and TomTom hosted by the Linux Foundation in 2022 and the release of its first dataset [2] has also led to heated debates on the OSM forum, regarding the future of OSM. Concerns have been raised about the monopolisation of geodata, the replacement of OSM by other sites or the backlining of OSM [3]. 

Consequently, analysing and continuously monitoring the impact of corporate contributors and continuing to observe their fluctuating patterns of editing will be significant to the understanding of the sustainability of OSM. Therefore, this talk will look at corporate editing in OSM at three scales - global, national and local to answer the two research questions:

(RQ1) What is the impact of corporate mapping on global scale mapping?

(RQ2) What is the impact of corporate mapping on country and small-scale mapping? 

Methodology:

There are two main avenues to track corporate contributors: Either through corporate affiliated OSM User IDs (UIDs) or through corporate hashtags in OSM changesets. UIDs of corporation affiliated mappers have been used in the past to track corporate activity in OSM (e.g. [1, 4, 5]). A list of affiliated usernames can be collected from disclosed lists on the OSM Wiki or corporations GitHub pages [6]. The second way to track corporate edits is through corporate hashtags in changesets. Since 2009, it became possible to add hashtags to changesets in OSM, and this has become common practice, especially to show affiliation to regions, events, organisations or corporations [7]. For the analysis presented here, in total 24 companies were tracked including Apple, Kaart, Amazon, Microsoft, TomTom, Grab, DigitalEgypt, Mapbox and Meta. We used tracking with hashtags was used as proposed by [7].

The dataset used for the analysis integrated data from two sources: The OpenStreetMap History Database [8] and the OSM Changeset database. The OSHDB was used to derive OSM geometries and attribute information as well as information about the editors. The data was then intersected with a dataset of country boundaries to assign a mapping to a specific country. The OSM changeset dataset was joined to this contribution dataset. The dataset included a plethora of information, but the most relevant columns for the analysis were the OSM ID, Changeset timestamp, hashtags and User IDs, country, year and month as well as the geometry information – including the centroids. (We aim at presenting this dataset in detail in another workshop at SOTM 2024.)

At the global level, two analyses were carried out. First, the temporal development of corporate and total edits from 2016-01-01 – 2023-12-31, including a breakdown by individual corporation. Second, the absolute number of corporate edits per country and the percentage of corporate edits based on total edits per country for the period 2019-06-01 to 2023-05-31 were analyzed. For an additional overview, the country-level results were grouped by Human Development Index (HDI) class, for a more in depth understanding of the spatial distribution of corporate edits in respect to socio-economic factors.

Countries with more than 15% corporate edits and more than 100,000 total edits in this period were selected for an in-depth analysis. A total of 28 countries met these requirements and we extracted the monthly corporate and non-corporate edits. The overall timeframe for analysis was divided into two time periods: t0 (2019-06-01– 2021-05-31) and t1 (2021-06-01 – 2023-05-31). For each country we derived the change in average activity for both corporate and non-corporate mapping.

Three countries were selected from the 28 countries with high corporate mapping activity for the small-scale analysis: Colombia, Indonesia and the United Arab Emirates. For these countries we produced a high-resolution spatial dataset based on a H3 grid utilizing the centroid geometry of each OSM contribution. We performed a spatial auto-correlation analysis to identify regions where corporate (and non-corporate) edits have increased / declined over the past years. In addition to the maps, a normalized confusion matrix was calculated to compare the spatial autocorrelation results and present the overlap or difference between the trends in corporate and non-corporate mapping.

Results and Discussion:

At the global scale (RQ1), corporate editing increased from 2016 to 2021 and has decreased since then. There is a wide variety of companies involved in OSM, but the large number of edits and its concurrent decrease in edits is mainly driven by three companies, namely Meta, Kaart and Apple. Other researchers have investigated corporate mapping activity ​[1, 4, 7]​, but a decline in their mapping activity has not yet been reported or expected. The observed decline is particularly evident in the case of Apple, which experienced a peak in edits during 2020 (14 million edits) and 2021 (12 million edits) before decreasing by more than half in 2022 (4 million edits).

Corporate edits are concentrated in high and medium HDI regions, with almost 80% of edits distributed across 32 countries. As seen in other analyses, non-organised mapping tends to focus on very high HDI regions ​[9]​, while humanitarian mapping tends to focus on low HDI regions [10]. The results presented here suggest that corporate mapping tends to focus more on high and medium HDI regions. The discussion about digital inequalities and power imbalances that may arise from corporate contributions in particular countries or regions should be ongoing, as it is a discussion for OSM as a whole. ​​​As of now, it is not clear why the large tech corporates map less. At the same time, it is unlikely that all high and medium HDI countries are completely mapped in OSM already [10].

Regarding the small-scale analysis our results show that there is no strong correlation between the increase or decrease in the mean corporate or non-corporate edits for the three selected countries. For most regions with a strong increase (high-high cluster) or decrease (low-low cluster) in corporate or non-corporate edits, there is no significant change for the other. This suggests that there is only a rather small influence of corporate mapping dynamics on other parts of the OSM mapping community in a country.

The ability to quantify the impact of corporate editing, particularly on volunteer mapping behaviour, continues to be an important measure for the OSM community. For example, further investigating would be necessary to understand the intentions and impacts of corporate mapping for various map features (not just looking at overall edit count). Understanding the intentions of different groups and communities in OSM and their impact on the data is a core necessity to obtain ’OSM Data Literacy’, especially for everyone who relies on high quality OSM data for research, business or decision making.

