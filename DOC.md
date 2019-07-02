# The Laughing Broccoli

Hello good people!
The following is a step-by-step manual on how to make my life easier

## Resources
1. [Jira](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE)
2. [Developer Subgroup](https://ccle.ucla.edu/course/view/CCLE_Subgroups?section=2)
3. [Git Squash](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html)
4. [Moodle Coding Style](https://docs.moodle.org/dev/Coding_style)
5. [Git Moodle Walkthrough](https://kb.ucla.edu/articles/ucla-git-walkthrough-for-moodle)
6. [Moodle Docker Setup](https://github.com/ccle/moodle-docker)

## Checklist

### Prepping the broccoli
- [ ] Is today a Monday? Is it the start of a new sprint? [Checkout your new partners](https://ccle.ucla.edu/mod/page/view.php?id=815435)
- [ ] Let's checkout the [Jira board](https://ucla-ccle.atlassian.net/secure/RapidBoard.jspa?rapidView=1&projectKey=CCLE) to see what is up for today
  - Go from right to left. Prioritize tickets on **testing** or **code review**.
- [ ] Let's go terminal
- [ ] Start up your local DEV
- [ ] Log in to Slack
- [ ] Open your :heart: IDE


### Cooking the broccoli (In Progress)
- Read the ticket description
- Click on **Linked issues** (if exist) for reference or clarification
- @\<reporter\> to ask further questions
- Make sure you're in the right branch
  - `git branch` to check your current branch
  - If you're just starting the ticket: 
    1. `git checkout master`
    2. `git pull origin master`
    3. `git submodule update --init --recursive`
    4. `git checkout -b <patch/feature>/CCLE-<ticket#>-<short-ticket-description>`
  - Else: `git checkout <the ticket's branchname>`
- Cook the broccoli
#### Things to note: 
* Am I following [moodle coding guidelines](https://docs.moodle.org/dev/Coding_style)?
* Am I editting core moodle code? *link to file, with target*
  * If yes, am I surrounding your commits with the appropriate comments? End with a period.
  ```
  // START UCLA MOD: CCLE-8459 - Messaging does not email students.
  Your change here
  // END UCLA MOD: CCLE-8459.
  ```


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
