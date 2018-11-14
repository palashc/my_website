+++
# Project title.
title = "Evaluating Druid and Presto"

# Date this page was created.
date = 2018-11-12T00:00:00

# Project summary to display on homepage.
summary = "Studying the design of Druid and Presto and benchmarking them on certain use-cases."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Systems", "Databases"]

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

In recent years, the proliferation of internet technology has created a surge in machine generated events. These events generally have three parts – timestamp, dimensions and metrics. For example – advertising impression data with dimensions like publisher, gender, country etc and metrics like clicks, price etc. Individually these events contain minimal useful information and are of low value. Earlier, companies were willing to discard this data due to the time and resources required to extract any meaning out of it. But now, big data technology such as Hadoop has contributed much to helping companies convert their low value event streams to high value aggregates for a variety of applications.</br></br>However, Hadoop opens our eyes to new problems. Hadoop is a great batch-processing and data warehousing system but it does not make any performance guarantees and its performance degrades under concurrent workload. If a product’s use case needs guarantees around query performance and data availability in a highly concurrent environment, Hadoop is certainly not going to meet the needs. Using an RDBMS like MySQL or Postgres is not an option since data might be stored in a star schema which will lead to operational overhead and table-scan operations (global counts) will be very slow. Another option is to pre-compute aggregates for all possible combinations of dimensions and store them in a key-value NoSQL store. However, the time required to pre-compute aggregates will increase exponentially with the number of dimensions. While working in the Infrastructure Team at Adobe Media Optimizer, I had to evaluate other big data systems for a similar use-case.</br></br>Druid is a distributed column-oriented real-time analytical data store which has a parallelized architecture and is optimized for OLAP workflows.</br></br>Presto is a distributed SQL query engine designed to query large data sets distributed over one or more heterogeneous data sources.
