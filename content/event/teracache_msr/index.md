---
title: 'TeraCache: Efficient Caching over Fast Storage Devices'

event: Microsoft Research Cambridge PhD Virtual Workshop on Next-Generation Cloud Infrastructure
event_url: https://www.microsoft.com/en-us/research/event/2021-phd-workshop-on-next-generation-cloud-infrastructure/agenda/

location: Virtual

summary: 
abstract: 
  Many analytics computations are dominated by iterative processing stages,
  executed until a convergence condition is met. To accelerate such workloads
  while keeping up with the exponential growth of data and the slow scaling of
  DRAM capacity, Spark employs o↵-heap caching of intermediate results. However,
  o↵- heap caching requires serialization and deserialization (serdes) of data
  that add significant overhead especially with growing datasets. This thesis
  proposes TeraCache, an extension of the Spark data cache that avoids the need of
  serdes by keeping all cached data on-heap but o↵-memory, using memory-mapped I/O
  (mmio). To achieve this, TeraCache extends the original JVM heap with a managed
  heap that resides on a memory-mapped fast storage device and is exclusively used
  for cached data. Preliminary results show that the TeraCache prototype can speed
  up Machine Learning (ML) workloads that cache intermediate results by up to 37%
  compared to the state-of-the-art serdes approach.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2021-03-24T11:10:00Z'
date_end: '2021-03-24T12:40:00Z'
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
url_slides: ''
url_video: ''
url_poster: 'uploads/teracache_msr.pdf'

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
