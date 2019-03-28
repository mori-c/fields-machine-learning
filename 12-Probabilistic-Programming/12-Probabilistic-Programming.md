# 04 ⋯ Probabilistic Models

[Machine Learning with Probabilistic Programming](http://www.fields.utoronto.ca/talks/Statistical-learning-theory)

[Dan Roy](http://danroy.org/), University of Toronto
[Gintare Karolina Dziugaite](), University of Toronto

Resources ⋯ STA4516

- STA4516 ⋯ Topics in Probabilistic Programming 
    - [ ]  2015 - [hhttp://danroy.org/teaching/2015/STA4516/](http://danroy.org/teaching/2015/STA4516/)
    - [ ]  2012 - [Probabilistic Programming: Foundations and Applications](http://probabilistic-programming.org/wiki/NIPS*2012_Workshop)
    - [ ]  2008 - [Probabilistic Programming: Universal Languages and Inference; Systems; and Applications](http://probabilistic-programming.org/wiki/NIPS*2008_Workshop)
- [Towards common-sense reasoning via conditional simulation: legacies of Turing in Artificial Intelligence](https://arxiv.org/pdf/1212.4799)
- [TOWARDS COMMON-SENSE REASONING VIA CONDITIONAL SIMULATION: LEGACIES OF TURING IN ARTIFICIAL INTELLIGENCE](http://danroy.org/papers/FreRoyTen-Turing.pdf)


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
╰  [Pyro](https://paperswithcode.com/paper/pyro-deep-universal-probabilistic-programming)


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


6. Probabilsitic Python Program

Example

bernoulli = generates 0|1
```
def binominal(n, p):
    return sum( [bernulli(p) for i in range(n)] )
```

```
[bernulli(p) for i in range(n)]
```
create list of indepent calls of binary numbers of, mean of P


Create a statistical model
```
def binominal(n, p):
    return sum( [bernulli(p) for i in range(n)] )

def randomized_trial()
    
    ## model, but not bayesian
    return ( binominal(100, p_control),
             binominal(10,  p_treatment) )
             
## if run, returns variables undefined
```

Define random values, represents **Bayesian Model**
```
def binominal(n, p):
    return sum( [bernulli(p) for i in range(n)] )

def randomized_trial()
    p_control   = uniform(0,1)  # prior
    p_treatment = uniform(0,1)  # prior

    return ( binominal(100, p_control),
             binominal(10,  p_treatment) )
             
```

**Bayesian Model** of a randomized trial

Distribution:
-- >
time-series = simulation 
e.g., (71, 9)

Inference
<--

Query Program

```
def QUERY(guesser, checker):
    # guesser: Unit -> S
    # predicate: S -> Boolean
    accept = False
    
    while (not accept)
        guess = guesser()
        accept = checker(guess)
    return guess
    
```
lambda (_): True === QUERY predicate
guesser = 
checker = deterministic...takes inputs if true
take 2 programs, 

```
def N():
    return uniformInt(range(1, 180))
    # this is your guesser
```

QUERY(N, div235):
```
def div235(n):
    return isDivBy(n, 2) or isDivby(n, 3) of isDivBy(n, 5)
# takes interger
```


QUERY checker = deterministic

(P, 1A) |--> P(.|A) := P(. ⋂ A) / P(A)

rquals to while loop


---

**Stochastic Inference Problem** [Section 5](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf)

**Rejection Sample**
Return a single sample
```
accept = False
while (not accept):
    guess = guesser()
    accept = checker(guess)
return guess
```
* really slow 
* **k** = kevin bottle
* input: guesser and checker, probabilitistic programs
* output: distribution program
* Bay stat inf
    * **prior** distrib <--> guesser()
    * **likelihood(g)** <--> ℙ{ checker(g) is True } = while loop
    * **posterior** distrib <--> return value distrib

---

QUERY: **Inferring Bias of a Coin** [Section 6](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf)

return query of probability
```
accept = False
while (not accept):
    guess = guesser()
    accept = checker(guess)
return guess

```

* report prob of next value that is 1
𝑥n ∈ {0, 1}
𝑥n+1 = 1? 
    e.g., 0,0,1,0,0

```
def guesser():
    q = uniform()
    return q
    
def checker(q): # judges x roles from array
    return [0,0,1,0,0] == bernoulli(q,5)
```

Maths:
ℙ{checker(q) is True} = q(1-q)ⁿ⁻ˢ

ˢ = S

Baysain is about combining prior

---

**Inferring Objects from an Image** : [Section 07](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf)

```
accept = False
while (not accept):
    guess = guesser()
    accept = checker(guess)
return guess

```

Thing not observed, and unknown
```
def guesser():              # how many from the following distributions
    k = geometric()
    blocks = [ randomblock() for _ in range(k) ]
    colors = [ randomcolor() for _ in range(k) ]
    return (k,blocks,colors)

def checker(k,blocks,colors):   # comparative check for evidence
    return rasterize(blocks,colors) ==
```

---

**Extracting 3D Structure from Images** [Section 08](https://simons.berkeley.edu/sites/default/files/docs/5675/talkprintversion.pdf)
Guesser inference and of an Object

mesh poly <-- inference <-- image of an object
```
accept = False
while (not accept):
    guess = guesser()
    accept = checker(guess)
return guess

```
* silence of razeriation 
* not contraint by prior


mesh poly --> checker --> materialized mesh simulation of digital object model
```
accept = False
while (not accept):
    guess = guesser()
    accept = checker(guess)
return guess
```
* checker can't render, but checks for symmertry, noise 
* **gaussian noise modelling**
* only 1 data point if NN'ed


Conculsion:

* Bayesian Analysis == core ALGM && QUERY !== core ALGM
    * let `model()` = P and ......
* [inverse graphics / vision] - old idea
    * pixar uses this
    * optical illusions
* run image, 
* first and last factorial or vectorial(?) representations
* this is more sophisticated than gaussian modelling
* ***How do you create a learner guesser?***


---

**Church / Trace-MCMC** [Section]()

* represents as a search tree 
* returns 1 or 3
```
# flip bernoulli of 0|1 ---> p(1-p)ᵏ⁻¹
# keeps calling bernoulli until it reaches 1
def geometric(p):
    if bernoulli(p) == 1: return 1
    else: return 1 + geometric(p)
    
# trace function
# unnormalized probability
def aliased_geometric(p):
    g = geometric(p)
    return 1 if g < 3 else 0
    
```
* choose random or move around by rejecting while in state transistion
* uses a markov chain monte carlo for each while loop, search state to state until queried value reached
* stochastic of the **k** power

A. Proposal state transistion
B. metropolis-hastings rule state transistion


---

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
    
    
    
[A stochastic programming perspective on nonparametric Bayes](http://danroy.org/papers/RoyManGooTen-ICMLNPB-2008.pdf)
[Fields-CQAM Interdisciplinary Thematic Program](https://www.eventbrite.ca/e/fields-cqam-interdisciplinary-thematic-program-92001-tickets-51212616314)

