---
title: 'GateKeeper: Transparent Placement of Big Data Objects in Hybrid Managed Heaps'

event: 18th EuroSys Doctoral Workshop (EuroDW '24)
event_url: https://2024.eurosys.org/euroDW.html

location: Athens, Greece

summary: 
abstract:
  Popular big data frameworks running on top of managed runtimes must process
  datasets that typically outgrow DRAM capacity. Existing approaches extend the
  man- aged heap over slow but high-capacity media other than DRAM, such as NVMe
  SSDs. The state-of-the-art avoids costly garbage collection (GC) scans over the
  slow tier using two managed heaps, one in each tier. They use a DRAM (I/O) cache
  to offer fast access to objects in the slow tier. Nevertheless, these systems
  encounter signif- icant hurdles in determining which objects to migrate to the
  slow tier. One approach within existing systems relies on programming models or
  hints, demanding additional user effort and necessitating the rewriting of
  legacy frameworks, which is impractical in real-life deployments. An
  alternative category of systems identifies, transparently at runtime, the
  objects to move to the slow tier based on their object hotness. However, these
  solutions require costly code instrumentation, leading to a slowdown in
  application performance.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-04-22T15:15:00Z'
date_end: '2024-04-22T15:30:00Z'
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
url_slides: 'uploads/gatekeeper_kolokasis_eurodwl.pdf'
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
