---
layout: default
title: Data voorbeeld
parent: Overstort
nav_order: 1
---

# Data voorbeeld

Volgende JSON structuren worden aangeboden aan de bron:

## Metingen

```json
{
  "type": "Observatie",
  "fenomeentijd": "2024-07-27T14:00:00Z",
  "modifiedAt": "2024-07-29T15:00:00Z",
  "gemetenAfstand": "-10.5",
  "temperatuur": "15",
  "debiet": "0",
  "lat_WGS84": "50.948995878",
  "long_WGS84": "5.298607495000001",
  "lat_Lambert72": "xxx",
  "long_Lambert72": "yyy",
  "overstortstatus": "nietOverstort",
  "validatieStatus": "raw",
  "gebruikteProcedure": "OW19",
  "isWaargenomenMet": "418858"
}
```

## Sensoren

```json
{
  "id": "418858",
  "type": "Sensor",
  "name": "Overstortmeter Ijinus US LTE",
  "familyType": "",
  "owner": "Aquafin",
  "manufacturerName": "ELSCOLAB",
  "serialNumber": "IJA0102-00001836",
  "deviceState": "Actief"
}
```