+++
# Project title.
title = "Serverless Networking"

# Date this page was created.
date = 2020-03-11T00:00:00

# Project summary to display on homepage.
summary = "Using UDP hole-punching for Serverless Communication"

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

Serverless is an emerging paradigm for the deployment of applications and services, influenced by the recent shift towards containers and microservices. Serverless function provides a simplified programming model for creating cloud applications and abstracts away most of the operational concerns. However, it lacks one important component needed to unlock its complete potential - communication. In the latest offering of Function-as-a-Service platform, two serverless functions can only communicate with each other through an intermediary storage service like S3 since the functions are not directly network-addressable. This approach is slower and adds extra cost for the cloud consumer. In this project, we explore an alternative means to achieve serverless communication - NAT Hole Punching. We analyze the feasibility of the approach for various scenarios of serverless function placement in the context of AWS network infrastructure, and evaluate the mechanism on some micro- and macro-benchmarks.