# keep your fork in sync

suppose `$THIS_REPO` is the url you get when you click on 'clone this repo'.
create a fork (unless you already did), and suppose `$YOUR_FORK` is the url
you get from cloning it. at a command line, do:

```
git clone $YOUR_FORK
git remote add upstream $THIS_REPO
git fetch upstream
git merge upstream/master
git push origin
```

all copies of your fork (i.e. the one on github, and the one cloned to your local)
should now have the latest changes from `origin`.

but watch out for merge conflicts!
