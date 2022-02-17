### ds219sp2022

This is a repository for students in Spring 2022 DS 219

#### Be sure you've set your text editor in your local git config

This only has to be run once, it's a global git setting that will apply
to all of your local github repositories. In the below example,
[atom](https://blog.atom.io/2014/12/10/a-windows-installer-and-updater.html) is set.

`atom` is a common and easy-to-use editor, but you can set any editor you prefer.

```shell
git config --global core.editor "atom"
```

#### Fork then clone this repository

```shell
# fork first
git clone git@github.com:yourname/ds219sp2022.git
cd ds219sp2022
git remote add upstream git@github.com:sallyom/ds219sp2022.git
```

##### origin == your cloned fork

```
https://github.com/yourghusername/ds219sp2022
git@github.com:yourghusername/ds219sp2022
```

##### upstream == the original repository

```
https://github.com/sallyom/ds219sp2022
git@github.com:sallyom/ds219sp2022
```

#### Continually keep your local `main` branch up to date with upstream `main` branch

```shell
# this ensures your local working branch is current with latest upstream main branch
git checkout main
git fetch --all
git rebase upstream/main
git push origin main
```

#### Create a new branch for new work

```shell
git checkout -b my-new-branch
```

#### Continually keep your local and remote `my-new-branch` branch up to date with upstream main branch

```shell
git checkout my-new-branch
git fetch --all
git rebase upstream/main
# Now your local working branch will have current main branch + any commits you've added
git push --force-with-lease origin my-new-branch
```
