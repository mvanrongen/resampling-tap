--- 
title: "CamStats - TAP"
author: "Martin van Rongen"
date: "2022-05-13"
site: bookdown::bookdown_site
documentclass: book
#bibliography: [book.bib, packages.bib]
# url: your book url like https://bookdown.org/yihui/bookdown
# cover-image: path to the social sharing image like images/cover.jpg
description: "These are the materials used as a course design for the Teaching Associate's Programme, Cambridge University. They are an adaptation of the materials I developed for the CamStats series of statistics." 
---



# Overview

Statistical courses are often taught in a way that focuses on the underlying mathematics. That approach may work well in some situations, particularly where a certain level of theoretical knowledge is required.

However, when it comes to using statistics in research, this theoretical approach can show some shortcomings. A large proportion of post-graduate students who receive training via the Bioinformatics Training Facility do not have a strong mathematical background, which means that they often struggle with the statistical topics that have been taught during their undergraduate years. As a result, students tend to follow the statistical methods that are generally used in the journal within their respective fields, without really understanding _why_ or questioning the suitability of these methods.

The materials on resampling techniques are part of a larger series of statistical topics that tries to remedy this. All of these sessions are delivered as a lecture-practical. In each 40-60 minute lecture the underlying principles of the topic is discussed, using examples and practical applications. Discussion with students is encouraged by asking questions - often by asking for opinions and experiences, rather than testing specific knowledge.

This approach encourages students to engage and think about the wider context of what they are doing and why.

### Assessment
Assessment of individual progress occurs through ongoing formative assessment exercises, rather than a formal assessment. The focus of the course is very much on encouraging an **intuitive understanding** of the underlying principals, rather than a mathematical one. As such, there are no mathematical derivations (and definitely no pen and paper calculations!).

### Evaluation
All of the course within the Bioinformatics Training Facility get surveyed using `surveymonkey` surveys. The exact content of the surveys is too large to cover here, but with these surveys we for example gain insight on how participants engage with the course materials - both during and after the course. We also assess after six months if they have used the knowledge they've gained in their own research.

A less formal way of assessing how participants engage with the materials is through their questions in a shared Q&A document that gets used during the course. Usually if questions are technical in nature I can tell that participants are focusing on the practical implementation of the coding. Although this is understandable, particularly during early sessions, the aim is get participants to ask questions that are at a deeper level, for example asking for reasons why certain techniques are used, or volunteering if alternative techniques are also valid. This shows me that participants are thinking beyond what they're learning - often relating it to the context of their own research.

A second informal way of gauging engagement with the materials is the number of questions I get during and after the course about their own data. People often contact me to ask if a certain analysis technique that they've tried on their own research data is correct, or they ask questions on how to apply some of the covered topics to their own research. To me this is the most relevant learning outcome: using the knowledge they've gained to better their own research.

## Core aims
The general learning outcomes for these sessions is two-fold:

:::highlight
1. Have an intuitive understanding of the statistical techniques
2. Be able to apply these techniques appropriately to their own research data, using R
:::

## Datasets {#index-datasets}

This course uses various data sets. The easiest way of accessing these is by creating an R-project in RStudio. Then download the `data` folder [here](camstats_data.zip) by right-clicking on the link and <kbd>Save as...</kbd>. Next unzip the file and copy it into your working directory. Your data should then be accessible via `<working-directory-name>/data`.

:::note
The practicals have "tabs" that show _tidyverse_. This is because the materials are developed in parallel by using R syntax that uses _tidyverse_, base R and Python. For the purpose of this draft, a few examples for base R are included.

The rationale behind providing three distinct programmatic ways of performing these techniques is to encourage participants to focus on understanding the statistics and not the programming language. By offering three different programming syntax participants can choose whatever syntax they are most comfortable with.

The materials also limit the use of colours to ones that are colourblind friendly. This is to encourage participants to consider their use of colours when creating their own figures (discussed throughout the course).
:::
