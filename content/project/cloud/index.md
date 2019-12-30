+++
# Project title.
title = "Comparing Cloud Models"

# Date this page was created.
date = 2019-12-10T00:00:00

# Project summary to display on homepage.
summary = "A comparative study of Virtual Machines, Containers and Serverless"

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
url_pdf = "https://drive.google.com/open?id=15vKo73XY4CEEmMUY8AwPELd8Mhxkh2E9"
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

We performed an in-depth analysis of Virtual Machines, Containers and Serverless using two different CPU-bound and IO-bound applications. We can conclude the following observations from our analysis - (i) Serverless is the most convenient for deploying and maintaining an application closely followed by Containers. The deploy- ment is much slower for Virtual Machines. (ii) For dif- ferent types of workloads, Containers give a better per- formance and scalability compared to Virtual Machines and Serverless. (iii) From a monetary standpoint, Server- less and Containers are cheaper compared to Virtual Ma- chines for smaller workloads, but Containers are the best option for larger workloads. Containers and Virtual ma- chine are more suitable for building services which need to be always online so as to avoid the overhead of load- ing the state in Serverless. Our study and the results have helped us understand the various dimensions of deploy- ing applications in the cloud and we will be able to take an informed decision in the future.
