---
title: "Setup and Introduction"
linktitle: "00: Setup and Introduction"
date: "2021-01-19"
module: "0"
start_date: "2021-01-19"
end_date: "2021-01-25"
menu:
  content:
    parent: Course content
    weight: 1
type: docs
toc: true
---




## Required content
- <i class="fab fa-youtube"></i> Lecture: Course Introduction ([see below](#lecture-course-introduction))
- <i class="fas fa-desktop"></i> Install R and RStudio ([see below](#install-the-software-you-need)).
- <i class="fas fa-cloud"></i> Create an [RStudio Cloud](https://rstudio.cloud/) account. A free account is fine!
- <i class="fas fa-book"></i> [R For Data Science: Introduction](https://r4ds.had.co.nz/introduction.html)
- <i class="fab fa-youtube"></i>  [Take a tour of RStudio’s IDE](https://rstudio.com/products/rstudio/?wvideo=520zbd3tij )
- <i class="fas fa-book"></i> [STATS 545: R Basics](https://stat545.com/r-basics.html)

## Suggested content

- <i class="fas fa-desktop"></i> [RStudio Primers: Programming basics](https://rstudio.cloud/learn/primers/1.2)

## Install the software you need

For this course, we need to install R, RStudio, and the packages we'll be using. This is a three step process!

Check out [STAT 545: Install](https://stat545.com/install.html) for more guidance.

1. [Install the latest version of R](https://cloud.r-project.org/)
2. [Install the latest version of RStudio](https://rstudio.com/products/rstudio/download/#download)
3. Follow the instructions below to install all the packages we will be using in the course

Open RStudio and run this code in the console. **NOTE**: R may ask you to install source packages instead of binaries. (`Do you want to install from sources the packages which need compilation? (Yes/no/cancel)`. **Say "no" for now.** We'll circle back to what this means later.

```r
options(repos = "https://cran.rstudio.com/")
install.packages("remotes")
remotes::install_github("malcolmbarrett/masterepir")
```

This will take some time as many packages will be downloaded. When complete, you'll see `DONE (masterepir)` displayed in the console.

**NOTE**: You may encounter an error trying to install certain packages that require additional software. A common source of such errors is needing Rtools on Windows or xcode on Mac. Read more here on how to set these up on your local computer: https://r-pkgs.org/setup.html#setup-tools


`masterepir::install_course()` will install the course materials on your computer. Then, it will open a new RStudio Project containing the files you'll need.

``` r
masterepir::install_course()
```

By default, this package downloads the materials to a conspicous place like your Desktop. You can also tell `install_course()` exactly where to put the materials with `destdir`:

``` r
masterepir::install_course(destdir = "a/path/on/your/computer")
```

## Set up an RStudio Cloud account

We'll also be using [RStudio Cloud](https://rstudio.cloud/). Sign up for a free account. Then, join the RStudio Cloud course workspace at http://bit.ly/master_r_epi_mar21. The RStudio Cloud workspace will have all the R packages and course material you need. In other words, the course material will just work here without you having to do any setup! If you are having trouble with your local setup, we highly recommend just using this workspace.

**Important**: Please turn in all your assignments on RStudio Cloud, even if you're working on your local computer. For assignments, you don't need to do anything to "submit." The TAs and I will have access to the most recent state of your assignment.  

**For grading, it's critical that we can run your assignment.** Make sure you restart your R session often while working (In RStudio, go to `Session > Restart R`) and re-run your code so you know it's working properly. See ["Start R with a Blank Slate"](https://rstats.wtf/save-source.html#always-start-r-with-a-blank-slate) for more information.

## Lecture: Course Introduction

Videos for each section of the lecture are [available at this YouTube playlist](https://www.youtube.com/playlist?list=PLYCuG6HXKxjSp6ooKP-BsVZ5RXp1Yx_hq).

- [01 - Welcome](https://www.youtube.com/watch?v=YuUA26T4y7o&list=PLYCuG6HXKxjSp6ooKP-BsVZ5RXp1Yx_hq)
- [02 - Intro to R and RStudio](https://www.youtube.com/watch?v=GP2XcZaOXd4&list=PLYCuG6HXKxjSp6ooKP-BsVZ5RXp1Yx_hq)

You can also watch the playlist (and skip around to different sections) here:

<div class="embed-responsive embed-responsive-16by9">
<iframe class="embed-responsive-item" src="https://www.youtube.com/embed/videoseries?list=PLYCuG6HXKxjSp6ooKP-BsVZ5RXp1Yx_hq" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
