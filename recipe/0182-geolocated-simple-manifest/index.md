---
title: Geolocated Simple Manifest
id: 182
layout: recipe
tags: [maps, geolocate, annotation]
summary: "Geolocate a simple Manifest"
---

### Use Case 
There is a photo taken from an event being encoded as a IIIF Presentation API 3.0 Manifest. I would like to geolocate the Manifest to the event's main building using coordinates.  

### Implementation Notes
* All individual items within the Manifest, as well as the Manifest, are resolvable at the URIs seen in the example.  
* The Manifest used was taken from the [rights](https://github.com/IIIF/cookbook-recipes/issues/8) recipe.  If you have any questions about the Manifest, visit that recipe to learn more. 

### Restrictions
Nested GeoJSON coordinate arrays are incompatible with the processing model of JSON-LD 1.0. The JSON-LD 1.1 processing model does not have this restriction.  

{% include jsonviewer.html src="manifest.json" config='data-line=""' %}

## Related IIIF Stories
* 

## Related Recipes
* [Geolocating Assertion](https://github.com/IIIF/cookbook-recipes/issues/139)

{% include acronyms.md %}
{% include links.md %}