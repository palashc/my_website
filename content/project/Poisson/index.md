+++
# Project title.
title = "Poisson Matrix Factorization"

# Date this page was created.
date = 2017-04-10T00:00:00

# Project summary to display on homepage.
summary = "Probabilistic Models for Bayesion Recommender Systems."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Bayesian ML", "Machine Learning"]

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
url_pdf = "https://drive.google.com/open?id=1aGCl84QsoHGmNDyFqewWcqqlYl9Zx1LY"
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

Recommendation systems are a vital component of the modern web. They help readers effectively navigate otherwise
unwieldy archives of information and help websites direct users to items - movies, articles, songs, products that they
will like. Collaborative filtering is one of the techniques used for building recommendation systems which involves
inferring user preferences and item attributes from data. </br> In this project, I studied various models for Bayesian Recommender Systems including Poisson Matrix Factorization and its extensions like Hierarchical Poisson Matrix Factorization and Bayesian Non-parametric Poisson Matrix Factorization. I analyzed the effect of latent dimensions on the models and learnt the use of auxiliary variables in variational inference to make the models locally conjugate and facilitate inference. I also evaluated their performance on MovieLens 1M dataset.