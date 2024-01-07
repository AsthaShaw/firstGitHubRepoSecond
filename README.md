This is a demo

git divergent branches - when does branches gets diverse when they have separate commits. So you need to reconcile too

1. git pull origin main   (did not work)

2. git rebase- this will reapply your local commits on the top of the remote branches commits. This can create a cleaner history but may require resolving conflicts

3. Fast Forward (ff only)- This will only perform a pull if it can be done using a fat forward merge, which implies that your local branch is behind the remote and has no additional commits

git pull --ff-only origin main


git pull --rebase origin main

git log —oneline really cool

This video is a good reference for divergent branches
https://www.youtube.com/watch?v=HzBoMI7yqsU&t=50s