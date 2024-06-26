---
title: 'Using interactive data visualization to make sense of large datasets'
date: 2022-11-16
permalink: /posts/2022/11/making-sense-of-data/
author_profile: True
toc: True
excerpt_separator: <!--more-->
tags:
  - data
  - analytics
  - terminal
  - bash
  - github
  - git 
  - irods
  - pip
  - python
  - hpc
  - high performance computer
  - programming
  - coding
  - cyverse
  - data
  - science
  - computing
  - soft skills
  - linux
  - data visualization
  - interactive visualization
  - phenomics
  - plant science
---

As sensor technology improves, data volumes grow. We now live in a sea of data collected by our phones, smartwatches, and home assistants like Alexa. Science is not any different, new sensors are enabling the collection of large datasets that can be mined for new scientific discoveries. In plant science, sensor technology is being applied to study how plants grow under drought conditions. 
<!--more-->

---

> **_NOTE:_** Access the workshop notebook [here](https://colab.research.google.com/drive/1qXUkjBhO-1my5SxuUNoYLsgzh5UCzJop?usp=sharing).

# Phenomics: A case study in big data

We will be using data collected by the Field Scanalyzer at the University of Arizona Maricopa Agricultural Center. The Field Scanalyzer covers over an hectare of land - capturing data from over 20,000 plants over a growing season. The Field scanalyzer is equipped with stereo RGB and thermal cameras, a PSII chlorophyll fluorescence imager, and a pair of 3D laser scanners (pictured below). 

<p align="center"><img src="https://github.com/emmanuelgonz/emmanuelgonz.github.io/raw/master/images/bold_gantry_box.png"></p>

Collectively, these sensors capture 20 terabytes (TBs) in a three-month period, which makes converting these raw data into information a difficult task. Accomplishing extraction of information requires leveraging machine learning, high performance computers, and distributed computing.

<p align="center"><img height=500 src="https://github.com/emmanuelgonz/emmanuelgonz.github.io/raw/master/images/file_sizes_swg.png"></p>

These multiple sources of data provide a fine-scale information of plant growth under drought (decreased water) conditions. Today, we will use some of these data to learn interactive visualization using Python!

<p align="center"><img src="https://github.com/emmanuelgonz/emmanuelgonz.github.io/raw/master/images/lettuce_data_examples.png"></p>

---

# Workshop materials

- [Google Colab notebook](https://colab.research.google.com/drive/1qXUkjBhO-1my5SxuUNoYLsgzh5UCzJop?usp=sharing)


---
## Survey

Please provide your feedback to improve future workshops here: [https://bit.ly/2022-ds2f](https://bit.ly/2022-ds2f).

---

## Additional materials

- Seminar invitation
  - [School of Plant Sciences Seminar - Transforming a quarter petabyte of field phenomics data into functional traits and beyond](https://cals.arizona.edu/spls/content/spls-tuesday-seminar-transforming-quarter-petabyte-field-phenomics-data-functional-traits) 
    - Date: Tuesday, 22-Nov 
    - Time: 4pm
    - Zoom link: [https://arizona.zoom.us/j/83941552191](https://arizona.zoom.us/j/83941552191)
    - Password: spls2022

- Reading
  - [Living in Data: A Citizen's Guide to a Better Information Future by Jer Thorp](https://www.amazon.com/Living-Data-Citizens-Better-Information/dp/0374189900)
  - [Data Science by John D. Kelleher and Brendan Tierney](https://arizona-primo.hosted.exlibrisgroup.com/permalink/f/6ljalh/01UA_ALMA51598298120003843)

- Software
  - [PhytoOracle](https://github.com/phytooracle/automation)
    - Data processing pipelines that convert raw data from the Field Scanalzyer into phenotypic trait information
    - To check out our open source code, [click here](https://github.com/phytooracle). 

---

# Acknowledgements

This program is funded by the University of Arizona Libraries: [https://data.library.arizona.edu/ds2f](https://data.library.arizona.edu/ds2f). 

With special thanks to: 
- Jeffrey Oliver
- Megan Senseney
- Jim Martin
- Yvonne Mery
- Leslie Sult
- Cheryl Casey