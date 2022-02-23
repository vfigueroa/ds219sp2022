### ds219sp2022

#### Assignment Due Feb.23

Before beginning, make sure your local and origin `main` branches are up to date. Refer to 
[README.md](https://github.com/sallyom/ds219sp2022/blob/main/README.md)

#### Create a new branch for new work

```shell
git checkout -b my-new-branch
```

#### Add a file to your clone or fork of this repository in the `how-to-contribute` folder.

```shell
<editor> how-to-contribute/yourname.md
```
In this file, answer the question from the [L04 Lesson Notes](https://piazza.com/class_profile/get_resource/kyeyevqkher3wa/kzpyerxrucx6i2), Slide #15

#### When you are ready to commit and push your local working branch to your GH repository

```shell
git add .
git commit -m "name-how-to-contribute-assignment"
git push origin my-new-branch
```

#### Submit a Pull Request to the upstream repository

```
This you will most likely do from the GitHub site
```

#### After the initial push of your branch to GH, you will have to use `--force-with-lease` for any other pushes.

Read [here](https://blog.developer.atlassian.com/force-with-lease/) for more information about force pushing.

```shell
git push --force-with-lease origin my-new-branch
```

#### To get back to your main branch

You won't be able to check out a branch unless the branch you are currently working
in is clean, ie, you've commited all changes locally

```shell
git checkout main
```
