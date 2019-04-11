# 01 ⋯ Introduction to Machine Learning

[Introductory Topics](http://www.fields.utoronto.ca/talks/Introductory-Topics)

[Roger Grosse](http://danroy.org/)
Assistant Professor of Computer Science, University of Toronto
Founding Member of the Vector Institute

---

Resources ⋯ Publications / Bayesian Learning / STA4516 / Courses

- [Publications on Google Scholar](https://scholar.google.com/citations?user=xgQd1qgAAAAJ&hl=en)
- [Convolutional deep belief networks for scalable unsupervised learning of hierarchical representations](http://people.ee.duke.edu/~lcarin/DeepBelief.pdf) 2009 - 2097 Citations

- CSC 421/2516 ⋯ W 2019 - Neural Networks and Deep Learning
    * [Course Overview / Assignments / Lectures / Tutorials](http://www.cs.toronto.edu/~rgrosse/courses/csc421_2019/) 
    * [Lecture Slides 01](http://www.cs.toronto.edu/~rgrosse/courses/csc421_2019/slides/lec01.pdf): Introduction
- CSC 2541 ⋯ F 2017 - [Scalable and Flexible Models of Uncertainty](https://csc2541-f17.github.io/) 🦑
- CSC 411/2515 ⋯ F 2018 - Machine Learning and Data Mining
    * [Topics in Machine Learning: Scalable and Flexible Models of Uncertainty](https://csc2541-f17.github.io/)
    * [Course Outline / Python Exercises & Tutorials](https://www.cs.toronto.edu/~rgrosse/courses/csc411_f18/)
    * [Lecture Slides 01](http://www.cs.toronto.edu/~rgrosse/courses/csc411_f18/slides/lec01-slides.pdf): Introduction to Machine Learning
    * [Course Syllabus](https://www.cs.toronto.edu/~rgrosse/courses/csc411_f18/syllabus.pdf)
- CSC 321 ⋯ Intro to Neural Networks
    * W 2018 ⋯ [Intro to Neural Networks and Machine Learning](http://www.cs.toronto.edu/~rgrosse/courses/csc321_2018/)
    * F 2018 ⋯ [http://www.cs.toronto.edu/~rgrosse/courses/csc321_2018/](http://www.cs.toronto.edu/~rgrosse/courses/csc321_2018/)
    * W 2017 ⋯ [http://www.cs.toronto.edu/~rgrosse/courses/csc321_2017/](http://www.cs.toronto.edu/~rgrosse/courses/csc321_2017/)
    * W 2015 ⋯ [http://www.cs.toronto.edu/~rgrosse/csc321/](http://www.cs.toronto.edu/~rgrosse/csc321/)

<br>
<br>

## Abstract

This lecture will introduce basic machine learning and deep learning concepts which will be used throughout the course. I’ll briefly review linear regression and classification methods, and then introduce neural networks and the back propagation algorithm.

<br>
<br>
<!-- • -->
## Core Topics

* Topics Overview
* What is ML
* Why ML
* Machine Learning Workflow
* Implementing ML Systems
* Suggested Further Readings


<br>
<br>

## Lecture Notes

#### Topic

1. Sub topic

<br>


#### [Probabilistic Inference]()

A. MEDICAL DIAGNOSIS MODEL DESCRIPTION
1. def model as stochastic inference = `QUERY(diseasesAndSymptoms,checkSymptoms)` 
    * `diseasesAndSymptoms() ` = random | 0
    * `checkSymptoms(...)` feature values checks until match value is reached
2. feature 01: def prior program with `diseasesAndSymptoms()`
    * each 𝑛 = disease, sample an independent binary random variable 𝐷𝑛 with mean 𝑃𝑛
    * 𝐷𝑛 = boolean of 𝑛
e.g.,

| 𝑛 | 𝐷isease | 𝑃𝑛 |
|---|---------|----|
| 1 |Arthritis|0.06|

3. feature 02: .....
    * 𝑚 = symptom
    * 𝑳𝑚 = symptom(𝑚) Patient(𝑳) could have
    * ....

<br>
<br>

## Lecture Materials

<br>

|  Lecture    | [Probabilistic Programming in Machine Learning]() ⌇ Fields ﹊  <sup>28/03/2019</sup> |
| --------- | :--------- |
| [![Placeholder ALT IMG TEXT](http://img.youtube.com/vi/aLFJ5ERxt2c/0.jpg)](https://www.youtube.com/watch?v=aLFJ5ERxt2c&ap=%3D18%2526fmt)        | Probabilistic programs can be used to give compact representations of distributions: in order to represent a distribution, one simply gives a program that would generate an exact sample were the random number generator to produce realizations of independent and identically distributed random variables. This approach to representing distributions by probabilistic programs works not only for simple distributions on numbers like Poissons, Gaussians, etc., and combinations thereof, but also for more exotic distributions on, e.g., phrases in natural language, rendered 2D images of 3D scenes, and climate sensor measurements  |
| Downloads  |  [📼](placeholder) 4.13 GB ⌇ 📄 [PDF](placeholder) 3.87 MB      |

<br>

#### Probabilistic Programming *Systems*

Probabilistic programming systems support statistical inference on models defined by probabilistic programs. By constraining some variables of a program (e.g., simulated sensor readings in some climate model) and studying the conditional distribution of other variables (e.g., the parameters of the climate model), we can identify plausible variable settings that agree with the constraints. 

<br>

#### External Lecture Materials

<br>

| Lecture    | [Uncertainty in Computation](https://simons.berkeley.edu/talks/daniel-roy-10-06-2016) ⌇ Berkeley ﹊ <sup>06/10/2016</sup> |
| --------- | :--------- |
| [![Probabilistic Programming](http://img.youtube.com/vi/TFXcVlKqPlM/0.jpg)](https://www.youtube.com/watch?v=TFXcVlKqPlM&ap=%3D18%2526fmt)     | Probabilistic programming is, in the abstract, the study of algorithmic processes that represent and transform uncertainty. In practice, there are many probabilistic programming systems that, to varying degrees of generality and efficiency, allow users to characterize states of uncertainty via probability models and update those models in light of data, either exactly or approximately. I will give a survey of the field and characterize some challenges ahead.  |
| Downloads  |  [📼](https://video.simons.berkeley.edu/2016/logic/1/14-Roy.mp4) 4.13 GB ⌇ 📄 [PDF](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf) 3.87 MB      |


<br>
<br>

## Resources

1. [Deep Learning](https://www.deeplearningbook.org/)   

2. University of Toronto: Computer Science Department - [Machine Learning](http://www.learning.cs.toronto.edu/courses.html)

3. [Introduction to Machine Learning](https://medium.com/@charliechenyuzhang/introduction-to-machine-learning-ml-e6b43d59b76f), Charlie Chenyu Zhang - Sep 17, 2018
4. Princeton University, COS 324 ⋯ F 2018 - [Introduction to Machine Learning](https://www.cs.princeton.edu/courses/archive/fall18/cos324/)
5. [Understanding Machine Learning:
From Theory to Algorithms](http://www.cs.huji.ac.il/~shais/UnderstandingMachineLearning/), Shai Shalev-Shwartz and Shai Ben-David - 2014
<!-- https://www.cs.huji.ac.il/~shais/UnderstandingMachineLearning/understanding-machine-learning-theory-algorithms.pdf -->
6. Machine Learning and Medicine: [ML Resources](https://sgfin.github.io/learning-resources/), Sam Finlayson with Zak Kohane
7. [Summaries of papers on machine learning](https://github.com/fregu856/papers), Fredrik Gustafsson
8. [Optical Illusion](http://cs229.stanford.edu/proj2006/Bolouki-OpticalIllusion.pdf), Sara Bolouki, Roger Grosse, Honglak Lee, Andrew Ng - 2006
9. [Introducing K-FAC](https://towardsdatascience.com/introducing-k-fac-and-its-application-for-large-scale-deep-learning-4e3f9b443414): A Second-Order Optimization Method for Large-Scale Deep Learning, Kazuki Osawa - Dec 14, 2018
10. [Metacademy](https://metacademy.org/)


