<!--Copyright (C) 2021 SuperDARN Canada, University of Saskatchewan 
Author(s): Marina Schmidt 
Modifications:

Disclaimer:
-->

# Pull Requests 

Pull Requests in GitHub are a nice means of allowing others to review and test your code. 
This allows members of the community to know what is coming up in new releases of RST and be part of the collaboration.  


## Code Check List

Before submitting a PR check the code check list first:

- copyright and disclaimer, or modification line is added 
- the code compiles and runs with no extra warnings
- documentation is updated or in another PR for users 
- unit tests or various testing has been added/done 
- code is on its own *git* branch
- all code is pushed to the branch 

## Creating the PR 

Once you have confirmed the above is done you can go to [RST's Pull Requests](https://github.com/SuperDARN/rst/pulls)
and click on `New pull request`. If templates are available select which one is most appropriate. Otherwise make your own. 

### Merging Direction 

When in doubt merge to `develop`! Otherwise here are some other options:

- merge to another branch if you `checkout` from that branch this helps to break things into smaller parts for quicker review and testing
- merge to `master` **ONLY** if it is a **HOTFIX** or **RELEASE** branch. 

    !!! Note
        **HOTFIX** is a substantial fix for a bug that prevents users from installing or using RST or gives inaccurate data. Document fixes can 
        also be seen as a **HOTFIX** as they do not require release and DOI'ing on the code. 

- In some cases, documentation can be merged to `master` if it is fixing some typos. 

### Writing a PR

Follow the template to fill out the required sections. If there is no template, here is a check list to ensure you have all the information: 

- Informative title 
- Description of the changes you made 
- Scope on what people should focus on 
- How to install the code if there is any changes 
- Code fragments showing how to test the code and expected output/plots
- Extra details 

### Extra Tidbits

Pull requests on GitHub have other ways to help users know what your PR is all about. 
Here are some things you can do to get more attention:

- assign reviewers you want feedback from 
- add labels
- assign a project to it if applicable 
- assign a milestone if applicable 
- Linking issues if applicable

### Draft or not to Draft? 

Draft Pull Requests are a way to tell reviewers that this code is not intended to be `merged` right away. 
These kinds of pull requestions are handy for the following situations:

- It has multiple other PRs that are merging to it that needed to be tested/reviewed first 
- Has a major bug or need further work but you are looking for input and want to show others the changes you have done

## Guidelines 

Here are some general guidelines to follow with Pull Requests: 

- Do not merge your own code unless you have 2 or more approvals (1 being testing and the other being a code review) and no one is responding to merge 
- Make sure your code is fully complete before making a PR to avoid commit emails occurring frequently 
- Make sure your code is tested on various operating systems if needed 
- Optional code is reviewed in a Code Review 
