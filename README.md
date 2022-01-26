# training-test

This is a test repository. It only has a few roles:

-   demonstrate how to create a repository in GitHub
-   practice with a commit
-   later, we'll see how to access the repository in RStudio

# Git from RStudio

From within RStudio, we can perform the same versioning actions that we can in GitHub, and much more. Plus, we have the natural advantages of the programming IDE with code completion and other features to make our work easier.

-   Add files to version control
-   Commit changes
-   Push commits to GitHub

# Typical Git Commands
The following are useful and commonly used `git` commands for the command line.
  - `git clone`: to copy a whole repository to local system
  - `git add`: notify git to track particular changes (same as stage)
  - `git commit`: store those changes as a version
  - `git pull`: merge changes from a remote repository to a local repository
  - `git push`: copy changes from a local repo to a remote repo
  - `git status`: determine the state of all files in the local repo
  - `git log`: print the history of changes in a repo

# Resolving Conflict in Git

When there is a merge conflict, the repository is placed in a "Merging" state until the issue gets resolved. The abort the merge altogether, enter the following into the command line: <center>`git merge --abort`</center>
<br>
If you know which version of the code creating the merge conflict you would like to use, you can perform the following `git` commands. <br>To keep the collaborators file, run `git checkout --theirs conflicted_file.Rmd`. If you want to keep your own file, run `git checkout --ours conflicted_file.Rmd`. Then, you can stage, commit, push as normal.

# Workflows to Avoid Merge Conflicts
Aside from frequent communication with team members, follow this workflow:
<center>`Pull -> Edit -> Add(Stage) -> Pull -> Commit -> Push`</center>
<br>
Make sure to always pull at the beginning of working sessions, and commit often in small code chunks. 

# GitHub Etiquette
Cloning a collaborator's repository is fine and appropriate when the two collaborators are personally close with one another. However, a more appropriate method of using GitHub with collaborators that have a working relationship (rather than a personal one) typically feel more inclined to `fork` anothers repository. This allows less access to the files within the owner's original repository itself, and works analogous to suggesting changes in a Google Doc, rather than outright editing one. 
<br>

Once a collaborator has forked a repository, they then must clone it normally to their local machine. This allows the collaborator to have an "original" version of their Owner's repository that the collaborator can edit freely, without making final changes to the Owner's repository. The Owner can then pull from the collaborators repository, but allows the Owner to remain in control of precisely what's changed.

# Data Modeling & Tidy Data
<u> What is a relational data model?</u> Relational databases -- such as SQL, Oracle, or Microsoft Access -- use relational data models to organize tables. Relational data models allow for powerful search and filtering; handling large, complex data sets; enforcing data integrity; and reducing redundancy.

<u> What is tidy data?</u> Tidy data are data that are designed in such a way that each column is a variable, and each row is an observation or a data point. Additionally, columns contain <i>only one</i> type of information, and a single piece of data is recorded only once.

# Merging Data
  - <b><u>Inner Join:</b></u> An inner join occurs when you merge a subset of rows that have matching data in both tables being merged.
  - <b><u>Left Join:</b></u> A left join takes all rows from the left table, and merges the data from matching rows in the right table. If keys don't match from the left table, the data is presented as a missing value (NA) from the right table.
  - <b><u>Right Join:</b></u> A right join is the exact same, in the reverse direction.
  - <b><u>Outer Join:</b></u> An outer join includes all data from all rows in both tables, including missing values where necessary.