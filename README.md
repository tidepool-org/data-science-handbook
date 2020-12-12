# Tidepool's Data Science Team Handbook 
Welcome to the Tidepool Data Science Team Handbook. Please be sure to read [Team Governance](governance.md)
to get a sense of our purpose and philosophies. 

## Purpose
The purpose of this repository is provide guidance to those contributing to the Tidepool Data Science Team, 
and to document how Tidepool's Data Science Team operates. It is also a place to capture all of the non-code related
items that make up our ecosystem. 

## In this Repository
* [Cheat Sheets](cheat-sheets)
* [Checklists](checklists)
* G-Suite
    * G-Suite Instructions (TODO: instructions/g-suite.md)
    * [G-Suite Acrchitecture](g-suite-architecture)
* GitHub
    * [GitHub Instructions](instructions/github.md)
    * [GitHub Architecture](github-architecture) 
* [Governance](governance.md)
* [Instructions](instructions)
* [Lessons Learned & Gotchas](lessons-learned-and-gotchas)
* [Templates](templates) - all non-github templates
* [Tips & Tricks](tips-and-tricks.md)
* [Tutorials](tutorials)

## Architecture, Ecosystem & Tech Stack
* 1password - for password management
* aws - for cloud computing
    * compute-1
    * compute-2
    * S3
* confluence - our knowledge-management-system for internal and external knowledge sharing 
but it will point to github and g-suite
* datasets
    * can contain phi, or psi (partner sensitive information)
    * can exist in multiple locations
    * can exist in multiple states (e.g., raw, interim, processed)
    * for tidepool it can be all data or donor_data
    * mvp is to create for internal, partner, and public use
    * needs version control
    * source can be tidepool or external
    * we need to know what transformations were done
* email - for corresponding with partners and non-time sensitive materials
* g-suite - for creating documents that need review or collaboration
* github - for version control
* jira - for project and sprint management)
* knowledge-management-system - we may use confluence to share 
but data will be version controlled in github and g-suite:
    * data-science-insights repository (in github)
    * Data Science Team Drive (in g-suite)
* local-machine - the tools most of the team uses
    * macbook pro
    * excel
    * gitkraken
    * pycharm
* meetings - zoom for video chats, and google docs for meeting notes
* monday - for long term and roadmap planning
* slack - for real-time communication
* travis - for continuous integration
* templates and checklists:
    * if code or text based put in github, 
    * if application specific put directions and locations in handbook templates and checklist section
* zoom - for meetings
* zotero - for collecting papers and citing our work

## FAQs

### Google Doc vs. Report in GitHub
Q: When writing a document or report should I use a Google Doc or put the Github via markdown?

A: If the document is going to require feedback (comments, edits, suggestions) then start with a google doc.
Once the document is finalized, it can be converted into a markdown document and stored in GitHub using this
[Google Docs add-on tool](https://gsuite.google.com/marketplace/app/docs_to_markdown/700168918607).
