---
title: ""
date: 2026-02-08
type: landing

design:
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ""
      button:
        text: Download CV
        url: uploads/Xiaoyu_He_CV.docx
    design:
      css_class: dark
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: markdown
    content:
      title: Research Focus
      subtitle: ""
      text: |-
        My research lies at the intersection of causal inference, dynamical systems, and machine learning for biomedical data.

        I am particularly interested in:
        - causal effect estimation from observational data
        - causal graph learning under latent confounding
        - robust modeling of high-dimensional clinical and metabolomics data

        I enjoy collaborations that connect statistical rigor with practical impact.
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: All Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
---
