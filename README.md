<img align="right" height="110" src="laughing_broccoli.jpg">

# The Laughing Broccoli 

Hello good people!\
The following is a step-by-step walkthrough on how to cook the perfect broccoli
### How to use:
* See where you are in the Table of Contents
  * Whose broccoli are you dealing with?
* Click on it and go through the points

----

## Table of Contents
#### My broccoli
1. [Prepping your kitchen](#prepping-your-kitchen)
2. [Cooking your broccoli](#cooking-your-broccoli-in-progress) (In Progress)
3. [Plating your broccoli](#plating-your-broccoli-in-progress--code-review) (In Progress &#8594; Code Review)
4. [Please taste my broccoli](#please-taste-my-broccoli-passed-code-review) (Code Review &#8594; Testing)
7. [Cleaning your kitchen](#cleaning-your-kitchen-optional)
#### Friend's broccoli
6. [Reconsidering your friend's broccoli](#reconsidering-your-friends-broccoli-code-review) (Code Review)
7. [Tasting your friend's broccoli](#tasting-your-friends-broccoli-testing) (Testing)
#### Nobody's broccoli
8. [Getting more broccoli](#getting-more-broccoli-backlog) ([Backlog](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE&view=planning.nodetail))
9. [Found new broccoli](#found-new-broccoli-creating-new-tickets) (Creating new tickets)
#### Misc
10. [Resources](#resources)

----

## Checklist

### Prepping your kitchen
- Monday? New sprint? [Check out your new partners](https://ccle.ucla.edu/mod/page/view.php?id=815435)
- Check out the [Jira board](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE) to see what is up for today
  - Go right to left. Prioritize tickets on **testing** or **code review**.
- Let's go terminal! :muscle:
- Start up your local DEV [(cmd)](docker_tips.md#start-container)
- Log in to Slack
- Open your :heart: IDE


### Cooking your broccoli (In Progress)
- Read the ticket description
- Click on *Linked issues* (if exist) for reference or clarification
- @\<reporter\> to ask further questions
- Make sure you're in the right branch
  - `git branch` to check your current branch
  - If you're just starting the ticket, [create a new branch](git_stuff.md#create-a-new-branch-off-master): \
    Else: `git checkout <the ticket's branchname>`
- Cook the broccoli [tips and tricks](cooking_tips.md)
- Make git commits as needed ([cmd](git_stuff.md#commit-files-you-changed))
  - Only add changes you made. Sometimes you'll see that there are changes that you didn't make (submodule updates).

### Plating your broccoli (In Progress &#8594; Code Review)
**Final checks:**
* Am I following these [coding rules](cooking_rules.md#coding-rules)
* Am I editting core moodle code? [click here](cooking_rules.md#what-to-do)

**When you're done** 
- organize it to **one or several logical commits** (tip: [git squash](git_stuff.md#squashing-commits)). Use your senses :massage: .... When in doubt, ask Rex :raising_hand:
- `git push -u origin <branch_name>`
- Go to [moodle github](https://github.com/ucla/moodle) and copy the link of your commit
- [Go to Jira](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE)
  - Add screenshots if you're changing UI
  - Write out [test instructions](), before you forget lol
    - consider all possible cases of the problem
  - @\<reviewer\> \<ask to please review nicely\>: \<link to commit\>
  - Assign your peer reviewer and tester
  - Assign the ticket to your reviewer
  - Change the status from In Progress &#8594; Code Review
- Give yourself a pat in the back :clap: :relaxed:

### Please taste my broccoli (Passed Code Review)
When you've received your ticket back and it passed review
- Push to the `development` branch ([cmd](git_stuff.md#pushing-to-development))
- Make sure you have test instructions on [Jira](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE)
- @\<tester\> Please test \<possibly a cute emoji\>
- Assign your ticket to your tester
- Change the status from Code Review &#8594; Testing

### Reconsidering your friend's broccoli (Code Review)
- Understand the problem. Clarify with ticket owner
- Look for the link to the github commit
- Reconsider the broccoli
- [Peer review checklist](peer_review.md#peer-review-checklist)
- [Coding rules](cooking_rules.md#coding-rules)
- Make comments on Github or Jira as needed
- @\<owner\>
  - mention whether the broccoli looks good or not.
  - paste your [peer review checklist](peer_review.md#peer-review-checklist)
- Assign ticket back to owner
- If broccoli **looks good**: move to Testing\
  Else: move to In Progress

### Tasting your friend's broccoli (Testing)
- Understand the problem
- Make sure there are **Test Instructions** that considers all possible cases of the problem.
- NOW [TASTE](https://test.ccle.ucla.edu/) IT :tongue: :yum: :mask: 
- @\<owner\> and mention whether the broccoli is delicious or not
- Assign ticket back to owner
- If broccoli is **delicious**: move to Passed :white_check_mark:\
  Else: move to In Progress

### Cleaning your kitchen (Optional)
- Stop your local dev [(cmd)](docker_tips.md#stop-container)

### Getting more broccoli (Backlog)
When you have nothing left to do, you may 
* Go to the ([backlog](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE&view=planning.nodetail)) 
* Prioritize tickets that have more urgent MoSCoW ratings first
* Of the equivalent urgency tickets, choose the one you like most
* Assign yourself the ticket
* Change the *Sprint* to the current sprint
* Don't forget to move it to *In Progress*
### Found new broccoli (Creating new tickets)
When you find more issues that are unrelated to your ticket, please:
* Consult Rex and ask if new tickets can be created
* Click on the + button on the left pane
* Fill in the info
* Set the Sprint to *To Be Ranked (Future Sprint)*

----

## Outside Resources
### Git stuff
- [Git for dummies](https://github.com/k88hudson/git-flight-rules#flight-rules-for-git)
- [WTH is git rebase](https://git-rebase.io/)
- [Git Moodle Walkthrough](https://kb.ucla.edu/articles/ucla-git-walkthrough-for-moodle)
- [Git Squash](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html)
### Misc
- [Jira](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE)
- [Developer Subgroup](https://ccle.ucla.edu/course/view/CCLE_Subgroups?section=2)
### [Coding guidelines](cooking_rules.md#coding-rules)
### Docker stuff
- [Moodle Docker Setup](https://github.com/ccle/moodle-docker)

