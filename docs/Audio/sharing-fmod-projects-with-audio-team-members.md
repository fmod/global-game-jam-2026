---
title: Sharing FMOD Projects
layout: home
parent: Audio Team
nav_order: 2.2
---
# Sharing FMOD Projects

If you want to collaborate on an FMOD project with another team member, you'll need to add the folder containing the `.fspro` file to version control.

If you're using Git either with GitHub or some other provider, we have a couple of recommended configurations to make your life easier.

## LFS

### Setup

Install [Git Large File Storage](https://git-lfs.com/) A.K.A. Git LFS.

You can check if Git LFS is installed by running `git lfs install` from the command line within your repository.

> _**NOTE:** GitHub Desktop users should have an option to open the repository in a Terminal/Command Line to get you here quickly._

### Configuration

We suggest tracking your audio source files with LFS.

If you don't already have one, create a file named `.gitattributes` in the same directory as your `.fspro` project file, and add the following contents:

```
# Auto detect text files and perform LF normalization
* text=auto

# Audio formats
*.mp3 filter=lfs diff=lfs merge=lfs -text
*.ogg filter=lfs diff=lfs merge=lfs -text
*.wav filter=lfs diff=lfs merge=lfs -text
*.aiff filter=lfs diff=lfs merge=lfs -text
*.aif filter=lfs diff=lfs merge=lfs -text
*.mod filter=lfs diff=lfs merge=lfs -text
*.it filter=lfs diff=lfs merge=lfs -text
*.s3m filter=lfs diff=lfs merge=lfs -text
*.xm filter=lfs diff=lfs merge=lfs -text
```

If you know that you'll be using another audio file format, you may want to add that file extension by following the same pattern here. For example, you might add another line `*.pcm filter=lfs diff=lfs merge=lfs -text` if you are working with `.pcm` files.

## Ignore

We suggest ignoring a few folders that FMOD Studio uses but should not be committed.

If you don't already have one, create a file named `.gitignore` in the same directory as your `.fspro` project file, and add the following contents:

```
# FMOD Cached files
.cache/*
.user/*
.unsaved/*
``` 

### Ignoring Banks

If you want to ignore built Banks to slim down your commit size for a jam, you can also ignore the Builds folder and elect to send built banks to your development team ad-hoc.

```
Builds/*
```
