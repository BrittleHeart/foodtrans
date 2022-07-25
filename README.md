# Introduction
TODO

## What is that repo?
FoodTrans's repo is a main repository for managing microservices:
So, that's go as follows:

If new modues are added, we're implementing changes to the file **<root-dir>/.gitmodules**,
and if it's needed, just create an pr. After code review, code is going to be deployed to main branch

## How to add new gitmodules?
Simple enough:

1. Go to .gitmodules file
2. Use the template below

```
[submodule "submodule-name"]
	path = <module-name>
	url = <repo-url>
```

or, if you rather prefer to use bash

```bash
$ git submodule add <repo-url>
$ git add .
$ git commit -m "Added Submodule 'submodule-name'"
$ git push origin <main-repo-url>
```

Create new pr, pray for merge 😎

## Currently planned modules
1. Auth
2. Filesystem
3. Bug reports
4. UI
5. CRON
6. Webserver

