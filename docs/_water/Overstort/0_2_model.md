---
layout: default
title: Implementatie model
parent: Overstort
nav_order: 2
---

## Intro

Het OSLO model [`waterkwaliteit`](https://data.vlaanderen.be/doc/applicatieprofiel/waterkwaliteit) werd gebruikt als basis om deze dataset te converteren naar een OSLO compliant dataset.


Concreet werden volgende klasses gebruikt, maar gemapt op SSN/SOSA ipv ISO19156:
* Observatie (sosa:Observation)
* Kenmerktype (sosa:ObservableProperty)
* Object (sosa:FeatureOfInterest), meer specifiek Meetpunt (wk:Meetpunt) en Emissiepunt (imjv:Emissiepunt)

<br>
<br>

## Implementatiemodel volgens SSN/SOSA

<div id="enlargeImage">
<a href="https://github.com/bramverdonck/OSLO-mapping/blob/07e9aafc0aef1c5744d26f3b2b27fc21a6221e6d/docs/_water/Overstort/Aquafin%20Overstort%20EA%20Model.jpeg?raw=tru"><img src="https://github.com/bramverdonck/OSLO-mapping/blob/07e9aafc0aef1c5744d26f3b2b27fc21a6221e6d/docs/_water/Overstort/Aquafin%20Overstort%20EA%20Model.jpeg?raw=tru" width="100%" text-align="center"></a>
</div>

Een belangrijk verschil met OSLO waterkwaliteit is dat de specifieke kenmerken en parameters (temperatuur, debiet, hoogte...) werden uitgemodelleerd op Kenmerktype in plaats van subklasses.

## OSLO Waterkwaliteit

<div id="enlargeImage">
<a href="https://data.vlaanderen.be/doc/applicatieprofiel/waterkwaliteit/kandidaatstandaard/2023-06-01/html/overview.jpg"><img src="https://data.vlaanderen.be/doc/applicatieprofiel/waterkwaliteit/kandidaatstandaard/2023-06-01/html/overview.jpg" width="100%" text-align="center"></a>
</div>