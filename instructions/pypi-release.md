#pypi release
1. If you do not have a pypi account, create a user account on https://pypi.org/ or https://test.pypi.org/ depending on 
where you will be deploying. If this is an existing project in pypi, you will need to be a maintainer or owner of the project. 
2. Create and checkout a Github Branch from the Master Branch for the project you will be deploying.
3. Setup the virtual environment and run all test and TOX 
4. Update the `version_string` with the version number for this release. (v0.1.0).
5. If you are deploying to the https://test.pypi.org/, ensure the `twine` execution is using `--repository-url https://test.pypi.org/legacy/`
   within the 'pypi_push.sh' script. Example would be `python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
   if not, modify and save. 
6. If you are deploying to https://pypi.org/, ensure the `twine` execution does not contain `--repository-url https://test.pypi.org/legacy/`
   within the 'pypi_push.sh' script. If not, modify and save.
7. From the commandline excecute the `pypi_push.sh` and enter in your userid and password. If successful, it will
 give you 
a link to view your upload. 
8. Undo any changes you made to the `pypi_push.sh` file. 
9. Create a git PR to merge your branch into master. This will ensure the version update is in the master branch. 
10. Once the PR is complete create a git version release from the master branch. 
