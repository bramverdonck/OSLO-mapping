---
layout: default
title: Stap voor stap
parent: Overstort
nav_order: 3
---

# Intro

Voor het mappen van de JSON naar JSON-LD volgens OSLO wordt gewerkt in 2 stappen.

Eerst gebeurt een rudimentaire omzetting naar Linked Data door een basis JSON-LD context toe te voegen.

Daarna gebeurt een omzetting naar OSLO via SPARQL Construct query.

# Voorbeeld bruto vracht observatie water 

## Ruwe data

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

## Intermediate mapping

Om de intermediate mapping te doen, wordt de JSON verrijkt met een default JSON-LD context:
```json
  {
    "@context": {
      "@vocab": "https://aquafin.be/ns#"
    }
  }
```

## OSLO mapping

Op basis van de intermediate omzetting kan vervolgens een OSLO mapping uitwerkt worden adhv SPARQL CONSTRUCT queries. 

### SPARQL CONSTRUCT

Bovenstaande JSON-LD wordt dan gebruikt in de SPARQL construct:

```
CONSTRUCT {
  ...
} WHERE {
  
}
```


## Pipeline

cd pipeline
docker-compose up -d

# send the message
curl  -X POST 'http://localhost:9004/metingen-pipeline-raw' --header 'Content-Type: application/json' --data-binary  @./metingen.json