# development-guidelines
How we do version control, etc.

## Version control
We use Git and GitHub as our version-control system. Here is the workflow you should follow:

+ Create the project under the **OrlandoSentinel** organization
+ Fork the project under your personal account
+ Clone the project you just forked onto your machine
+ Add the original OrlandoSentinel repository as another origin: `git remote add original REPOSITORY_URL_HERE`
+ Do not make any commits on the master branch. This branch should always be stable and ready for deployment. Instead, make a feature branch named after whatever you’re doing (hotfix, add styles, etc.), and do all your commits there. When you’re ready to make your changes live, you’ll first want to merge your feature branch back into the master branch locally. Then, push your master branch back to your forked repository. Finally, submit a pull request back to the original repository under OrlandoSentinel.
+ It’s likely others will be contributing to our repositories. That’s why it was important in the fourth bullet point to add the original repository as another remote. When you’re working off your forked repository, you can pull in changes from the original to make sure you’re staying in sync: `git pull original master`
