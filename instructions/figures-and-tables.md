# Figures and Tables

In many projects and analyses, the Data Science Team uses various figures
and tables to communicate both analysis steps and findings/results. 

This page provides an overview of the tools used for creating these figures 
and tables, as well as best practices, naming conventions and other guidelines
decided on by the team.

Our goal through many of these guidelines is to create figures and tables for analyses
that are clear, informative, reproducible and do not duplicate previous data visualization work.

## Data Visualization Tools

The Data Science Team uses a variety of visualization tools and packages
for generating figures including:

1. Matplotlib
2. Plotly 
3. Dash, 
4. Plotly Orca

[TODO: link to a page with references and tutorials for each of these tools after created]

## General Visualization Guides and Best Practices

For more general data visualization guides, references, and best practices, see
the [Data Visualization Cheat Sheets and References Page](https://github.com/tidepool-org/data-science-handbook/blob/master/cheat-sheets/data-visualization.md).

## Naming Conventions

All tables and figures should be named using the following convention.

    [short-desciption]_[utc-datetime]_[code_version]_[file-type]
    
For example,
        
    icgm-sensitivity-analysis-table1_2020-04-27-16-04-38_v0-1-0.png


## Options for Hosting and Sharing Figures

1. GitHub Pages
2. Heroku
3. Google Colab: As a team, we decided we will not save figures in Google colab, but if someone 
(most likely outside of the Data Science Team) wants to save a figure in colab, 
they can use the plotly built in tool.

[TODO: link to tutorials for these solutions after create]