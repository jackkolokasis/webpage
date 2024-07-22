---
title: Dynamic DRAM Partitioning Between Managed Heap and Page Cache

event: CS446 - Managed Runtime Systems
event_url: https://foivos.zakkak.net/courses/managed-runtime-systems

location: Deprartment of Computer Science, University of Crete, Greece

summary: 
abstract:
  'Popular big data frameworks running on top of managed runtimes must process
  datasets that typically outgrow DRAM capacity. Existing approaches extend the
  managed heap over slow but high-capacity media other than DRAM. The
  state-of-the-art avoids costly garbage collection (GC) scans over the slow
  tier using two managed heaps, one in each tier. They use a DRAM (I/O) cache to
  offer fast access to objects in the slow tier. However, existing systems
  partition DRAM between the DRAM heap and I/O cache statically, requiring tedious
  hand-tuning, which is impractical in real-life deployments and cannot adapt to
  dynamically changing application behavior.

  <br>
  <br>

  This talk presents DynaHeap to address the problem of dynamically dividing a
  fixed DRAM budget between the DRAM heap and I/O cache for the slow tier.
  DynaHeap relies on three concepts:
  (1) it considers GC and I/O costs for periodically (re)partitioning DRAM, 
  (2) it eliminates hand-tuned configurations using an adaptation mechanism that
  maintains a suitable division of DRAM without application knowledge, and  
  (3) it flexibly adapts to applications behavior.

  <br>
  <br>

  We evaluate DynaHeap compared to TeraHeap, a state-of-the-art dual-heap managed
  runtime system, using three real-world analytics frameworks\: Spark, Giraph, and
  GDS-Neo4j. DynaHeap dynamically adjusts to applications memory needs for DRAM
  heap and I/O cache, improving performance compared to TeraHeap. In
  DRAM-constrained datacenter environments in particular, DynaHeap outperforms
  DynaHeap by up to 3.9x.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-04-18T10:00:00Z'
date_end: '2024-04-18T12:00:00Z'
all_day: false

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
url_slides: 'uploads/flexheap_kolokasis_cs446.pdf'
url_video: ''

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
