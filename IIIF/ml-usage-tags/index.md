---
title: IIIF ML/AI Usage Tags Recipe
id: 
layout: recipe
tags: [rights, requiredStatement]
summary: "Ethical ML/AI Use Tags for IIIF Manifests"
viewers:
 - Mirador
 - UV
topic: 
 - text
 - presentation
property: rights, requiredStatement   
---

## Use Case

## Implementation Notes


For humans, within [`requiredStatement`](https://iiif.io/api/presentation/3.0/#requiredstatement)

  `"label": { "en": [ "No AI" ] },
  "value": { "en": [ "Material related to this IIIF Manifest should not be used for AI or ML  
  training datasets." ] }` 

  `"label": { "en": [ "No Image AI" ] },
  "value": { "en": [ "Image-based material related to this IIIF Manifest should not be used for 
  AI or ML training datasets." ] }`

  `"label": { "en": [ "Regulated ML/AI Use Permitted - Attribution Required" ] },
  "value": { "en": [ "Material related to this IIIF Manifest may be used for AI or ML training 
  datasets, as long as Standard Attribution of source content is maintained for the ML/AI 
  dataset. Original URL of source IIIF manifest must be maintained and referenced." ] }`

  `"label": { "en": [ "Regulated ML/AI Use Permitted - Consent Required" ] },
  "value": { "en": [ "Material related to this IIIF Manifest may be used for AI or ML training   
  datasets, if Prior Written Consent is obtained from the source holding institution. Standard 
  Attribution of source content must be maintained for the ML/AI dataset. Original URL of 
  source IIIF manifest must be maintained and referenced." ] }`


For machines, within [`rights`](https://iiif.io/api/presentation/3.0/#rights)

* URIs to be pursued for machineable interactions


## Restrictions

No known restrictions.

## Example

{% include manifest_links.html manifest="manifest.json" %}

{% include jsonviewer.html src="manifest.json" config='data-line="31-89"' %}

The direct link to the fixture is a useful convenience.

## Related Recipes

* [Rights][0008] for demonstrating use of `rights` and `requiredStatement`
