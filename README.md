README for SMI205 Assessmnet 2 template
================
Aneta Piekut
2023-05-22

- <a href="#1-replication-report---template"
  id="toc-1-replication-report---template">1. Replication report -
  template</a>
  - <a href="#11-your-workflow" id="toc-11-your-workflow">1.1. Your
    Workflow</a>
  - <a href="#12-re-publishing-data-and-code"
    id="toc-12-re-publishing-data-and-code">1.2. Re-publishing data and
    code</a>
- <a href="#2-rpubs-version-of-the-template"
  id="toc-2-rpubs-version-of-the-template">2. Rpubs version of the
  template</a>
- <a href="#3-renv-package" id="toc-3-renv-package">3. <code>renv</code>
  package</a>
  - <a href="#31-how-to-work-with-renv-package"
    id="toc-31-how-to-work-with-renv-package">3.1. How to work with
    <code>renv</code> package</a>
  - <a href="#32-trouble-shooting-with-renv-package"
    id="toc-32-trouble-shooting-with-renv-package">3.2. Trouble shooting
    with <code>renv</code> package</a>
- <a href="#4-transparency-checklist" id="toc-4-transparency-checklist">4.
  Transparency checklist</a>
- <a href="#5-my-enviroment" id="toc-5-my-enviroment">5. My enviroment</a>

> Clone this repository in your R Studio -\> New Project -\> Version
> control.

# 1. Replication report - template

Edit `SMI205_Assessment2_Template.Rmd` by adding pieces of your work
into it. It is a template prepared to help you to write a transparent
research report. Your job is to make your research fully reproducible.

Publish it as a reproducible report on [Rpubs.com](https://rpubs.com/)
website and create a project repository on Github (optional).

> Use your student number to name your Rpubs and Github accounts so your
> work is anonymous.

As any template, it can be improved, so go on and make edits so your
report is even more transparent.

## 1.1. Your Workflow

As with other projects, organise your work transparently into a
hierarchy of folders.

Project TIER Protocol 4.0
(<https://www.projecttier.org/tier-protocol/protocol-4-0/>) offers an
excellent guide for what to include and how to organise reproduction
documentation for a project based on quantitative methods.

## 1.2. Re-publishing data and code

You should not be republishing data that you have not created or
substantially edited to create a new version of a dataset.

> Check what is the licence of the data and code:
> <https://www.sheffield.ac.uk/library/copyright/licences>. It might be
> the licence allows remixing, tweaking, and building upon others work
> non-commercially.

If you found a replication package for your chosen paper, remember to
credit the original material, like R scripts, developed by other
researchers.

# 2. Rpubs version of the template

HTML version of the template is published here:
<https://rpubs.com/AnetaPiekut/SMI205_Assessment2_2023_template>

# 3. `renv` package

The Template.Rproj was created without using `renv` package, yet, you
could consider using it. The `renv` package helps you to create a
reproducible environment for your R project. Read more here:
<https://rstudio.github.io/renv/>.

It saves information about R and loaded packages. So if you later (after
any R updates or changes in the packages) or other people open your
Rproj, it will install the same libraries, and will not use the central
libraries installed on a computer ([Joseph
2022](https://medium.com/@adrian.joseph/renv-make-r-environment-reproducible-414d88c683aa)).

## 3.1. How to work with `renv` package

It is likely you will need to install new packages and would like to
change the saved local libraries. There are three important commands in
the package to do so:

- Call `renv::init()` to initialise a new project-local environment with
  a private R library.
- Call `renv::snapshot()` to save the state of the project library to
  the lockfile (called renv.lock).
- Call `renv::restore()` to recall the packages and version the last
  time you called `renv::snapshot()`.

They are called automatically when you work in RProj and initiate `renv`
at the start.

## 3.2. Trouble shooting with `renv` package

Here is a useful guide by Joseph A. (2022). renv: make R environment
reproducible. URL:
<https://medium.com/@adrian.joseph/renv-make-r-environment-reproducible-414d88c683aa>
(accessed 09/02/2023).

# 4. Transparency checklist

- Are all files organised and saved in relevant folders?
- Are all files, variables and R objects named and organised in a way,
  so their role is clear?
- Have you created a READme file introducing your project?
- Is a replication package or any other files provided by the authors
  properly referenced in your work?
- Is your project portable? Are your directory paths relative?
- Have you tested whether your project runs on a different device?
- Remove from your repository any unused templates before submitting
  your work.
- Make sure you save information about your workspace specifications in
  your READme file (see my below).
- Before saving files in remote, Github repository, make sure you are
  not sending over any sensitive information.

# 5. My enviroment

Below you can find information about versions of R and specific packages
used to create this project.

``` r
sessionInfo()
```

    ## R version 4.2.2 (2022-10-31 ucrt)
    ## Platform: x86_64-w64-mingw32/x64 (64-bit)
    ## Running under: Windows 10 x64 (build 19045)
    ## 
    ## Matrix products: default
    ## 
    ## locale:
    ## [1] LC_COLLATE=English_United Kingdom.utf8 
    ## [2] LC_CTYPE=English_United Kingdom.utf8   
    ## [3] LC_MONETARY=English_United Kingdom.utf8
    ## [4] LC_NUMERIC=C                           
    ## [5] LC_TIME=English_United Kingdom.utf8    
    ## 
    ## attached base packages:
    ## [1] stats     graphics  grDevices utils     datasets  methods   base     
    ## 
    ## loaded via a namespace (and not attached):
    ##  [1] compiler_4.2.2  fastmap_1.1.0   cli_3.6.0       tools_4.2.2    
    ##  [5] htmltools_0.5.4 rstudioapi_0.14 yaml_2.3.7      rmarkdown_2.20 
    ##  [9] knitr_1.42      xfun_0.37       digest_0.6.31   rlang_1.0.6    
    ## [13] evaluate_0.20
