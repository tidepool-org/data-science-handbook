# Using Github

All Data Science Team work does should be version controlled in the [Tidepool's Github Account](https://github.com/tidepool-org).

## Repository Naming Convention:
    data-science--<type>--<short-consise-name>  
All data science Github repositories should start with `data-science` followed by the *type* of work
encapsulated by double dashes (e.g., `data-science--explore--`), followed by a short and concise  
description of the work (e.g., `data-science--explore--optimize-loop-settings`). 


## Types of Work
The *type* of work the Data Science Team does varies, but it generally starts in the exploratory phase (`--explore--`). 
The following list includes the types of work that the team has historically done, is currently doing, 
or is planning to do. We imagine this list will grow, but for now the following types will be used:
* analysis: each analysis should get its own repository. For example:
    * `data-science--analysis--icgm-sensitivity`
    * `data-science--analysis--loop-accuracy`
    * `data-science--analysis--risk-scenarios`
* blogpost: all of the code, figures, and text that make up a blogpost. For example:
    * `data-science--blogpost--10000-donors-2020-02-06` (TODO & DEBT)
    * `data-science--blogpost--cgm-data-2017-11-02` (TODO & DEBT)
    * `data-science--blogpost--insulin-pump-data-2018-02-15` (TODO & DEBT)
* collaboration: reserved for collaboration projects. For example:
    * `data-science--collaboration--diabetes-data-science-working-group`
    * `data-science--collaboration--google-forecast-bgs`
* explore: 95% percent of the work we do will start in an exploratory phase. For example:
NOTE: if the work is short, then put in data-science--insights-- repository (see below). 
    * `data-science--explore--algorithm-improvements` 
    * `data-science--explore--donor-data-distributions`
    * `data-science--explore--optimize-settings`
* handbook: a single repository that includes:
    * cheat-sheets - NOTE: be sure to cite sources
    * checklists - to capture anything/everything that has to be manually set up
    * faqs
    * how-tos
    * gotchas
    * governance
    * instructions
    * recipes
    * templates
        * includes templates for every item on this list
        * does not include github and g-suite templates
    * tips-and-tricks
    * tutorials
* insights: a knowledge management repository. We will use github gist, markdown, and code should be down with 
colab notebook or plotly-dash application, 
non-code should be done in markdown, 
and done in gith in using colab and github :
    * donor-data-insights
    * literature-reviews. For example:
        * surveillance-error-grid
    * single-page-learnings
* template: reserved for github repository templates. For example:
    * `data-science--template--gist` template for small code samples and insights 
    * `data-science--template--explore` only includes a `master` branch
    * `data-science--template--product` includes a `master` and `develop` branch 
    * `data-science--template--pypi-package`
* tool: Code that is useful to other repositories is put here after the exploratory phase. For example:
    * `data-science--tool--controllers`
    * `data-science--tool--data-tools`    
    * `data-science--tool--metrics`    
    * `data-science--tool--models`    
    * `data-science--tool--simulators`    
    * `data-science--tool--visualization-tools`        
* viz: all code to support visualizations (figures and tables) in important documents. For example:
    * `data-science--viz--in-loop-algorithm-doc`
    * `data-science--viz--tidepool-loop-bolus-recommendation-tool`
    * `data-science--viz--qsub-<YYYY-MM-DD>`

## Commit Naming Convention
    <type>(<optional-scope>): <subject>
The commit message format was inspired by this [reference](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716#gistcomment-2862793).

### Commit Types
* feat: new feature for the user, not a new feature for build script. For example:
    * `feat: add new local time function`
* fix: bug fix for the user, not a fix to a build script. For example:
    * `fix: remove simple local time function`
* docs: changes to the documentation. For example:
    * `docs: explain new local time function`
* style: formatting, missing semi colons, etc; no production code change. For example:
    * `style: apply black and flake8`
* refactor: refactoring production code, eg. renaming a variable. For example:
    * `refactor: update utc time to be compatible with new local time`
* test: adding missing tests, refactoring tests; no production code change. For example:
    * `ensure local time is correct during travel`
* chore: updating grunt tasks etc; no production code change. For example: 
    * `add travis ci`
 