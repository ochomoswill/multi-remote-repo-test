
## Pushing to Multiple GIT Remotes

### Create a new remote called "all" with the URL of the primary repo.
git remote add all git@github.com:[username]/[repo].git
### Re-register the remote as a push URL.
git remote set-url --add --push all git@github.com:[username]/[repo].git
### Add a push URL to a remote. This means that "git push" will also push to this git URL.
git remote set-url --add --push all git@bitbucket.org:[username]/[repo].git
### To push to the two remotes
git push all [branch]


## Reference

[Multiple GIT Remote Repositories](https://jigarius.com/blog/multiple-git-remote-repositories)