# 04 ⋯ Probabilistic Models

[Machine Learning with Probabilistic Programming](http://www.fields.utoronto.ca/talks/Statistical-learning-theory)

[Dan Roy](http://danroy.org/), University of Toronto
[Gintare Karolina Dziugaite](), University of Toronto

Resources ⋯ STA4516

- STA4516 ⋯ Topics in Probabilistic Programming 
    - [ ]  2015 - [hhttp://danroy.org/teaching/2015/STA4516/](http://danroy.org/teaching/2015/STA4516/)
    - [ ]  2012 - [Probabilistic Programming: Foundations and Applications](http://probabilistic-programming.org/wiki/NIPS*2012_Workshop)
    - [ ]  2008 - [Probabilistic Programming: Universal Languages and Inference; Systems; and Applications](http://probabilistic-programming.org/wiki/NIPS*2008_Workshop)


## Abstract

---

Probabilistic programming systems, like Stan, Church, Anglican, Edward, Pyro, and others, automate statistical inference in probabilistic models defined by probabilistic programs. By constraining some variables of a program (e.g., simulated sensor readings) and studying the conditional distribution of other variables (e.g., model parameters), we can identify plausible explanations for the constrained variables. In this seminar, I will introduce basic principles of probabilistic programming, using a running A.I. example of medical diagnosis. Along the way, students will be exposed to various basic principles of Bayesian inference


## Core Topics

---

•  Probabilistic programmig basic principles
    e.g., A.I. medical diagnosis example
•  Bayesian inference principles
•  Automate statistical inference
•  Probabilistic models
•  Probabilistic programs
╰  constraining variables
      e.g., simulated sensor readings
╰  conditional distribution variables
      e.g., model parameters
•  Probabilistic programming systems:
╰  Stan
╰  Church (language)
╰  Anglican
╰  Edward
╰  Pyro


## Lecture

1. Baysian Learning
* limitation in frequency
* **representing** *degree of belief*
* Probabilities are *personal*, reflection of factors, observations, past assumptions tested to predict
* key structures of *joint distributions* of multiple random variables
    X = pa
    Y
    Z
    S
    W
    ℙ { X = x, Y = y, Z = z, S =s, W = w}
    * extension of logic
    * booleans
    * inferences
* Learning to classify, predict from conditions
    
2. Bayesian Inference <sup>*fully Bayesian*</sup>
* θ* = unknown quantities, modelled as random prior distribution
* everything is a random variable = frequent sampling properties = seeking a remainder
    
3. Universial Stochastic Inferences
* Computational Object Framework
    * **programs** = distributions 
    - programs taking programs
    - programs represented as simulators  
    * **predicates** = evidence
    * **procedure** = conditioning from high order

4. Computational Frameworks
* Probabilistic Programming
* ABC - Approxi Bayseian Computation
* Implicit Generative Models

5. Computational Tutorial
* **Query** = prob model as **programs**



#### March 2019

#### October 6th, 2016

[Uncertainty in Computation](https://simons.berkeley.edu/talks/daniel-roy-10-06-2016)
![A Personal View of Probabilistic Programming](https://www.youtube.com/watch?v=TFXcVlKqPlM)[⬇️ ](https://video.simons.berkeley.edu/2016/logic/1/14-Roy.mp4) 4.13 GB

Probabilistic programming is, in the abstract, the study of algorithmic processes that represent and transform uncertainty. In practice, there are many probabilistic programming systems that, to varying degrees of generality and efficiency, allow users to characterize states of uncertainty via probability models and update those models in light of data, either exactly or approximately. I will give a survey of the field and characterize some challenges ahead.

📄 [PDF](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf) 3.87 MB




## Probabilistic Programming

Programs can be used to give compact representations of distributions: in order to represent a distribution, one simply gives a program that would generate an exact sample were the random number generator to produce realizations of independent and identically distributed random variables. This approach to representing distributions by probabilistic programs works not only for simple distributions on numbers like Poissons, Gaussians, etc., and combinations thereof, but also for more exotic distributions on, e.g., phrases in natural language, rendered 2D images of 3D scenes, and climate sensor measurements


### Probabilistic Programming *Systems*

Probabilistic programming systems support statistical inference on models defined by probabilistic programs. By constraining some variables of a program (e.g., simulated sensor readings in some climate model) and studying the conditional distribution of other variables (e.g., the parameters of the climate model), we can identify plausible variable settings that agree with the constraints. Conditional inferences like this would allow us to, e.g., build predictive text systems for mobile phones, guess the 3D shape of an object from only a photograph, or study the underlying mechanisms driving observed climate measurements

Probabilistic programming systems for machine learning and statistics are still in their infancy, and there are many interesting theoretical and applied problems yet to be tackled. My own work focuses on theoretical questions around representing stochastic processes and the computational complexity of sampling-based approaches to inference. I was involved in the definition of the probabilistic programming language [Church](http://projects.csail.mit.edu/church/wiki/Church), and its first implementation, MIT-Church, a Markov Chain Monte Carlo algorithm operating on the space of execution histories of an interpreter. Some of my key theoretical work includes a study of the computability of conditional probability and de Finetti measures, both central notions in Bayesian statistics. Readers looking for an overview of these results are directed to the introduction of my doctoral dissertation. A less technical description of a probabilistic programming approach to artificial intelligence can be found in a recent book chapter on legacies of Alan Turing, co-authored with Freer and Tenenbaum



## Course Materials

[📼]() Lecture
[📄]() Slides


- Table of Contents
    1. 
