# The Relationship Between Music Preferences and Mental Health


Mükerrem Mina Tanısa, DSA210 Term Project, Fall 2025-2026


## Motivation and Overview

As it is suggested by many scientific research, and from our daily lives, we know music plays a vital role in **stress reduction** and **emotional regulation**. It can also be said that different genres of music can have distinct psychological impact on us, for example:

* *Classical* or *Lo-Fi* music are often linked to relaxation; we listen them when we are studying, trying to focus or just relax.
* *Heavy Metal* or *Rap* music in the other hand may increase arousal and stress, or they may boost our mood depending on the conditions.

In this project I aim to explore whether **musical preferences** can serve as a **non-clinical indicator of mental health** by analyzing self-reported survey data gathered from Kaggle. Below you may find the detailed dataset description.

---

## Dataset Overview

**Dataset:** `mxmh_survey_results.csv`
**Source:** [Kaggle - Music & Mental Health Survey](https://www.kaggle.com)
**Size:** around 1,000 responses

| **Category**          | **Columns**                                                                                         | **Description**                                 |
| --------------------- | --------------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| **Demographics**      | `age`, `primary_streaming_service`                                                                  | Age and preferred music platform                |
| **Listening Habits**  | `hours_per_day`, `while_working`, `instrumentalist`, `composer`, `exploratory`, `foreign_languages` | Frequency and context of music listening        |
| **Music Preferences** | `fav_genre`, plus genre frequency columns (`pop`, `jazz`, `rock`, etc.)                             | Primary and secondary genre choices             |
| **Mental Health**     | `anxiety`, `depression`, `insomnia`, `OCD`                                                          | Self-reported indicators (`Yes/No/Sometimes`)   |
| **Qualitative Field** | `music_effects`                                                                                     | Textual reflections on music’s emotional impact |

---

## Data Preparation & Cleaning

Before continuing with **EDA**, the dataset will be carefully reviewed to ensure the accuracy of the values. Missing and/or inconsistent data entries will be handled, cleaned; which may also include unrealistic responses such as extreme values since the data is build upon a self-reporting survey. Categorical answers will also be converted to respective numerical values to prepare the data for better comparison and applying **Machine Learning** techniques. Some other standardizations can be done to ensure a clean and reliable dataset for meaningful **EDA** and **ML** practices.

---

## Exploratory Data Analysis (EDA)

I will conduct EDA after preparing and cleaning the data.

**EDA includes:**

* Age, gender, and listening hours distributions
* Most common genres and platforms
* Average depression/anxiety rates by genre
* Correlation heatmap between variables
* Boxplots: listening hours vs. mental health
* And more...

**Libraries:**
The data analysis and ML applications will require roughly the following libraries of Python:
`pandas`, `matplotlib`, `seaborn`, `numpy`

---

## Hypothesis Testing

I will test hypotheses such as, but not limited to:

### Example Hypotheses
---
* **H₀:** There is no relationship between music genre and depression level.
* **H₁:** Listeners of *classical* or *lo-fi* music have lower anxiety than *metal* or *rap* listeners.
---
* **H₀:** There is no relationship between daily music listening time and reported insomnia levels.
* **H₁:** People who listen to music for **longer** daily durations are **more** likely to report insomnia symptoms.
---

## Expected Findings

* Certain genres (*classical*, *lo-fi*) may associate with **lower anxiety**.
* High listening hours might correlate with **sleep issues (insomnia)**.
* Gender and age could **moderate** mental health effects.
* And more to be discovered...

---

## Limitations & Future Work

* Self-reporting may be biased, and missing demographic biase values may limit the analysis.
* Future directions:

  * Integrate **Spotify API** for real-time listening data
  * Include, and combine **physiological datasets** for deeper insight

---
*This document was formatted including the help of ChatGPT for readability purposes.*
