---
# layout: post
title: "TIL: Add your git repo to a tarball"
excerpt: "Today I learned that you can neatly pack all of the files in your git repository into a tarball, automatically excluding files in your gitignore"
---

Today I learned that you can neatly pack all of the files in your git repository into a tarball:

```sh
git archive --format=tar -o my_repo.tar -v HEAD
```

The best thing about this is it will automatically honour your `.gitignore` file, so won't include any files you don't care about.

## Other formats

It also works with zip files:

```sh
git archive --format=zip -o my_repo.zip -v HEAD
```

## Including the git repo itself

It doesn't include the git repository itself (the `.git` directory). If you'd like to include it, you can run:

```sh
git archive --format=tar -o my_repo.tar -v HEAD
tar -rf my_repo.tar .git
```

## Sources

- https://stackoverflow.com/a/3069593/1688034
- https://stackoverflow.com/a/11621730/1688034
