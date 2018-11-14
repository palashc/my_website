+++
# Project title.
title = "Load Value Prediction"

# Date this page was created.
date = 2017-05-12T00:00:00

# Project summary to display on homepage.
summary = "Predicting values loaded by machine intructions to aid Instruction Level Parallelism."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Systems", "Computer Architecture"]

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
url_pdf = "https://drive.google.com/open?id=1-FYNd5kLepy0Y7HFcafHNDcnEugw6R8U"
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

Data dependencies can severely hinder Instruction Level Parallelism (ILP). Data dependencies decrease ILP when long latency instructions flow through the pipeline, and there are not enough independent instructions available to keep the processor busy. Data dependent instructions will stall behind these long latency instructions, potentially creating one or several critical paths through a portion of the program. Load Value Prediction (LVP) is an approach that breaks data dependency on load instructions by predicting the value which is fetched by the instruction. LVP exploits value locality which can be defined as the likelihood of a previously-seen value recurring repeatedly within a storage location. In this project, we explore this notion of value locality, exploit it in order to perform load value prediction and analyze the performance on SPEC2006 Benchmarks.