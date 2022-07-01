
# Pushing to Multiple GIT Remotes

Create a new remote called "all" with the URL of the primary repo.

```bash
git remote add all git@github.com:[username]/[repo].git
```

Re-register the remote as a push URL.

```bash
git remote set-url --add --push all git@github.com:[username]/[repo].git
```

Add a push URL to a remote. This means that "git push" will also push to this git URL.

```bash
git remote set-url --add --push all git@bitbucket.org:[username]/[repo].git
```

To push to the two remotes

```bash
git push all [branch]
```

## Reference

[Multiple GIT Remote Repositories](https://jigarius.com/blog/multiple-git-remote-repositories)
[Pushing to Multiple Git Repos](https://gist.github.com/rvl/c3f156e117e22a25f242)
