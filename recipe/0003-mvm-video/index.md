---
title: Simplest Manifest - Video
id: 3
layout: recipe
tags: [video, presentation]
summary: "The simplest viable manifest for video content. This pattern presents a single video file in a IIIF Presentation resource."
---


## Use Case

The simplest viable manifest for video content. This pattern presents a single video file in a IIIF Presentation resource.

## Implementation Notes

The implementation is identical to the [image example][0001], except that the content is video and the canvas has a duration as well as a height and width.

## Example

This example shows a Manifest with a single Canvas that lasts for 1801 seconds, or just over 30 minutes. It has a single video file (30-minute-clock.mp4) which is associated with it. The mp4 also has a duration of 30 minutes.

{% include manifest_links.html viewers="UV" manifest="manifest.json" %}

{% include jsonviewer.html src="manifest.json" %}

# Related Recipes

* [Simplest Manifest - Image][0001] and [Simplest Manifest - Audio][0002] are equivalent to this example.

{% include acronyms.md %}
{% include links.md %}
