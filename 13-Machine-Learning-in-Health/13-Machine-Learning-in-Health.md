#  13⋯ Machine Learning in Health

[Modern mathematical machine learning approaches to problems in health and medicine: 

From deep learning to algebraic signal processing](http://www.fields.utoronto.ca/talks/Modern-mathematical-machine-learning-approaches-to-problems-health-and-medicine-deep-learning)

[David Uminsky](), USFCA - University of San Francisco

---

Resources ⋯ Statistical Mathematics / Machine Learning  Medicine

- [Spectral Analysis of the Supreme Court]()
- [Multiclass Total Variation Clustering](https://arxiv.org/pdf/1306.1185.pdf)
- [Google Scholar Platform](https://scholar.google.com/citations?user=ei--1CoAAAAJ&hl=en&oi=ao)

- MATH 340 ⋯ [Differential Equations](https://www.usfca.edu/catalog/course/340-differential-equations) 
  Topics include a review of first-and second-order equations, series solutions, systems of linear and non-linear differential equations, numerical methods, qualitative methods, introduction to partial differential equations
  
- MATH 398 ⋯ Directed Reading and Research 
    - [ ]  2012 - [Probabilistic Programming: Foundations and Applications](http://probabilistic-programming.org/wiki/NIPS*2012_Workshop)
    - [ ]  2008 - [Probabilistic Programming: Universal Languages and Inference; Systems; and Applications](http://probabilistic-programming.org/wiki/NIPS*2008_Workshop)
  
<br>
---

## Abstract


Three different data science approaches will be explored on three very different problems that come from health. In the first problem we consider the prevalent challenge that poisson noise and compression plays in many real world medical imaging problems.  We show that by taking a more generalized approach to traditional activation functions, standard deep learning architectures for computer vision can achieve higher accuracies in fewer epochs for images that exhibit poisson noise and high compression.  In our second example, we consider the challenge of rigorously detecting epistasis in subsets of the genome to understand a specific phenotypic response. We show that using appropriate non-abelian fourier transforms creates   a natural change of basis of the genome that significantly improves our ability to  detect higher order gene interaction for a given phenotypic response.  In the final example, we consider the problem of detecting Atrial Fibrillation in short time ECG recordings.  We show that one can take a topological data analysis (TDA) approach to classification problem that yields comparable results to state of the art deep learning models.

<br>
<br>

## Core Topics

* Activation functions into generalization
* Deep learning CNN architectures 
* Poisson noise and high compression accuracies images with fewer epochs
* Rigorously epistasis detection in subsets genome challenges in specific phenotypic response detection
* Non-abelian Fourier Transforms to  detect higher order gene interaction - phenotypic responses Atrial Fibrillation detection in short time ECG recordings
* Problems in topological data analysis (TDA) classification

<br>
<br>

## Lecture

### A ⌇ Machine Learning

1. Data Science in Health Overview
2. Unsupervised Data Clustering / Learning
* MNIST dataset
3. Activation functions into generalization
4. Deep learning CNN architectures 
5. Balanced Cut Problem Model (NP-hard proof)
``` 
V = {x₁, ... , x𝘕}
```
* k-NN Graph (nearest neighbor)
* Graph weight
```
wᵢⱼ = 𝑒 <sup> -||xᵢ-xⱼ|| 2/2 δ�</sup>
```
* Min Cut Clustering
```
cut(A, Ac) = ∑ i ∈ A, j ∈ A c wij
```
* **Cheeger Cut** & **Normalized Cut** 

<br>

### B ⌇ Poisson Noise & Compression 

1. General Overview
* Non-local
* Dynamical systems
2. TAct 
3. [ReLu]() - NN
* see softmax function, sigmoid function, and tobit model
* Noisy ReLu - gaussian noise & Boltzmann machines
* [Leaky ReLu]()
4. Poisson Noise
* High compression accuracies images with fewer epochs
5. LeNet-5
* Rigorously epistasis detection in subsets genome challenges in specific phenotypic response detection
6. Explicit-Implicit Gradient Flow ALGM

<br>

### C ⌇ Challenges in Medical Imaging

1. General Overview
* Non-AbelianFourier Transforms to  detect higher order gene interaction
* Phenotypic responses Atrial Fibrillation detection in short time ECG recordings
2. Nonlinear Particle Models
3. Non-Abelian
4. Fourier Transform
5. Time-Series
* Partial differential equations
7. [CIFAR]()
8. Fluid Dynamics
9. Topological Data Analysis (TDA) Classification

<!-- br -->

<!--  ## Lecture Material -->

<!-- br -->

<!--
|  Lecture    | [Probabilistic Programming in Machine Learning]() ⌇ Fields ﹊  <sup>28/03/2019</sup> |
| --------- | :--------- |
| [![Placeholder ALT IMG TEXT](http://img.youtube.com/vi/aLFJ5ERxt2c/0.jpg)](https://www.youtube.com/watch?v=aLFJ5ERxt2c&ap=%3D18%2526fmt)        | Probabilistic programs can be used to give compact representations of distributions: in order to represent a distribution, one simply gives a program that would generate an exact sample were the random number generator to produce realizations of independent and identically distributed random variables. This approach to representing distributions by probabilistic programs works not only for simple distributions on numbers like Poissons, Gaussians, etc., and combinations thereof, but also for more exotic distributions on, e.g., phrases in natural language, rendered 2D images of 3D scenes, and climate sensor measurements  |
| Downloads  |  [📼](placeholder) 4.13 GB ⌇ 📄 [PDF](placeholder) 3.87 MB      |
-->

<!-- br -->

<!-- ### Probabilistic Programming *Systems* -->
<!--
Probabilistic programming systems support statistical inference on models defined by probabilistic programs. By constraining some variables of a program (e.g., simulated sensor readings in some climate model) and studying the conditional distribution of other variables (e.g., the parameters of the climate model), we can identify plausible variable settings that agree with the constraints. Conditional inferences like this would allow us to, e.g., build predictive text systems for mobile phones, guess the 3D shape of an object from only a photograph, or study the underlying mechanisms driving observed climate measurements
-->
<!--
Probabilistic programming systems for machine learning and statistics are still in their infancy, and there are many interesting theoretical and applied problems yet to be tackled. My own work focuses on theoretical questions around representing stochastic processes and the computational complexity of sampling-based approaches to inference. I was involved in the definition of the probabilistic programming language [Church](http://projects.csail.mit.edu/church/wiki/Church), and its first implementation, MIT-Church, a Markov Chain Monte Carlo algorithm operating on the space of execution histories of an interpreter. Some of my key theoretical work includes a study of the computability of conditional probability and de Finetti measures, both central notions in Bayesian statistics. Readers looking for an overview of these results are directed to the introduction of my doctoral dissertation. A less technical description of a probabilistic programming approach to artificial intelligence can be found in a recent book chapter on legacies of Alan Turing, co-authored with Freer and Tenenbaum
-->

<br>
<br>

## External Lecture Materials

<br>

| Lecture    | [Multiclass Total Variation Clustering](https://arxiv.org/abs/1306.1185) ⌇ Berkeley ﹊ <sup>05/06/2013</sup> |
| --------- | :--------- |
| [![Multiclass Total Variation Clustering Unsupervised Learning Machine Learning Optimization ](http://img.youtube.com/vi/TFXcVlKqPlM/0.jpg)](https://www.youtube.com/watch?v=TFXcVlKqPlM&ap=%3D18%2526fmt)     |  Many clustering models rely on the minimization of an energy over possible partitions of
the data set. These discrete optimizations usually pose NP-hard problems, however. A
natural resolution of this issue involves relaxing the discrete minimization space into a
continuous one to obtain an easier minimization procedure. Many current algorithms, such
as spectral clustering methods or non-negative matrix factorization (NMF) methods, follow
this relaxation approach. |
| Downloads  | <!-- [📼](https://video.simons.berkeley.edu/2016/logic/1/14-Roy.mp4) 4.13 GB ⌇--> 📄 [PDF](https://arxiv.org/pdf/1306.1185.pdf) 3.87 MB   |

<br>

| Lecture    | [Uncertainty in Computation](https://simons.berkeley.edu/talks/daniel-roy-10-06-2016) ⌇ USF ﹊ <sup>06/10/2016</sup> |
| --------- | :--------- |
| [![Probabilistic Programming](http://img.youtube.com/vi/TFXcVlKqPlM/0.jpg)](https://www.youtube.com/watch?v=TFXcVlKqPlM&ap=%3D18%2526fmt)     | Probabilistic programming is, in the abstract, the study of algorithmic processes that represent and transform uncertainty. In practice, there are many probabilistic programming systems that, to varying degrees of generality and efficiency, allow users to characterize states of uncertainty via probability models and update those models in light of data, either exactly or approximately. I will give a survey of the field and characterize some challenges ahead.  |
| Downloads  |  [📼](https://video.simons.berkeley.edu/2016/logic/1/14-Roy.mp4) 4.13 GB ⌇ 📄 [PDF](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf) 3.87 MB      |


## Resources

1. [Probabilistic Programming](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf)   
2. [A stochastic programming perspective on nonparametric Bayes](http://danroy.org/papers/RoyManGooTen-ICMLNPB-2008.pdf)
3. [Fields-CQAM Interdisciplinary Thematic Program](https://www.eventbrite.ca/e/fields-cqam-interdisciplinary-thematic-program-92001-tickets-51212616314)
4. [Papers with Code](https://paperswithcode.com/task/probabilistic-programming)

