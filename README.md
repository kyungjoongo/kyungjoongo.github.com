
GitHub Pages Basics / Creating Project Pages using the command line

How can we help?

Creating Project Pages using the command line
If you're familiar with command-line Git, it's straightforward to manually create a Project Pages site.

Make a fresh clone

To set up a Project Pages site, you need to create a new "orphan" branch (a branch that has no common history with an existing branch) in your repository. The safest way to do this is to start with a fresh clone:

git clone https://github.com/user/repository.git
# Clone our repository
Cloning into 'repository'...
remote: Counting objects: 2791, done.
remote: Compressing objects: 100% (1225/1225), done.
remote: Total 2791 (delta 1722), reused 2513 (delta 1493)
Receiving objects: 100% (2791/2791), 3.77 MiB | 969 KiB/s, done.
Resolving deltas: 100% (1722/1722), done.
Create a master branch

Once you have a clean repository, you'll need to create a new master branch unless your cloned repository already has a master branch.

Tip: You can also create a gh-pages branch for your Project Pages site instead. To learn more about your options, including the option to publish your Project Page from a /docs folder on your master branch, see "User, Organization, and Project Pages."
Switch directories into your new cloned repository:

cd repository
Check if your repository already has a master branch:

git branch
# shows a list of branches for your repository