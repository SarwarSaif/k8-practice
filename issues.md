### Unable to merge branch
zen@zen-VirtualBox:~/projects/k8-practice$ git merge develop
fatal: refusing to merge unrelated histories
zen@zen-VirtualBox:~/projects/k8-practice$ git pull origin master --allow-unrelated-histories
From https://github.com/SarwarSaif/k8-practice
 * branch            master     -> FETCH_HEAD
Already up to date.
zen@zen-VirtualBox:~/projects/k8-practice$ git pull origin develop --allow-unrelated-histories
From https://github.com/SarwarSaif/k8-practice
 * branch            develop    -> FETCH_HEAD
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
zen@zen-VirtualBox:~/projects/k8-practice$ ^C
zen@zen-VirtualBox:~/projects/k8-practice$ git pull origin master --allow-unrelated-histories
From https://github.com/SarwarSaif/k8-practice
 * branch            master     -> FETCH_HEAD
Already up to date.
zen@zen-VirtualBox:~/projects/k8-practice$ git config pull.rebase false
zen@zen-VirtualBox:~/projects/k8-practice$ git merge develop
fatal: refusing to merge unrelated histories
zen@zen-VirtualBox:~/projects/k8-practice$ git pull origin develop --allow-unrelated-histories

### 