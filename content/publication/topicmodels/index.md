+++
title = "Application Tool Recommendation"
date = 2017-03-01T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Palash Chauhan", "Aditya Gupta", "Naman Jain", "Sanjeev Biswas"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
#publication_types = ["0"]

# Publication name and optional abbreviated version.
publication = ""
publication_short = ""

# Abstract and optional shortened version.
abstract = "Computing application range significantly in their perceived complexity. Some applications are immediately intuitive. Most of the users might be able to leverage the functionality of these applications when first exposed to them without much instruction. Other application, however, may require some amount of prior knowledge, learning or experimentation. Such applications have an abundance of functionality buried in menus, accessible through particular dialogs, initiated by particular keyboard shortcuts and so forth. Adobe Creative Cloud products such as Photoshop and llustrator are prime examples of such applications. Cancellation rates are the highest in the first 30-60 days when users are onboarding indicating difficulty in usage. Conventional techniques of informing the users about the functionality of the application involve enabling users to search for the desired functionality and obtain articles/videos which demonstrate the usage of tools. Providing information this way, however, places the responsibility of obtaining the information on the user itself. This may seem tedious to most users and lead to frustration and finally in cancellation of a subscription.<br/><br/>To tackle this issue, we propose a system for contextual prediction of user actions in such applications and a method to surface relevant user guidance in the form of text/images/videos relevant to the context in which the user is working. We make an analogy where a user session is seen as a document and the actions taken by the user in a string format are the words. We then model huge volume of user session data using a Topic Model (LDA: Latent Dirichlet Allocation). The extracted topics, which are nothing but distributions over the set of application tools (or subsets of tools considering the top-k tools), can then be interpreted with the help of an expert. The topics are equivalent to ‘sub-workflows’ in an entire user workflow. For example a user working in Illustrator might work with shapes or with text or with images, all of which could be different topics with different set of tools defining them. We also propose a sliding window approach to detect which topic the current user workflow belongs to. Using this approach we build a topic-transition model which can then be used in a live user session to identify what the user is trying to do and surface relevant guidance information. We show that predicting the next few topics the user might move to is more helpful than just predicting the next few tools the user might use.  The entire approach can also be extended to achieve a user-base segmentation and tool analysis."
abstract_short = ""

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides = "example-slides"

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["Machine Learning", "Big Data Analysis", "Topic Models", "Adobe Creative Cloud"]

# Links (optional).
url_pdf = ""
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = "https://patents.google.com/patent/US20180260718A1/"
url_slides = "https://drive.google.com/open?id=1MpPBGYHO4OUURfVZEQVGC5KnOagsqaZQ"
url_video = "https://drive.google.com/open?id=1g0DWmAWe3GqHszaRjaEhLJnBtEwh025K"
url_poster = ""
url_source = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
# url_custom = [{name = "Custom Link", url = "http://example.org"}]

# Digital Object Identifier (DOI)
doi = ""

# Does this page contain LaTeX math? (true/false)
math = true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
+++

