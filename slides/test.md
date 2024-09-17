---
marp: true
theme: gaia
_class: lead
paginate: false
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---

![bg left:40% 80%](../logo.png)

# **Feature Engineering**

## The Machine Learning Fundamentals

---

# What is machine learning?
Machine learning fits mathematical models to data in order to derive insights or make predictions. 

>[Machine Learning is the] field of study that gives computers the ability to learn without being explicitly programmed.
>    —Arthur Samuel, 1959

These models take **features** as input. A feature is a numeric representation of an aspect of raw data. 
<!--
Features are used as input variables in models that learn from data to make predictions or decisions without being explicitly programmed.
-->
---
# Feature engineering
Feature engineering is the act of extracting features from raw data and transforming them into formats that are suitable for the machine learning model. It is a crucial step in the machine learning pipeline, because the right features can ease the difficulty of modeling, and therefore enable the pipeline to output results of higher quality.

---
# Machine Learning is great for:
- Problems for which existing solutions require a lot of hand-tuning or long lists of rules: one Machine Learning algorithm can often simplify code and perform better.
- Complex problems for which there is no good solution at all using a traditional approach: the best Machine Learning techniques can find a solution.
- Fluctuating environments: a Machine Learning system can adapt to new data.
- Getting insights about complex problems and large amounts of data.

---
## The Machine Learning Pipeline

* **Data**: What we call data are observations of real-world phenomena. 
<!--
Each piece of data provides a small window into a limited aspect of reality. The collection of all of these observations gives us a picture of the whole. But the picture is messy because it is composed of a thousand little pieces, and there’s always measurement noise and missing pieces.
-->
* **Models**: A mathematical model of data describes the relationships between different aspects of the data. 
<!--
  For instance, a model that recommends music might measure the similarity between users (based on their listening habits), and recommend the same artists to users who have listened to a lot of the same songs.
  -->
* **Features**: A feature is a numeric representation of raw data. 
<!--
There are many ways to turn raw data into numeric measurements, which is why features can end up looking like a lot of things. Naturally, features must derive from the type of data that is available. 
-->

---

Some models are more appropriate for some types of features, and vice versa. The right features are relevant to the task at hand and should be easy for the model to ingest. **Feature engineering** is the process of formulating the most appropriate features given the data, the model, and the task.

---


