---
title: "TeraHeap: Reducing Memory Pressure in Managed Big Data Frameworks"
summary: TeraHeap extends the JVM to use a second, high-capacity heap over a fast storage device that coexists with the regular heap. TeraHeap provides direct access to objects on the second heap. It also reduces GC cost by fencing the garbage collector from scanning the second heap. TeraHeap leverages frameworks’ property of choosing specific objects for off-heap placement and offers frameworks a hint-based interface for moving such objects to the second heap.
tags:
  - Java Virtual Machines

date: '2016-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: 'https://github.com/jackkolokasis/teraheap'

#image:
#  caption: Photo by rawpixel on Unsplash
#  focal_point: Smart

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen
url_code: 'https://github.com/jackkolokasis/teraheap'
url_pdf: ''
url_slides: 'uploads/teraheap_asplos23_kolokasis.pdf'
url_video: 'https://www.youtube.com/watch?v=2fSqvkNk07M&ab_channel=ACMSIGARCH'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---


