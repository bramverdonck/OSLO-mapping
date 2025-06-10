---
layout: default
parent: Overstort   
title: Examples Overstort
nav_order: 4
---

# Voorbeelden Overstort

## Prefices 

```
PREFIX dcat:                             <http://www.w3.org/ns/dcat#>
PREFIX dct:                              <http://purl.org/dc/terms/>
PREFIX foaf:                             <http://xmlns.com/foaf/0.1/>
PREFIX geo:                              <http://www.opengis.net/ont/geosparql#>
PREFIX ldes:                             <https://w3id.org/ldes#>
PREFIX m8g:                              <http://data.europa.eu/m8g/>
PREFIX overstort-event-cleansed:         <https://ldes-overstort.test.az.aquafin.be/ldes/overstort-event-cleansed/>
PREFIX overstort-event-cleansed-by-page: <https://ldes-overstort.test.az.aquafin.be/ldes/overstort-event-cleansed/overstort-event-cleansed-by-page/>
PREFIX owl:                              <http://www.w3.org/2002/07/owl#>
PREFIX prov:                             <http://www.w3.org/ns/prov#>
PREFIX rdf:                              <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs:                             <http://www.w3.org/2000/01/rdf-schema#>
PREFIX sh:                               <http://www.w3.org/ns/shacl#>
PREFIX shsh:                             <http://www.w3.org/ns/shacl-shacl#>
PREFIX skos:                             <http://www.w3.org/2004/02/skos/core#>
PREFIX tree:                             <https://w3id.org/tree#>
PREFIX xsd:                              <http://www.w3.org/2001/XMLSchema#>
```

#### Eindresultaat Overstort Sensor op de LDES Server

```
<https://aquafin.be/id/sensor/f5e0491b-13f0-4f0b-a384-e18d14070400/2025-06-06T06:53:45.831925690>
        rdf:type                     <http://www.w3.org/ns/sosa/Sensor>;
        dct:description              "Overstortmeter Ijinus RD LTE";
        dct:identifier               "P9999999";
        dct:isVersionOf              <https://aquafin.be/id/sensor/f5e0491b-13f0-4f0b-a384-e18d14070400>;
        dct:type                     "Overstortmeter";
        <http://www.w3.org/2003/01/geo/wgs84_pos#lat>
                5.129880773497998E1;
        <http://www.w3.org/2003/01/geo/wgs84_pos#long>
                4.904165566604088E0;
        prov:generatedAtTime         "2025-06-06T06:53:45.831Z"^^xsd:dateTime;
        <http://www.w3.org/ns/sosa/hasFeatureOfInterest>
                <https://aquafin.be/id/meetpunt/P_000000176054>;
        <https://aquafin.be/ns#lat_Lambert72>
                2.2113103E5;
        <https://aquafin.be/ns#long_Lambert72>
                1.8734346E5;
        <https://aquafin.be/ns#modified_at>
                "2025-04-30T08:16:08.948Z"^^xsd:dateTime;
        <https://aquafin.be/ns#quality_label>
                "E00";
        <https://aquafin.be/ns#valid_from>
                "2025-03-25T00:00:00.000Z"^^xsd:dateTime;
        <https://aquafin.be/ns#valid_to>
                "2025-04-11T13:31:56.947Z"^^xsd:dateTime;
        <https://schema.org/serialNumber>
                "IJA0102-00009961";
        <https://schema.org/vendor>  "ELSCOLAB";
        <https://smartdatamodels.org/dataModel.Environment/deviceId>
                "P9999999";
        <https://smartdatamodels.org/dataModel.Environment/deviceModel>
                "Ijinus";
        <https://smartdatamodels.org/dataModel.Environment/deviceName>
                "Overstortmeter Ijinus RD LTE";
        <https://smartdatamodels.org/dataModel.Environment/deviceStatus>
                "ACTIEF";
        <https://smartdatamodels.org/owner>
                "AQUAFIN" .
```

#### Eindresultaat Overstort Event op de LDES Server


```

<https://aquafin.be/id/event/cb69ecd5-52a5-459b-88bf-c46d8ed796c0/2025-04-16T14:58:59.625248841>
        rdf:type              <http://www.w3.org/ns/sosa/Event>;
        dct:isVersionOf       <https://aquafin.be/id/event/cb69ecd5-52a5-459b-88bf-c46d8ed796c0>;
        prov:generatedAtTime  "2025-04-16T14:58:59.625Z"^^xsd:dateTime;
        <http://www.w3.org/ns/sosa/event_end_time>
                "2025-04-05T18:15:00.000Z"^^xsd:dateTime;
        <http://www.w3.org/ns/sosa/event_start_time>
                "2025-04-05T18:01:00.000Z"^^xsd:dateTime;
        <http://www.w3.org/ns/sosa/hasFeatureOfInterest>
                <https://aquafin.be/id/meetpunt/P_000000582719>;
        <http://www.w3.org/ns/sosa/madeBySensor>
                <https://aquafin.be/id/sensor/P1035782>;
        <http://www.w3.org/ns/sosa/modified_at>
                "2025-04-06T05:14:26.333Z"^^xsd:dateTime;
        <http://www.w3.org/ns/ssn/status>
                "WerkingOnbekend";
        <https://aquafin.be/ns#is_deleted>
                false .
```
