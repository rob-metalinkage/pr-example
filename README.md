# pr-example
Repo to demonstrate and example of how to commit a PR from a fork to the master

- with this edit to form a PR against the original upstream master

Process:

(assuming you have a fork of a PR you want to sent a PR to)

1. Create branch in your fork,
2. Create a local working copy of this branch - from an existing checkout use
```git fetch my-new-branch```
3. sync this branch to the upstream master (you will create a PR against)

```
git remote add upstream https://github.com/rob-metalinkage/pr-example/tree/main
git fetch upstream

```
4. make changes to the specific files that you want to create a PR to accept upstream
5. run any local testing
6. commit and push to fork branch
7. create a PR **on your fork** to main/master (for testing github automations on main)
8. create a PR **on the upstream master** from your **branch**

Note that when PR is accepted on main of both upstream and fork main/master branches these will automatically handled cleanly when syncing fork to master 
