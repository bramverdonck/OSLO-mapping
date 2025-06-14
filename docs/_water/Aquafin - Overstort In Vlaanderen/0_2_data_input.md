---
layout: default
title: Data voorbeeld
parent: Overstort
nav_order: 1
---

# Data voorbeeld

Om alles overzichtelijk te maken, voorzien we onderstaand een voorbeeld in JSON-formaat van een eventbericht en een metadatabericht van een sensor. 
Dit is ook meteen het formaat waarin de brondata wordt aangeleverd om later ter beschikking gesteld te worden via LDES.


## Event
In de events vind je telkens een berekening terug van de start- en eindtijd van elk event, gevolgd door de specificatie over welk type event het gaat. Een event kan nl. een overstorting zijn, maar even goed de afwezigheid van een overstorting of een foutmelding. 

Onderstaand een json-voorbeeld

```json
{
	"type":"Event",
	"start_timestamp":"2025-02-18T08:31:00.000Z",
	"end_timestamp":"2025-02-18T08:41:00.000Z",
	"measurement_location":"P_000000181521",
	"status":"WerkingOnbekend",
	"is_observed_with":"P1037143",
	"modified_at":"2025-02-18T10:21:17.979Z",
	"is_deleted":"false"
}
```

## Sensor
In de Sensordata-json wordt alle relevante metadata per sensor doorgestuurd. 
Indien er wijzigingen optreden in de status, locatie of kwaliteit van de sensor, wordt een nieuwe versie beschikbaar gemaakt op de LDES Server die de meest recente versie van de sensormetadata bevat.


```json
{
	"id":"P2050378",
	"device_type":"Overstortmeter",
	"name":"Overstortmeter Ijinus US LTE",
	"owner":"AQUAFIN",
	"brand":"Ijinus",
	"supplier":"ELSCOLAB",
	"serial_number":"IJA0102-00004425",
	"device_state":"ACTIEF",
	"lat_WGS84":51.04243219340782,
	"long_WGS84":5.594445509825586,
	"lat_Lambert72":193183.8663904309,
	"long_Lambert72":235956.9331605651,
	"measurement_location":"P_000000217952",
	"quality_label":"0",
	"valid_from":"2025-04-11T13:31:56.947Z",
	"valid_to":"9999-12-31T23:59:59.000Z"
	"modified_at":"2025-04-11T13:31:56.947Z"
}

```

https://github.com/smart-data-models/dataModel.Device/blob/master/Device/doc/spec.md

https://www.w3.org/TR/wot-thing-description


## Context
```json
{
  "@context": {
      "@language": "nl",
      "adms": "http://www.w3.org/ns/adms#",
      "qudt-schema": "https://qudt.org/schema/qudt/",
      "terms": "http://purl.org/dc/terms/",
      "time": "http://www.w3.org/2006/time#",
      "sc": "http://purl.org/science/owl/sciencecommons",
      "skos": "http://www.w3.org/2004/02/skos/core#",
      "geosparql": "http://www.opengis.net/ont/geosparql#",
      "qudt-unit": "https://qudt.org/vocab/unit/",
      "sosa": "http://www.w3.org/ns/sosa/",
      "xsd": "http://www.w3.org/2001/XMLSchema#",
      "schema": "https://schema.org",
      "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
      "locn": "http://www.w3.org/ns/locn#",
      "geo" : "http://www.w3.org/2003/01/geo/wgs84_pos#",
      "prov": "http://www.w3.org/ns/prov#",
      "sosa": "http://www.w3.org/ns/sosa/",
      "ssn": "http://www.w3.org/ns/ssn/",
      "aquafin": "https://aquafin.be/ns#",
      "dcterms": "http://purl.org/dc/terms/",
      "environment": "https://smartdatamodels.org/dataModel.Environment/",
      "sdm": "https://smartdatamodels.org/"
      }
  }
```
