
git branching strategy


Distributed version control systems like Git give individuals wide flexibility in how they use version control to share and manage code. Your team should find a balance between this flexibility and the need to collaborate so that you share code in a consistent manner.

Why bother with branching?
Branching allows a team of developers to collaborate inside of one central code base. Team members publish, share, review and iterate on code changes through Git branches shared with others.

Adopt a branching strategy for your team. You collaborate better and spend less time managing version control, and your team spends more time developing.

Keep it simple
Keep your branch strategy simple by building from these three concepts:

Use feature branches for all new features and bug fixes
Merge feature branches into the master branch using pull requests
Keep master branch up-to-date
A strategy that extends these concepts and avoids contradictions will result in a version control workflow for your team that is consistent and easy to follow.

Feature branch strategy
Develop your features and fix bugs in feature branches based off your master branch (also known as topic branches). Feature branches isolate work in progress from the completed work in the master branch. Git branches are inexpensive to create and maintain. Even small fixes and changes should have their own feature branch.


Feature branching
Creating feature branches for all your changes makes reviewing history very simple. You can have a clean commit history which can be helpful to debug (or) revert when needed.

Branch naming convention
Use a consistent naming convention for your feature branches to identify the work done in the branch.

Few suggestions for naming feature branches: 
* feature/feature-name 
* feature/feature-area/feature-name 
* bugfix/description 
* hotfix/description

feature : New feature 
bugfix : Changes linked to a known issue 
hotfix : Quick fixes to the codebase

Review and Merge
The review of a pull request is critical for improving code quality. Only merge branches through pull requests that pass your review process. Avoid merging branches to the master branch without a pull request.

Reviews in pull requests take time to complete. Your team should agree on what's expected from pull request creators and reviewers. Distribute reviewer responsibility across your team and spread out knowledge of your codebase.

Research says that conducting peer review increases the number of distinct files a developer knows about by 66% to 150% depending on the project.
A few suggestions for successful pull requests:

Two reviewers is an optimal number
Take care not to assign the same reviewer(s) to a large number of pull requests. Pull requests work better when a reviewer’s responsibilities are shared across the team.
Provide enough detail in the description about the change
Include a build (or) linked version of your changes running in a staged environment with your changes so others can easily test
Branch Policy
Branch policies help teams protect their important branches of development. Policies enforce your team's code quality and standards. If you are using Github, here is how the branch policies look like:


Github repository branch policies
Manage releases
Once you have a stable master branch with up-to-date code, managing releases can be done either by maintaining release branches or tags.

Release Branches 
Create a release branch from the master as you get close to your release or other milestones, such as the end of the sprint. Give this branch a clear name associating it with a release, for example release/2.0 .

Tags 
Tags are useful for marking points in your history as important. Tags can be used instead of release branches and push the fixes into master as hotfixes through pull requests.

Conclusion
A git branching strategy is important to have a smooth development process. Defining how you branch, review, and release can help your team move fast.

I hope you’ve gotten a basic understanding about Git branching strategy. I’m looking forward to writing on Git workflow and concepts of Git. Comment on a topic that you want me to write about next. Cheers!
