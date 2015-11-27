# ScPo-CompEcon Syllabus

* **Course:** Computational Economics for PhDs
* **Teacher:** Florian Oswald, [florian.oswald@sciencespo.fr](mailto:florian.oswald@sciencespo.fr)
* **Classes:** Bi-weekly Friday 14:45-16:45, starting 29 of January, ending 8 of April

## Course Description

This is a course for PhD students at the [Department of Economics at Sciences Po](http://econ.sciences-po.fr) in Computational Economics. 

## Course Overview

In this course you will learn about some commonly used methods in Computational Economics. These methods are being used in all fields of Economics. The course has a clear focus on applying what you learn. We will cover the theoretical concepts that underlie each topic, but you should expect a fair amount of *hands on* action required on your behalf. In the words of the great [Che-Lin Su](https://bfi.uchicago.edu/people/che-lin-su):

> Doing Computation is the only way to learn Computation. Doing Computation is the only way to learn Computation. Doing Computation is the only way to learn Computation.

True to that motto, there will be a homework associated to each session. There will also be a term paper. It will be helpful to bring a laptop to the sessions if you have one.

Topics will be demonstrated through live-code examples/slides, available at [ScPo-CompEcon.github.io/slides](http://ScPo-CompEcon.github.io/slides).  


## Prerequisites

* No previous programming experience is required. 
* Some experience with the [Unix Shell](https://en.wikipedia.org/wiki/Unix_shell) and the verion control system Git would be very useful - for this course, and for the rest of your life as a scientist. I do therefore recommend that you spend some time (2h total max) with the following excellent tutorials:
    1. [Software Carpentry: The Unix Shell](http://swcarpentry.github.io/shell-novice/)
        * If you are on MacOS/Unix, just open the terminal application and you're good to go.
        * On Windows, you need to make up for the fact that you are not Unix. I recommend [Gnu on Windows (GOW)](https://github.com/bmatzelle/gow/wiki)
    1. [What is Version Control? 5 minute video.](http://git-scm.com/video/what-is-version-control)
    1. [Try Git on codeschool.org](https://try.github.io/levels/1/challenges/1): This is a 15 minute intro to Git. So cool!


## Homeworks

Each session is accompagnied by a homework. They will be listed within the [Course Outline](#course-outline).

### Workflow of Homeworks

The aim of the following setup is to put a system in place by which we can easily look at your solutions to a problem, you can easily look at my solutions (next to yours), and we can also look at the solutions of your peers in order to have a better learning experience. Writing code *is* a activity with tremendous returns from collaboration, and we will try and foster that in this course. Apart from this, a vast amount of high quality code is nowadays developed following this model, so it is a useful skill for you to know how the *fork-change-pull-request model* works. 

If you don't know what Git is, please look at the [prerequisites](#Prerequisites/Try-Git-on-codeschool.org) first.

If you're using GitHub Desktop, [these instructions](https://help.github.com/desktop/guides/contributing/) will help explain the Git/GitHub concepts. Here are the overall steps:

1. Fork the repository for the homework (found under [github.com/ScPo-CompEcon](https://github.com/ScPo-CompEcon)).
1. Clone the repository to your computer.
1. Create a new branch on your computer called `my-solution`.
1. Modify the files to complete your solution.
1. Make sure your code runs and produces all output.
1. Write a test for your code if possible.
1. Commit all of your code to your local repository.
1. Push your branch `my-solution` up to GitHub.
1. [Create a pull request for `my-solution`](https://help.github.com/articles/creating-a-pull-request) on the original repository, i.e. the owned by [github.com/ScPo-CompEcon](https://github.com/ScPo-CompEcon). All assignments are due at the start of the following class, unless otherwise specified.
1. You can continue to push fixes and improvements until the close date (24 hours before the next class).
1. I will push my solutions to Exercise repository once you have handed in yours. You can then sync your master branch with those solutions. This way, you have both your solutions (on branch `my-solution`) as well as my solution (on the `master` branch).

### Requirements for Homeworks

* I invite you to do the homeworks in teams of 2. 
* You have two weeks for each homework, and they are due 24 hours before the next class, so that I have time to look at them and provide some feedback.
* Please make clear who the contributors are in your comment on the pull request.
* There is clearly a tradeoff between you learning by trying hard, learning from seeing the work of your colleagues, and not learning at all by just copy and pasting the best solution 1 minute before the deadline. I can only remind you that you harm noone but yourself by not exerting effort on the homeworks.
* Each solution you submit must contain text file called `outline.md` where you describe briefly in words what you are doing in your implementation. It is good practice to write this before you even start. (you can always go back and edit this document if you find out that what you wanted to do does not work, but at least you know always what you are trying to do.)

## Term paper

You are expected to produce a term paper over the course of the semester.  This could be
* A replication of a paper that uses computational methods.
* Computing additional things that another (maybe theoretical) paper does not compute.
* Ideally, it would be your own research project.

### Requirements for the Term paper

* You must do this on your own.
* The paper should be *max* 15 pages of double-spaced 12pt font text, excluding any graphs or tables.
* The paper should contain
    1. A motivation/introduction and formulation of the research question.
    1. A justification for why one needs computational methods to answer this question.
    1. A model.
    1. A clear outline describing the computational approach to compute the model.
    1. A presentation of the results.
    1. A discussion of the accuracy of the obtained results.
* Furthermore, the code you write needs to be on github, if you want in a private rather than public repository, to which you grant me access. (you get access to 5 private repos for free). There will be extra marks for code readability and code quality.



## Weapon of Choice: Which Software?

My weapon of choice for this course is the [Julia Computing Language](http://julialang.org). I see this as an occasion to persuade you to overcome any switching costs that may have put you off from learning Julia up until now and to give it a try. That said, for most programmers (of Python, Matlab or R) these switching costs are small. [If you are a Fortran/C++ programmer, the switching costs are negative, i.e. you will enjoy the switch.]

I appreciate that people have strong opinions on which software is **best**. We will briefly touch upon that question in the first session and think about the pros and cons of different languages.

## Textbooks

There are some excellent references for computational methods out there. This course will use material from 

* **Fackler and Miranda** (2002), Applied Computational Economics and Finance, MIT Press
* **Kenneth Judd** (1998), Numerical Methods in Economics, MIT Press
* Nocedal, Jorge, and Stephen J. Wright (2006): Numerical Optimization, Springer-Verlag

(recommended ones in bold face)


## Course Outline

Each subsection here stands for one session of 2 hours. There are 6 subsections.

### First Session

#### Session: Introduction and Logistics

1. First things first 
    * Put name on sticky note on back of monitor
    * Discuss what the class is going to cover
    * Everyone introduce themselves
        * Name
        * What you "do"
        * What are your goals for the class?
        * What's something related to *computation* in Economics you worry that your peers understand but you don't?
1. Setup
    * How many people are comfortable with Git/GitHub?
    * Install [GitHub Desktop](https://desktop.github.com/)
        * If you are comfortable with Git already, you can skip this.
    * Sign up for GitHub
1. GitHub workflow
    * Walk through [workflow](#workflow)
    * Create pull request on [students repository](https://github.com/ScPo-CompEcon/students)
1. Explain how slides work
1. Talk through [homework requirements](#homework-projects/requirements)
1. Talk through [term paper requirements](#term-paper/requirements)
1. Talk through [weapon of choice](#weapon-of-choice)

#### Computation!
1. Basic Computing concepts
    * The fundamental tradeoff: Speed vs Accuracy
    * Some numerical gotchas
    * Computer Memory
    * Error Analysis
1. Function Approximation
    * Polynomial Interpolation
        * Basis functions and Coefficients
    * Regression as Approximation
    * Colocation Methods
    * Multidimensional Approximation
        * The Smolyak Grid

#### Reading

* Aruoba and Fernandez-Villaverde (2014) [A Comparison of Programming Languages in Economics](http://economics.sas.upenn.edu/~jesusfv/comparison_languages.pdf)


#### Homework

* Join [the chat room]().
* Fork the first homework at [github.com/ScPo-CompEcon/UnconstrainedOpt](https://github.com/ScPo-CompEcon/UnconstrainedOpt)
* Clone to your machine
* create `my-solution` branch
* do work, commit, push branch to your github, finally create pull request on [github.com/ScPo-CompEcon/UnconstrainedOpt](https://github.com/ScPo-CompEcon/UnconstrainedOpt)

### Session: Numerical Integration and Differentiation

* Monte-Carlo integration
* Newton-Cotes Formulas
* Gaussian Quadrature
* Multidimensional Quadrature
    * Quadrature with correlated shocks
* Numerical Differentiation
    * Finite Differences
    * Automatic Differentiation
    * [JuliaOpt/JuMP.jl](https://github.com/JuliaOpt/JuMP.jl)
        
### Session: Optimisation
1. Unconstrainted Optimisation
    * Comparison Methods
    * Newton's Method
    * Line Search, Trust Region, and other Methods
    * Application: Maximum Likelihood
    * Introduce [http://www.juliaopt.org](http://www.juliaopt.org)
1. Constrained Optimization
    * Theory
    * Some Numerical Methods for Constrainted Optimization
#### Homework


### Session: Constrained Optimisation Applications
1. MPEC on John Rust's Bus Engine Replacement
1. The Berry-Levinsohn-Pakes (BLP) paper as constrainted optimization problems

#### Homework


### Session: Numerical Dynamic Programming

* Review of DP theory
* Different Solution methods for different cases
    * Discretization
    * Parametric approximation methods [basically Function Approximation](#Function-Approximation)
    * The Endogenous Grid Method
    * Finite time vs inifinite horizon models

#### Homework

### Session: Sky's the Limit - Parallel Computing in the Cloud

* Brief intro to parallel computing concepts
* Parallel computing with julia
* (Free) Cloud computing via the [Github Student Developer Pack](https://education.github.com/pack/join)

#### Homework

## Pairing Tips

* Three people is possible, but two works best
* Agree on an editor and environment that you're both comfortable with
* The person who's less experienced/comfortable should have more keyboard time
* Switch who's "driving" regularly
* Make sure to save the code and send it to both people

## Resources

### Beginner Materials

### Recommended Reading

### Tools

#### GitHub

* Git and GitHub
    * [Official GitHub Help](https://help.github.com/)
    * [Recommended resources](http://hackerhours.org/resources.html#github)
* GitHub Pages
    * [Official site](http://pages.github.com/)
    * [Thinkful guide](http://www.thinkful.com/learn/a-guide-to-using-github-pages/)



## Grading

50% homeworks, 50% paper

## Statements on Plagiarism


### Instructor

Reuse and building upon ideas or code are major parts of modern software development.  As a professional programmer you will never write anything from scratch.  This class is structured such that all solutions are public.  You are encouraged to learn from the work of your peers.  I won't hunt down people who are simply copying-and-pasting solutions, because without challenging themselves, they  are simply wasting their time and money taking this class.

Please respect the terms of use and/or license of any code you find, and if you reimplement or duplicate an algorithm or code from elsewhere, credit the original source with an inline comment.

## License

I took considerable inspiration in setting up this course from the [https://github.com/advanced-js](https://github.com/advanced-js) at NYU, and I would like to greatly acknowledge making the materials useable to other teachers. The same license applies:

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">work</span> and all other materials under https://github.com/ScPo-CompEcon are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.