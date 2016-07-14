# how to hub flow

* start new feature

```
$ git hf feature start another_feature

Fetching origin
Switched to a new branch 'feature/another_feature'
Total 0 (delta 0), reused 0 (delta 0)
To git@github.com:bfg/hf-example.git
 * [new branch]      feature/another_feature -> feature/another_feature

Summary of actions:
- A new branch 'feature/another_feature' was created, based on 'develop'
- The branch 'feature/another_feature' has been pushed up to 'origin/feature/another_feature'
- You are now on branch 'feature/another_feature'

Now, start committing on your feature. When done, create a
pull request on GitHub.  Once that has been merged, use:

     git hf feature finish another_feature
```

* do some commits

* push the code

```
$ git hf feature push

Fetching origin
Already up-to-date.
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 639 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To git@github.com:bfg/hf-example.git
   f1248de..fd563b8  feature/another_feature -> feature/another_feature

Summary of actions:
- The remote branch 'origin/feature/another_feature' was updated with your changes

```

* create Github pull request
* merge it
* finish the feature

```
$ git hf feature finish

Fetching origin
remote: Counting objects: 1, done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From github.com:bfg/hf-example
   f1248de..6928163  develop    -> origin/develop
Switched to branch 'develop'
Your branch is behind 'origin/develop' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
Updating f1248de..6928163
Fast-forward
 README.md | 52 ++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 52 insertions(+)
Already up-to-date.
To git@github.com:bfg/hf-example.git
 - [deleted]         feature/another_feature
Deleted branch feature/another_feature (was ad27936).

Summary of actions:
- The latest changes from 'origin' were merged into 'master' and 'develop'
- The feature branch 'feature/another_feature' was merged into 'develop'
- Feature branch 'feature/another_feature' has been removed
- Feature branch 'origin/feature/another_feature' has been removed
- You are now on branch 'develop'
```
