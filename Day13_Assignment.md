
# Assignment:

## Git Merge
- Marge has all of the different commits from the feature branch are combined into one branch's history through the merge process. It generates a "merge commit," which is a new commit on the target branch.
— This tactic is straightforward and simple to understand. The most common use case for it is when team members need to update shared feature branches.
— However, the history becomes cluttered with merge commits, and debugging with “git bisect” can be more challenging due to the extra commits.
— Use Merge when updating a shared feature branch to avoid recalculating commit hashes that could lead to conflicts for others.
— Use Merge when updating a feature branch that is significantly behind the target branch, as resolving conflicts during rebase might be more difficult.

<img src = 'https://miro.medium.com/v2/resize:fit:720/format:webp/0*qS37ldEO_QdD4OLU.png'>

## Git Rebase
- Rebase replays the feature branch's commits on top of the target branch's most recent commit. Every commit on the feature branch generates a new commit hash. 
- It leads to a cleaner commit history because it avoids combining commits. It is generally not advised to share the feature branch with others, though, as this may result in faulty repositories for other users. 
- Rebase helps to uncover conflicts sooner because they are resolved when the changes are replayed onto the target branch.
- Use Rebase when updating a feature branch that is not shared with others. It keeps the branch history clean and easier to manage.

<img src = 'https://miro.medium.com/v2/resize:fit:720/format:webp/0*W28uicsv40QTx7vx.png'/>

### git rebase -i
-  if you want to change the last three commit messages, or any of the commit messages in that group, you supply as an argument to git rebase -i the parent of the last commit you want to edit, which is HEAD~2^ or HEAD~3


## Git Squash
- Squash creates a single commit with a fresh commit message by combining every individual commit from the feature branch. 
- The commit history from the feature branch is not carried over. This method helps to make it easier to track and locate changes when necessary by combining the feature branch updates into a single commit. 
- Squash is usually utilized together with `Rebase} or `Merge}.
- Use Squash when merging feature branch changes into the target branch. It creates a single commit for all the changes, making it easier to track.

<img src =
 "https://miro.medium.com/v2/resize:fit:720/format:webp/0*1-txFxO3qi5KbvAB.png" />


## Forks
- What are Forks, and why are they used
- A fork is a new repository that is linked to the original "upstream" repository using the same code and visibility settings.
- Forks are frequently used to iterate on ideas or modifications before proposing them back to the upstream repository, as in open source projects or when a user does not have write access to the upstream repository.
- For example, you can use forks to propose changes related to fixing a bug. Rather than logging an issue for a bug you have found, you can:
    - Fork the repository.
        - Make the fix.
        - Submit a pull request to the project owner.

## References
- Shikha, R. (2023, August 5). “Git Rebase vs Merge vs Squash: Choosing the Right Strategy for Version Control.” Medium. https://medium.com/@shikha.ritu17/git-rebase-vs-merge-vs-squash-choosing-the-right-strategy-for-version-control-a9c9bb97040e
- Git - Rewriting History. (n.d.). https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History
- Terra, J. (2023, October 12). Git Rebase vs. Merge: A Complete Guide. Simplilearn.com. https://www.simplilearn.com/git-rebase-vs-merge-article#:~:text=Thus%2C%20the%20squash%20and%20merge,the%20history%20to%20reflect%20this.
- Fork a repository - GitHub Docs. (n.d.). GitHub Docs. https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo