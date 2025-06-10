---
layout: list
title: "Navigating Data Errors in Machine Learning Pipelines"
subtitle: SIGMOD 2025 Tutorial / Friday, June 27th, 9 AM
summary: |
    Unerliable behavior of machine learning (ML) pipelines is often caused by errors present in the training data. In recent years, the research community has made significant progress in developing holistic approaches to identify the most harmful data errors, prioritize impactful repairs, and reason about their effects when errors cannot be fully resolved. This tutorial surveys prominent work in this area and introduces practical tools designed to address data quality issues across the ML development lifecycle.
# jsonld:
#   type: ResearchProject
#   name: ease.ml
#   alternateName: [ "easeml", "ease ml" ]
#   logo: https://ease.ml/images/easeml-logo.png
thumbnail: images/easeml-logo.png
sections:
    - title: Presenters
      partial: grid
      content:
        page: presenters
        param: pages
      params:
        small: false
        sortBy:
          param: order
    - partial: content
    - title: Literature Survey
      partial: list
      params:
        sortBy:
          param: order
      content:
        page: survey
        param: pages
    - title: Reading List
      partial: list
      content:
        data: publications
      params:
        header:
          field: group
        grouped: true
        showYearAfterVenue: true
        hideVenueTag: true

links:
  - icon: fa-solid fa-file-lines
    href: https://deem.berlin/pdf/icde-tutorial-navigating-data-errors-in-ml-pipelines.pdf
    large: true
    label: Paper
  - icon: fa-solid fa-file-powerpoint
    href: pdf/navigating-data-errors-review-slides.pdf
    large: true
    label: Slides
  - icon: fa-solid fa-laptop-code
    href: https://github.com/navigating-data-errors/tutorial
    large: true
    label: Hands-on
---

## Tutorial Overview

![Navigating Data Errors in ML Pipelines Schematic](images/navigating-data-errors-in-ml-pipelines-schematic.png)

***Key Question:** How should we handle data errors as they get propagated through a complex machine learling pipeline and hurt the quality of downstream predictive queries?*

Addressing data errors — such as missing, incorrect, noisy, biased, or out-of-distribution values — is essential to building reliable machine learning (ML) systems. Traditional methods often focus on refining the training process to minimize error symptoms or repairing data errors indiscriminately, without addressing their root causes. These isolated approaches ignore how errors originate and propagate through the interconnected stages of ML pipelines — data preprocessing, model training, and prediction — resulting in superficial fixes and suboptimal solutions. Consequently, they miss the opportunity to understand how data errors impact downstream tasks and to implement targeted, effective interventions.

In recent years, the research community has made significant progress in developing holistic approaches to identify the most harmful data errors, prioritize impactful repairs, and reason about their effects when errors cannot be fully resolved. This tutorial surveys prominent work in this area and introduces practical tools designed to address data quality issues across the ML lifecycle. By combining theoretical insights with hands-on demonstrations, attendees will gain actionable strategies to diagnose, repair, and manage data errors, enhancing the reliability, fairness, and transparency of ML systems in real-world applications.
