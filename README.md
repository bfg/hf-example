# this is readme.

# another section

# p3

trololo

# p4

haha

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
```
