+++
# Project title.
title = "Automatic Abstract Generation"

# Date this page was created.
date = 2016-12-10T00:00:00

# Project summary to display on homepage.
summary = "Text Summarization for Long Documents like research papers."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Deep Learning", "Machine Learning"]

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
url_pdf = "https://drive.google.com/open?id=1u5Ij8_uaoPntL53i5Oe9VunV8DnTnXJP"
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

As the problem of information overload grows, and as the amount of data increases, the interest in automatic summarization is also increasing. There has been a lot of reserach work in the area of text summarization. Summarization can be achieved either by extracting elements from the input (Extractive) or by understanding the content of the input and using language generation techniques (Abstractive).
Both these methods do not perform well on long documents like research papers. Through this project, we proposed an approach for automatic summarization which is a combination of both these methods. Salient sentences are first extracted from the long document which are then fed to a sequence-to-sequence RNN. We experimented with a number of ways to extract salient elements like LDA, LSA and TextRank and fed the best extraction to an RNN to generate an enhanced summary. We evaluated the generated summaries using the ROUGE metric on a dataset containing research papers from NIPS 2015.