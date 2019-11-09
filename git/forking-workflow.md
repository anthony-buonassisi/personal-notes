# forking-workflow

[Atlassian tutorial](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)

Each contributer has two Git repos:
* origin: private local repo
* upstream: public server-side repo

Process:
Central repo is forked and cloned once. After that, update local repo then update upstream.
1. fork the official repo
* select 'fork' option in GitHub
2. clone this forked repo onto local machine
* `git clone https://github.com/USER/REPO.git`
3. add official repo as upstream, cloned repo is origin by default
* `git remote add upstream git://github.com/REPO.git`
4. create local branch
* `git checkout -b BRANCH-NAME`
5. commit and push to forked repo
* `git commit`
* `git push origin`
6. open a PR to the official repo
* create PR in GitHub
7. PR is reviewed and merged by official repo maintainer
8. Check for updates from upstream repo
* `git fetch upstream`
9. Get updates from upstream repo
* `git pull upstream`

