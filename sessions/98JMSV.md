---
layout: session
title: "Some Assembly Required"
code: "98JMSV"
speaker_names: ['Sarah Hoffmann']
affiliations: None
room: "Maasai Mara"
length: "20"
time: "Friday, 14:30"
time_iso: "2024-09-06T11:30:00Z"
resources: [{ description: "Slides", url: "https://pretalx.com/media/sotm2024/submissions/98JMSV/resources/sotm2024_assembly_required_fYtOQFq.pdf" }]
recording: False
---

The more detailed our mapping of the real world becomes, the more it becomes apparent that a single node, way or relation is insufficient to represent the complex properties of a real-word object. Streets have many lanes. Buildings have entrances, 3D shapes and POIs inside. And let's not even start talking about the complexity of a major railway station.

This talk will take a systematic look at the different ways how complex objects are being mapped in OSM. We explore how editors cope with the complexities of detailed mapping and discuss the implication on how our processing tools need to change to better handle relationships between objects.

<hr>

In the early OSM days, when the map was still largely a white canvas, it was very easy to stick to a simple one-to-one relationship between real-world features and OSM objects. A street is a way. A building is a single closed way.
But the more we get into the details of mapping, the more this one-to-one principle gets us into trouble. Streets have many lanes. Buildings have entrances, 3D shapes and POIs inside. And let's not even start talking about the complexity of a major railway station.

For some of these complex constructs we have developed mapping schemas - using special tagging, relations or relying on spatial properties. But more often than not, the question of relationship between OSM object is sidestepped. The situation is more dire on the side of the processing tools. Most generic tools still look at every OSM object as an isolated feature. The tools that do process complex objects often do so only for a very specific type like 3D buildings or turning restrictions.

This talk will take a systematic look at the different ways how complex objects are being mapped in OSM. We explore how editors cope with the complexities of detailed mapping and discuss the implication on how our processing tools need to change to better handle relationships between objects.

