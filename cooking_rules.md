# Coding Guidelines

## Coding guidelines
- [CCLE Coding Standard](https://ccle.ucla.edu/mod/wiki/view.php?pageid=1639)
- Moodle Coding Style - [General or PHP](https://docs.moodle.org/dev/Coding_style),
[CSS](https://docs.moodle.org/dev/CSS_Coding_Style),
[JS](https://docs.moodle.org/dev/Javascript/Coding_Style),
[SQL](https://docs.moodle.org/dev/SQL_coding_style)
- [Code checker on DEV](http://localhost:8000/local/codechecker/index.php)
- [PHPdoc checker on DEV](http://localhost:8000/local/moodlecheck/index.php)

## Editting Core code
### What is core code?
Source: Tulasi\
Core code is all of the code that has **nothing** to do with UCLA. \
Code that is under local/ucla or theme/ucla** is our **custom code**
### What to do?
Look at the example below\
**Remember** that all comments must end with a **period.**
```
// START UCLA MOD: CCLE-8459 - Messaging does not email students.
Your change here
// END UCLA MOD: CCLE-8459.
```

