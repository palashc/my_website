+++
# Project title.
title = "Dense Image Captioning"

# Date this page was created.
date = 2016-12-11T00:00:00

# Project summary to display on homepage.
summary = "Teaching a computer vision system to localize and describe salient regions in images in natural language"

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
url_pdf = "https://drive.google.com/open?id=1vwUJx41TDZQJmcp0bBdlWgGMCKPHJy24"
url_slides = "https://drive.google.com/open?id=12rKhMdrLOJKHDKhW4r57HqHveb5JHoSA"
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

Dense captioning is a task which requires a computer vision system to both localize and describe salient regions in images in natural language. The dense captioning task generalizes object detection when the descriptions consist of a single word, and Image Captioning when one predicted region covers the full image. "DenseCap: Fully Convolutional Localization Networks for Dense Captioning" by Karpathy et. al. proposed a Fully Convolutional Localization Network (FCLN) architecture that processes an image with a single, efficient forward pass, requires no external regions proposals, and can be trained end-to-end with a single round of optimization. The architecture is composed of a Convolutional Network, a novel dense localization layer, and Recurrent Neural Network language model that generates the label sequences. </br>In this project, we tried two things. First was to reproduce the results obtained by the authors to get familiar with the codebase. Second, we replaced the test time Non-Maximal Supression with a Tyrolean Network as described in "A convnet for non-maximum suppression" by Hosang et. al. We were able to obtain a slight increase in the Mean Average Precision of DenseCap compared to our run of the original code.
