# Using Github

All Data Science Team work should be version controlled in 
[Tidepool's Github Account](https://github.com/tidepool-org).

## Repository Naming Convention:
    data-science--<type>--<short-consise-name>  
All data science Github repositories should start with `data-science` followed by the *type* of work
encapsulated by double dashes (e.g., `data-science--explore--`), followed by a short and concise  
description of the work (e.g., `data-science--explore--optimize-loop-settings`). 

## Types of Work
The *type* of work the Data Science Team does varies, but it generally starts in the exploratory phase (`--explore--`). 
The following list includes the types of work that the team has historically done, is currently doing, 
or is planning to do. We imagine this list will grow, but for now the following types will be used.

### Current *Types*
* explore - 95% percent of the work we do will start in an exploratory phase. If the project moves
beyond exploration then it can be renamed to one of the other *types*. Here are some exploratory examples:
    * `data-science--explore--algorithm-improvements` 
    * `data-science--explore--donor-data-distributions`
    * `data-science--explore--optimize-settings`
* analysis - each analysis should get its own repository:
    * `data-science--analysis--icgm-sensitivity`
    * `data-science--analysis--loop-accuracy`
    * `data-science--analysis--risk-scenarios`
* blogpost - all of the code, figures, and text that make up a blogpost:
    * `data-science--blogpost--10000-donors-2020-02-06` (TODO & DEBT)
    * `data-science--blogpost--cgm-data-2017-11-02` (TODO & DEBT)
    * `data-science--blogpost--insulin-pump-data-2018-02-15` (TODO & DEBT)
* template - reserved for github repository templates. For example:
    * `data-science--template--gist` template for small code samples and insights 
    * `data-science--template--explore` only includes a `master` branch
    * `data-science--template--product` includes a `master` and `develop` branch 
    * `data-science--template--pypi-package`
* tool - code that is useful to other repositories is put here after the exploratory phase:
    * `data-science--tool--controllers`
    * `data-science--tool--data-tools`    
    * `data-science--tool--metrics`    
    * `data-science--tool--models`    
    * `data-science--tool--simulators`    
    * `data-science--tool--visualization-tools`        
* visualize - all code to support visualizations (figures and tables) in important documents:
    * `data-science--visualize--tidepool-loop-bolus-recommendation-tool`
    * `data-science--visualize--qsub-<YYYY-MM-DD>`
* handbook - `data-science-handbook` a single repository that includes:
    * cheat-sheets - a place to put cheat-sheets (be sure to cite sources)
    * checklists - to capture anything/everything that has to be manually set up
    * lessons-learned-and-gotchas - share things that you wish someone would have told you before you got stuck or lost
    * governance - our mission statement and how we do (or want to do) data-science at Tidepool
    * instructions - instructions, procedures, and guides for meeting and using apps like like github and g-suite
    * templates
        * includes templates for every item on this list
        * does not include github and g-suite templates
    * tips-and-tricks - a place to share hacks with the idea that if you find it useful then someone else might too 
    * tutorials - for step-by-step walk-throughs 

### Ideas for future *Types*
* collaboration - for collaboration projects:
    * `data-science--collaboration--diabetes-data-science-working-group`
    * `data-science--collaboration--google-forecast-bgs`
* explain - for explanations on how something works:
    * `data-science--explain--how-dosing-decisions-work`
    * `data-science--explain--loop-algorithm`
* tutorial - step-by-step walk-throughs ideally written so someone with little to no experience would understand
    * `data-science--tutorial--make-interactive-viz-in-plotly-dash-`
* review - for literature reviews
    * `data-science--review--surveillance-error-grid`

### Really Small Projects
If the project is small or can be summarized with a small amount of code, then 
put the code in Github Gist. This will typically be done using Google Colab.

## Commit Naming Convention
    <type>(<optional-scope>): <subject>
The commit message format was inspired by this
[reference](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716#gistcomment-2862793).

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
 