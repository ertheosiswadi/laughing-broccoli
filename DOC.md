# The Laughing Broccoli

Hello good people!
The following is a step-by-step walkthrough on how to make my life easier

## Table of Contents
1. Prepping your kitchen
2. Cooking your broccoli (In Progress)
3. Plating your broccoli (In Progress &#8594; Code Review)
## Resources
1. [Jira](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE)
2. [Developer Subgroup](https://ccle.ucla.edu/course/view/CCLE_Subgroups?section=2)
3. [Git Squash](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html)
4. [Moodle Coding Style](https://docs.moodle.org/dev/Coding_style)
5. [Git Moodle Walkthrough](https://kb.ucla.edu/articles/ucla-git-walkthrough-for-moodle)
6. [Moodle Docker Setup](https://github.com/ccle/moodle-docker)
7. [Git for dummies](https://github.com/k88hudson/git-flight-rules#flight-rules-for-git)
8. [WTH is git rebase](https://git-rebase.io/)


## Checklist

### Prepping your kitchen
- Monday? New sprint? [Checkout your new partners](https://ccle.ucla.edu/mod/page/view.php?id=815435)
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

## Making a better broccoli (Tips and Tricks)
* Surround commit with comments UCLA MOD:

## Junk
localhost:8000
localhost:8001 phpmyadmin
tips and tricks
git commands
summarize the moodle coding guidelines
All comments should end with a period
Do not use literal strings, use get_strings()
editting css, creating js files
Adding new tickets from the backlog
