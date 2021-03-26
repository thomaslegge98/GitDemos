# Git Demo

## What do I need to do?

Follow these steps. These will hopefully give you some experience with the most important features of git and GitHub. All of the steps before the pull requests on this doc are completable using the command line or with a git GUI application such as GitKraken (recommended). This guide will have details for using GitKraken, but the steps will be roughly the same with other git GUIs.

Once you make the PR, the steps will basically all be done using the GitHub website.

### Objectives of your pull requests (PRs)

1. Add your favourite food to the list of foods in `Foods.yaml`.

2. Suggest what the next hands-on thing like this might be about in `NextTime.yaml`.

### Steps to complete

0. [Optional] Open your git GUI of choice, and open this repo within it.

1. Make a branch off of the latest commit on `main` (the main branch might be called `master` on our other repos). The name of the branch should be of the form `<your_last_name>/<thing_this_branch_does>`. For example, when Kip did the task, his branch was `hamiltons/add_pizza`, since pizza is the food he added to the list.
On GitKraken, right click on the latest `main` branch commit, and select create branch here. Follow the prompts to name your branch.

2. Open `Foods.yaml` in a text editor or IDE and add your favourite food to the list. Save your changes to the file.

3. Add the file to git's "Staging Area". This is like a preparatory zone where you can save files as ready to commit - although usually you'll commit them immediately anyway. On GitKraken, changed files will come up on the right at the top, where it says "1 change in working directory". Click to view the change, and you can see a "diff". Diffs are compact, intuitive ways to see what changes are made to a file. On the file in that top right menu is a "stage" button. Use it to add the file to the staging area.

4. Commit the changes to the file. Add a commit message describing the changes you made. On GitKraken, below where the file is staged is a prompt for a commit message. Enter a message, then click the button to commit the changes. The file change is now saved locally, and you can go back to this state of the repo easily in the future, if you need to.

5. Open `NextTime.yaml` and suggest something which we could do other sessions on (like this one). One example might be "Contributing the NUbook". This could be anything you're hoping to learn about to do with NUbots. Other examples could be "Using Docker", or "Making a module".

6. Stage and commit your changes to that file. 

7. Push your commits to `main`. This saves your commits to a branch on the remote repo, which is in this case on GitHub.

8. Make a PR. If you go to the GitHub website for the repo (https://github.com/NUbots/GitDemos), there shouold be a prompt suggesting that you make a pull request, because you just pushed changes to a branch. Follow that prompt to make a PR. Make sure that you:
- Give your PR a good title, describing the changes.
- Add a description to your PR if you have other things reviewers should know (you won't in this case). You can also add checklists for things which are yet to be done.
- Request reviews from people. For this task, just pick random peers who are here today. In the NUbots codebase, this will usually be your "mentor", and optionally team leaders, and anyone who knows things about the stuff you're editing. For example, if Moosa was making tests for vision, he might add Joel (his mentor), Ysobel (because team leader, why not lol), and perhaps Alex B (a vision expert) too. It's not a big deal if you request someone and they don't want to review it. They can just ignore the email lol. People who didn't get requested can still offer comments or reviews on your PR too.

Note that your PRs update automatically if you push commits to that branch on the remote repo. So if someone requests changes to your PR, you can make the changes locally, then stage, commit, and push them to automatically update your PR. The reviwer(s) will be notified that you made changes, but you can manually re- request review if you want to.

9. Review 2 other peoples PRs. Make a comment on specific lines they have changed, and add a main message of the review which isn't associated with the lines. We will approve them all towards the end, so just leave comments or request changes for now.

10. Reply to someone else's comment on a PR. Let them know that their choice of food is good, or if it stinks.

11. Merge the `main` branch into your branch. This should (hopefully in this case) make you deal with a merge conflict, which is where your branch changes the same line that another branch which was already merged into. You have to manually pick what changes your PR will make to those lines. **You might have to do this a few times, because I have set things up to make sure you deal with a merge conflict, which could cause you to have to deal with a few of them ¯\\_(ツ)_/¯**.

12. When we get close to the end of our time, approve a PR, and merge yours into `main` once yours is approved. Once you've merged yours in, see if anyone else still going could use a hand and help them out.
