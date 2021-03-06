# Jason

## Table of Contents

- [Jason](#jason)
  - [Table of Contents](#table-of-contents)
  - [About ](#about)
  - [Getting Started ](#getting-started)
    - [Installing](#installing)

## About <a name = "about"></a>

I'm storing ugly pictures of heads in a git repository.

## Getting Started <a name = "getting_started"></a>

These instructions are for design file management.

### Installing

Set up new repository with Git LFS, which is a way to manage large files.

* Set up a new repository
* Follow the steps for setting up Git LFS
```
$ git lfs
$ git lfs install
```
* List out all of the types of files you anticipate you will need to track. Sketch, Illustrator and Photoshop files can be huge. I would also recommend listing any prototyping software files.
```
git lfs track “*.psd”
git lfs track “*.sketch”
git lfs track “*.ai”
```
* Make sure that .gitattributes is tracked
```
git add .gitattributes
```
* Now you’re ready to push up your changes. First initialize GIT LFS with `$ git lfs`
* Commit and push your changes `git add file.psd` `git commit -m "Add design file"`
* push up your changes using the below
```
GIT_TRACE=1 GIT_CURL_VERBOSE=1 git push -u origin master
```


