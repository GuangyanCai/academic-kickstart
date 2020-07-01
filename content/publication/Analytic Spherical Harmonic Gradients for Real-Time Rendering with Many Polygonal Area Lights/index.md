---
title: "Analytic Spherical Harmonic Gradients for Real-Time Rendering with Many Polygonal Area Lights"
authors:
- Lifan Wu
- admin
- Shuang Zhao
- Ravi Ramamoorthi
date: "2020-07-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-07-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: []

# Publication name and optional abbreviated publication name.
publication: ACM Transactions on Graphics (SIGGRAPH 2020), 39(4), July 2020
publication_short: ""

abstract: Recent work has developed analytic formulae for spherical harmonic (SH) coefficients from uniform polygonal lights, enabling near-field area lights to be included in Precomputed Radiance Transfer (PRT) systems, and in offline rendering. However, the method is inefficient since coefficients need to be recomputed at each vertex or shading point, for each light, even though the SH coefficients vary smoothly in space. The complexity scales linearly with the number of lights, making many-light rendering difficult. In this paper, we develop a novel analytic formula for the spatial gradients of the spherical harmonic coefficients for uniform polygonal area lights. The result is a significant generalization, involving the Reynolds transport theorem to reduce the problem to a boundary integral for which we derive a new analytic formula, showing how to reduce a key term to an earlier recurrence for SH coefficients. The implementation requires only minor additions to existing code for SH coefficients. The results also hold implications for recent efforts on differentiable rendering. We show that SH gradients enable very sparse spatial sampling, followed by accurate Hermite interpolation. This enables scaling PRT to hundreds of area lights with minimal overhead and real-time frame rates. Moreover, the SH gradient formula is a new mathematical result that potentially enables many other graphics applications.

# Summary. An optional shortened abstract.
summary: In this paper, we develop a novel analytic formula for the spatial gradients of the spherical harmonic coefficients for uniform polygonal area lights. 

tags: []
featured: true

links:
- name: Code & Data
  url: https://cseweb.ucsd.edu/~liw086/diff-sh-s20/Falcor-diff-sh.zip
url_pdf: http://cseweb.ucsd.edu/~liw086/diff-sh-s20/diff-sh.pdf
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://vimeo.com/429735943'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: []
---

