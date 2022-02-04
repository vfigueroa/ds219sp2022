### ds219sp2022

#### This is a repository for students of DS 219

##### Fork then clone this repository

```shell
# fork first
git clone git@github.com:yourname/ds219sp2022.git
cd ds219sp2022
git remote add upstream git@github.com:sallyom/ds219sp2022.git

```

##### Create a new branch for new work

```shell
git checkout -b my-new-branch
```

###### Continually keep your local working branch up to date with upstream main branch

```shell
git fetch --all
git rebase upstream/main
# the above ensures your local working branch is current with latest changes in upstream main branch
```

##### When you are ready to push your local working branch to your GH repository

```shell
git push origin my-new-branch
```

##### Continually keep your local and remote `main` branch up to date with upstream main branch

```shell
git fetch --all
git rebase upstream/main
git push origin my-new-branch
```
