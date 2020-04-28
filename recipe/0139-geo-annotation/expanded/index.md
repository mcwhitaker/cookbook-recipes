---
title: Geographical Assertion Annotation 
id: 999
layout: recipe
tags: [maps, geocode, annotation]
summary: "Make a geographical assertion about the word Paris in some transcription text."
---

### Use Case
A correspondence between friends in Paris was discovered.  There is the desire to link all mentions of 'Paris' to Paris, France. 

### Implementation Notes
* `geocode` was used as the motivation throughout. The IIIF-Maps group is working on proper motivation extensions for the various kinds of assertions that could be made. The three main categories are `geocode`, `georeference` and `co-locate`.
* GeoJSON `properties` is a very generic field and [can be nearly anything](https://tools.ietf.org/html/rfc7946#section-3.2). If, for example, the targeted resource has a `label` and the `properties` field contains a `label`, the consuming interface must make a choice on which to preference for presentation purposes. This community should establish conventions to inject, override or extend resource properties.
* [`geometry` can be more than just a `Point`.](https://tools.ietf.org/html/rfc7946#section-3.1)


### The Canvas containing a jpeg for which transcription text was written which has the word 'Paris' in the transcription text is geocoded to Paris, France.  
[JSON-LD](canvas.json)

{: .line-numbers data-download-link data-download-link-label="Download me" data-src="canvas.json" }
```json
```

# Break-Down Of The Important Parts
### The Canvas Content
[JSON-LD](contentPage.json)

{: .line-numbers data-download-link data-download-link-label="Download me" data-src="content.json" }
```json
```

### The Canvas Supplementing Data to further describe the content
[Text](supplementingPage.json)

{: .line-numbers data-download-link data-download-link-label="Download me" data-src="supplementingPage.json" }
```json
```

### The geocoding Annotation which geocodes the supplemeting transcription text.  
[JSON-LD](geoAnno.json)

{: .line-numbers data-download-link data-download-link-label="Download me" data-src="geoAnno.json" }
```json
```

## Related IIIF Stories
* [https://github.com/IIIF/iiif-stories/issues/116](https://github.com/IIIF/iiif-stories/issues/116)
* [https://github.com/IIIF/iiif-stories/issues/119](https://github.com/IIIF/iiif-stories/issues/119)
* [https://github.com/IIIF/iiif-stories/issues/125](https://github.com/IIIF/iiif-stories/issues/125)
* [https://github.com/IIIF/iiif-stories/issues/135](https://github.com/IIIF/iiif-stories/issues/135)

## Related Recipes
* [0TBD]()
* [0TBD]()
* [0TBD]()

{% include acronyms.md %}
{% include links.md %}