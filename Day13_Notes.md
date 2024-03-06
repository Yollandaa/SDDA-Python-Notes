# Notes
- Mobile first -> it is still usable on desktop as compared to the other way around.

## Git
- Source control System
- Created by Linus torvalds, who also created Linux system
- What is special:
    - Offers you save points -> commits
    - 3 parts: working -> stage -> commit -> push
    - The rule is to do small commits and commit often -> 
- git init -> Creates the hidden file .git -> To track changes
- git add .
- git log -> Check commits made
- git checkout "commit #" -> go back to commit
    - if i do git checkout - -> goes back to previous checkout
- master points at the latest commit, and the commit you checked out
- git checkout - -> goes back to master
- Stuff we did:
    - git init
    - git add .
    - git commit -m "This is my first project with git"
    - git add .
    - git commit -m "Created double function"
    - git log
    - git add .
    - git commit -m "Cool file with awesome msg"
    - git log
    - git checkout c7f9f09860
    - git checkout -
    - git log
- --hard option: If you want to reset to the last commit and also remove all unstaged changes.
- The --soft option means that you will not lose the uncommitted changes you may have.
- git log --help -> git out about the git commands
- git log -Sprint -> Gets all the commits with print in them (inside code)
- git log -Sdouble -p
- pick-asxe
- git log -2
- Fliter by author name
- /map to find
- n - next match
- Different working branches:
    - master branch -> you make no commit here
    - staging banch
    - feature branch/dev branch -> Done here you merge to staging branch
- git cm "Some message" -> combines git add and git commit
- Checkout to the master branch (old)
- Merge with dev branch (new)
- Fast forward merge - no conflicts, no one commited to master while you were working on dev.
- Merge Conflict
    -Resolve
    - Stage
    - Commit
    - to see how the changes happened -> git log --graph
- git push --all -> to push all branches
- Git: Git is a distributed version control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows. 
- GitHub: GitHub is a web-based Git repository hosting service, which offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features. -> File storage space.

# Database
- Special software to store data.
- You can't store your database in your laptop, because of RAM
- Cloud is about renting PC
    - Google
    - Azure
    - AWS
    - and other cloud services companies
- Why rent instead of buying:
    - High initial cost
    - Mantainance
    - Power bill
    - Rent room, AC
- Advantage of open source -> Collaborative work, if there's a bug everyone jumps to fix it cuz they don't want to lose data.


## Asignment:
- Rebase and merge and squash and merge and how are they different from normal merge
- rebase, Squash - Normal Merge
- What are Forks, and why are they used
- git rebase -i