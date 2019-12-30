---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "SurfStore"
subtitle: "Implementing a Distributed Fault Tolerant stoarge system using RAFT consensus protocol"
summary: ""
authors: []
tags: [Systems]
categories: []
date: 2019-12-29T15:20:45-08:00
lastmod: 2019-12-29T15:20:45-08:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
Getting people to agree on something is hard. Getting machines connected through an asychronous network to agree on something is harder. RAFT is an easy-to-understand consensus protocol which uses leader election and log replication to achieve consensus. In this project, a cloud-based file storage system was built that can survive server failure, datacenter failure, and network failures. Leader election and log replication from the RAFT Consensus protocol were implemented to maintain a consistent state across servers. 
