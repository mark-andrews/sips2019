A [SIPS 2019](https://www.improvingpsych.org/SIPS2019/) workshop on
doing reproducible research with RMarkdown and Git
================
Mark Andrews
July 8, 2019

This workshop will be in room *Maxima* in the *Engels Meeting and
Conference Center* [Stationsplein 45, 3013 AK
Rotterdam](https://goo.gl/maps/CNkJifuEYnvw2EM1A) from 9:30 to 14:15
(with a break at 11:00-11:30 and 12:15-13:30) on July, 8, 2019.

This workshop will be hands-on and learn-by-doing and we will spend most
of the time creating articles and slides using RMarkdown, and working
with Git. I have some slides and notes, however.

  - [Workshop slides](slides/slides.pdf)
  - [Introduction to Git](git_intro/git_intro.md)
  - In the workshop, one of the major aims will be to create an [article
    like this](demos/demo.pdf) from scratch
  - And we’ll also try to make [beamer slides like
    this](demos/beamer_demo.pdf) and a [papaja based manuscript like
    this](demos/papaja_demo.pdf) from scratch too

Anything else that is needed can be obtained by browsing through the
GitHub repository or by downloading all of its content as a zip, or
better yet, by cloning this repository.

    git clone https://github.com/mark-andrews/sips2019.git

## Preparing R/RStudio

You should have R and RStudio installed on your computer. It is not
strictly necessary but it is best to have the latest version of both R
and RStudio. You should also make sure your already installed R packages
are up to date. In terms of the packages that you need for this
workshop, which should ideally install before the workshop starts, the
following (I think) covers everything. Unless otherwise stated, these
packages are all on CRAN so be installed using the `Install` button in
the `Packages` pane, or with `install.packages`.

  - `rmarkdown` and `knitr`: These will probably be installed already.
  - `tinytex`: If you have /installed and working on your machine, and
    have sucessfully got it working with `rmarkdown` and `knitr`, then
    you can skip this step. Otherwise, this is probably the single most
    important package for the workshop. It installs a subset of the /so
    that it can be used with `rmarkdown` and `knitr`. Although /is
    open-source and cross-platform software, installing and confguring
    it can be considerably more trouble than installing an R package.
    Therefore, `tinytex` is extremely welcome. Installing `tinytex`
    itself just takes a few seconds, but then you need to do
    `tinytex::install_tinytex()` to install and configure everything.
    That could take 10-20 minutes.
  - `tidyverse`: This is a package of packages and installing
    `tidyverse` installs dozens of other packages like `dplyr`, `tidyr`,
    `ggplot2`, and so on.
  - `papaja`: This must be installed from
    [GitHub](https://github.com/crsh/papaja) with
    `devtools::install_github("crsh/papaja")` (and so `devtools` must be
    installed first).
  - `cowplot`: Just required for a few examples.
  - `kableExtra`: Also, just required for a few examples.
  - `citr`: A handy add-on to RStudio, but not vital.

## Preparing Git

Git is available on macOS, Windows, Linux.

  - For macOS, I *believe* git is pre-installed. For any Mac I’ve used,
    thus was the case, and it also says so
    [here](https://apple.stackexchange.com/a/304101), but I could be
    wrong. In any case, there are many ways to install it on macOS. I’m
    not sure which is the best or easiest, but [this
    advice](https://hackernoon.com/install-git-on-mac-a884f0c9d32c)
    looks good.
  - For Windows, you want to use *Git Bash*. Install it from
    [here](https://git-scm.com/downloads). Here’s a helpful
    [video](https://youtu.be/eo00v2aw92Y).
  - For Linux users, if you don’t have it already, you’ll need to do
    `sudo apt-get install git` or `sudo pacman -S git`, or some such.
    You know the drill.

## Create a GitHub account

If you haven’t done so already, create a [GitHub](https://github.com/)
account. There’s no fee. That’s only if you want private repositories,
etc.
