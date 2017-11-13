# Online Collaboration with Git and GitHub

### GitHub

[Sign up](https://github.com/join) or use an existing account if you have one.

### Set up git
 * [Download git](https://git-scm.com/downloads) (command line <strong>strongly</strong> encouraged)
 * [Set your name](https://help.github.com/articles/setting-your-username-in-git/)
 * [Set your email address](https://help.github.com/articles/setting-your-commit-email-address-in-git/)

### Fork

Create a fork of this repository under your account (see [forking](https://guides.github.com/activities/forking/#fork)).

### Clone your fork

At the command line, enter the following:

    git clone <your-fork-url>

### Create a branch

Within your fork, create a branch whose name is your UNI. All your work should be maintained on this branch.

    git checkout -b <your-uni>

### Add your Markdown page
 
Create a new [Markdown](https://guides.github.com/features/mastering-markdown/) file under the `/people` directory whose name is your UNI and file extension is `.md`. For example, if your UNI were ab9876, the file would be `/people/ab9876.md`.

On this page describe your academic/professional interests or projects you are currently working on in under 500 words. The following variables must be defined in the [front matter](https://jekyllrb.com/docs/frontmatter/):

    ---
    layout: people
    github_username: <your-github-username>
    last_name: <your-last-name>
    first_name: <your-first-name>
    ---
    
After you've saved the file, add it to staging:

    git add /path/to/people/ab9876.md

This is now included on the list of changes to commit.

### Commit changes

In your commit message, state the page that was added. Below is an example of what the command should look like (see [Git Commit Best Practices](https://github.com/trein/dev-best-practices/wiki/Git-Commit-Best-Practices)).

    git commit -m "Add page `/people/ab9876.md`"

### Push commits
Your changes so far have been local. The following command pushes them to a new branch on your fork:

    git push origin <your-uni>

### Create a pull request

Create a pull request from the branch on your fork to the `master` branch on the origin repository (see [Creating a pull request from a fork](https://help.github.com/articles/creating-a-pull-request-from-a-fork/)).

_After the majority of students have successfully created a pull request, the instructor will demonstrate the merged result._
