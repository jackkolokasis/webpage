---
title: 'TeraCache: Efficient Caching over Fast Storage Devices'

event: Data and AI Summit Europe'20
event_url: 

location: Virtual

summary: 
abstract: 
  'This talk will introduce TeraCache, a new scalable cache for Spark that avoids
  both garbage collection (GC) and serialization overheads. Existing Spark
  caching options incur either significant GC overheads for large managed heaps
  over persistent memory or significant serialization overheads to place objects
  off-heap on large storage devices. Our analysis shows that: (1) serialization
  increases execution time by up to 30% and (2) caching on the managed heap
  increases GC time by 20%. In addition, these overheads become worse as datasets
  grow.

  <br>
  <br>

  TeraCache eliminates serialization and GC overhead for cached objects. To
  achieve this, TeraCache extends HotSpot JVM’s heap with a managed heap that
  resides on a memory-mapped fast storage device and is exclusively used for
  cached data. To avoid GC over TeraCache, we extend the Java runtime to use
  semantic hints from Spark allocating and freeing cached data objects. We modify
  the collector to not include cached objects, while maintaining safety.
  Preliminary results show that TeraCache can speed up ML workloads by up to 37%
  compared to the supported RDD storage levels.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2020-11-19T11:10:00Z'
date_end: '2020-11-19T12:40:00Z'
all_day: true

# Schedule page publish date (NOT talk date).
publishDate: '2017-01-01T00:00:00Z'

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  #  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
  #  focal_point: Right

links:
  #  - icon: twitter
  #    icon_pack: fab
  #    name: Follow
  #    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: 'uploads/kolokasis_spark_summit_final.pdf'
url_video: 'https://www.youtube.com/watch?v=O1PzEmUJ-X0&t=602s&ab_channel=Databricks'

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
#projects:
#  - example
---
