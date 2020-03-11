+++
# Project title.
title = "osbench"

# Date this page was created.
date = 2020-03-11T00:00:00

# Project summary to display on homepage.
summary = "Benchmarking the Ubuntu Operating System"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Systems"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides = "example-slides"

# Links (optional).
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#url_custom = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com/georgecushen"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  #caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

osbench is a micro-benchmark study of analyzing the major set of operations in the Ubuntu operating system. We isolate and perform experiments for four kinds of operations in an operating system - CPU, Memory, Network and File System. Prior to running experiments, we make calculated predictions for each operation based on hardware estimates found in documentations or using our own judgement. We present the results of our experiments and also compare them against our predictions. Overall, the study helped us gain an understanding of the relative performance of different basic operations and will help us identify performance bottlenecks in the systems we build in the future.
