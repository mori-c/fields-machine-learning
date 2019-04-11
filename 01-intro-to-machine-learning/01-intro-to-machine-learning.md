# 01 ⋯ Introduction to Machine Learning

[Machine Learning with Probabilistic Programming](http://www.fields.utoronto.ca/talks/Statistical-learning-theory)

[Dan Roy](http://danroy.org/), University of Toronto
[Gintare Karolina Dziugaite](), University of Toronto

Resources ⋯ Probabilistic Programming / Bayesian Learning / STA4516 / Other

- [Probabilistic Programming](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf)
- [Bayesian Learning](http://fopss18.mimuw.edu.pl/PDF/Roy.pdf)

- STA4516 ⋯ Topics in Probabilistic Programming 
    - [ ]  2015 - [hhttp://danroy.org/teaching/2015/STA4516/](http://danroy.org/teaching/2015/STA4516/)


## Abstract

---

Probabilistic programming systems, like Stan, Church, Anglican, Edward, Pyro, and others, automate statistical inference in probabilistic models defined by probabilistic programs. By constraining some variables of a program (e.g., simulated sensor readings) and studying the conditional distribution of other variables (e.g., model parameters), we can identify plausible explanations for the constrained variables. In this seminar, I will introduce basic principles of probabilistic programming, using a running A.I. example of medical diagnosis. Along the way, students will be exposed to various basic principles of Bayesian inference


## Core Topics

---

•  TOC topics


## Lecture

### Topic

1. Sub topic



---
### [Probabilistic Inference]()

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
4. ....


<br>
<br>

## Probabilistic Programming

<br>

|  Lecture    | [Probabilistic Programming in Machine Learning]() ⌇ Fields ﹊  <sup>28/03/2019</sup> |
| --------- | :--------- |
| [![Placeholder ALT IMG TEXT](http://img.youtube.com/vi/aLFJ5ERxt2c/0.jpg)](https://www.youtube.com/watch?v=aLFJ5ERxt2c&ap=%3D18%2526fmt)        | Probabilistic programs can be used to give compact representations of distributions: in order to represent a distribution, one simply gives a program that would generate an exact sample were the random number generator to produce realizations of independent and identically distributed random variables. This approach to representing distributions by probabilistic programs works not only for simple distributions on numbers like Poissons, Gaussians, etc., and combinations thereof, but also for more exotic distributions on, e.g., phrases in natural language, rendered 2D images of 3D scenes, and climate sensor measurements  |
| Downloads  |  [📼](placeholder) 4.13 GB ⌇ 📄 [PDF](placeholder) 3.87 MB      |

<br>

### Probabilistic Programming *Systems*

Probabilistic programming systems support statistical inference on models defined by probabilistic programs. By constraining some variables of a program (e.g., simulated sensor readings in some climate model) and studying the conditional distribution of other variables (e.g., the parameters of the climate model), we can identify plausible variable settings that agree with the constraints. Conditional inferences like this would allow us to, e.g., build predictive text systems for mobile phones, guess the 3D shape of an object from only a photograph, or study the underlying mechanisms driving observed climate measurements

Probabilistic programming systems for machine learning and statistics are still in their infancy, and there are many interesting theoretical and applied problems yet to be tackled. My own work focuses on theoretical questions around representing stochastic processes and the computational complexity of sampling-based approaches to inference. I was involved in the definition of the probabilistic programming language [Church](http://projects.csail.mit.edu/church/wiki/Church), and its first implementation, MIT-Church, a Markov Chain Monte Carlo algorithm operating on the space of execution histories of an interpreter. Some of my key theoretical work includes a study of the computability of conditional probability and de Finetti measures, both central notions in Bayesian statistics. Readers looking for an overview of these results are directed to the introduction of my doctoral dissertation. A less technical description of a probabilistic programming approach to artificial intelligence can be found in a recent book chapter on legacies of Alan Turing, co-authored with Freer and Tenenbaum


<br>
<br>

## External Lecture Materials

<br>

| Lecture    | [Uncertainty in Computation](https://simons.berkeley.edu/talks/daniel-roy-10-06-2016) ⌇ Berkeley ﹊ <sup>06/10/2016</sup> |
| --------- | :--------- |
| [![Probabilistic Programming](http://img.youtube.com/vi/TFXcVlKqPlM/0.jpg)](https://www.youtube.com/watch?v=TFXcVlKqPlM&ap=%3D18%2526fmt)     | Probabilistic programming is, in the abstract, the study of algorithmic processes that represent and transform uncertainty. In practice, there are many probabilistic programming systems that, to varying degrees of generality and efficiency, allow users to characterize states of uncertainty via probability models and update those models in light of data, either exactly or approximately. I will give a survey of the field and characterize some challenges ahead.  |
| Downloads  |  [📼](https://video.simons.berkeley.edu/2016/logic/1/14-Roy.mp4) 4.13 GB ⌇ 📄 [PDF](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf) 3.87 MB      |


<br>
<br>

## Resources

1. [Deep Learning](https://www.deeplearningbook.org/)   
<!--
2. [A stochastic programming perspective on nonparametric Bayes](http://danroy.org/papers/RoyManGooTen-ICMLNPB-2008.pdf)
3. [Fields-CQAM Interdisciplinary Thematic Program](https://www.eventbrite.ca/e/fields-cqam-interdisciplinary-thematic-program-92001-tickets-51212616314)
4. [Papers with Code](https://paperswithcode.com/task/probabilistic-programming)
-->

