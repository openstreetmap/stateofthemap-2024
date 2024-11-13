---
voc: https://media.ccc.de/v/sotm2024-49359-some-assembly-required
recordings: [{'size': 125, 'length': 1530, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2024-49359-eng-Some_Assembly_Required_webm-hd.webm', 'state': 'new', 'folder': 'webm-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2024-11-02T15:01:44.449+01:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2024/webm-hd/sotm2024-49359-eng-Some_Assembly_Required_webm-hd.webm', 'url': 'https://api.media.ccc.de/public/recordings/81306', 'event_url': 'https://api.media.ccc.de/public/events/6ba0affe-8abc-5c98-ac72-e4348cae827e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2024'}, {'size': 60, 'length': 1530, 'mime_type': 'video/webm', 'language': 'eng', 'filename': 'sotm2024-49359-eng-Some_Assembly_Required_webm-sd.webm', 'state': 'new', 'folder': 'webm-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2024-11-02T14:51:04.047+01:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2024/webm-sd/sotm2024-49359-eng-Some_Assembly_Required_webm-sd.webm', 'url': 'https://api.media.ccc.de/public/recordings/81305', 'event_url': 'https://api.media.ccc.de/public/events/6ba0affe-8abc-5c98-ac72-e4348cae827e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2024'}, {'size': 42, 'length': 1530, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2024-49359-eng-Some_Assembly_Required_sd.mp4', 'state': 'new', 'folder': 'h264-sd', 'high_quality': False, 'width': 720, 'height': 576, 'updated_at': '2024-11-02T14:33:56.131+01:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2024/h264-sd/sotm2024-49359-eng-Some_Assembly_Required_sd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/81304', 'event_url': 'https://api.media.ccc.de/public/events/6ba0affe-8abc-5c98-ac72-e4348cae827e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2024'}, {'size': 23, 'length': 1530, 'mime_type': 'audio/mpeg', 'language': 'eng', 'filename': 'sotm2024-49359-eng-Some_Assembly_Required_mp3.mp3', 'state': 'new', 'folder': 'mp3', 'high_quality': False, 'width': 0, 'height': 0, 'updated_at': '2024-11-02T14:32:02.747+01:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2024/mp3/sotm2024-49359-eng-Some_Assembly_Required_mp3.mp3', 'url': 'https://api.media.ccc.de/public/recordings/81303', 'event_url': 'https://api.media.ccc.de/public/events/6ba0affe-8abc-5c98-ac72-e4348cae827e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2024'}, {'size': 114, 'length': 1530, 'mime_type': 'video/mp4', 'language': 'eng', 'filename': 'sotm2024-49359-eng-Some_Assembly_Required_hd.mp4', 'state': 'new', 'folder': 'h264-hd', 'high_quality': True, 'width': 1920, 'height': 1080, 'updated_at': '2024-11-02T14:30:25.302+01:00', 'recording_url': 'https://cdn.media.ccc.de/events/sotm/2024/h264-hd/sotm2024-49359-eng-Some_Assembly_Required_hd.mp4', 'url': 'https://api.media.ccc.de/public/recordings/81302', 'event_url': 'https://api.media.ccc.de/public/events/6ba0affe-8abc-5c98-ac72-e4348cae827e', 'conference_url': 'https://api.media.ccc.de/public/conferences/sotm2024'}]
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

