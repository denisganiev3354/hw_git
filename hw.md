PS C:\Users\301FPS\Desktop\hw_git> git init
Initialized empty Git repository in C:/Users/301FPS/Desktop/hw_git/.git/
On branch master

No commits yet

Untracked files:
  (use "git add `<file>`..." to include in what will be committed)
        .gitignore
        README.md

PS C:\Users\301FPS\Desktop\hw_git> git status

On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached `<file>`..." to unstage)
        new file:   .gitignoregit
        new file:   README.md

PS C:\Users\301FPS\Desktop\hw_git> git status
On branch master
Untracked files:
  (use "git add `<file>`..." to include in what will be committed)
        main.py

nothing added to commit but untracked files present (use "git add" to track)

PS C:\Users\301FPS\Desktop\hw_git> git add .
PS C:\Users\301FPS\Desktop\hw_git> git commit -m "Add main.py"
[master e237cfd] Add main.py
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 main.py
PS C:\Users\301FPS\Desktop\hw_git> git status
On branch master
nothing to commit, working tree clean

PS C:\Users\301FPS\Desktop\hw_git> git log

commit e237cfd370a9904c9cd8e506c99d426229d4d82a (HEAD -> master)

Author: Casper3354 <denisganiev3354@gmail.com>

Date:   Mon Feb 9 20:01:54 2026 +0300

    Add main.py

commit cdead553b9f70dc073a13a1e33e768f738dfe084

Author: Casper3354 <denisganiev3354@gmail.com>

Date:   Mon Feb 9 19:57:40 2026 +0300

    frist commit

PS C:\Users\301FPS\Desktop\hw_git> git log
commit e237cfd370a9904c9cd8e506c99d426229d4d82a (HEAD -> master)
Author: Casper3354 <denisganiev3354@gmail.com>
Date:   Mon Feb 9 20:01:54 2026 +0300

    Add main.py

commit cdead553b9f70dc073a13a1e33e768f738dfe084
Author: Casper3354 <denisganiev3354@gmail.com>
Date:   Mon Feb 9 19:57:40 2026 +0300

    frist commit

///////////////////////////////////////////////////////////////////////////////////

PS C:\Users\301FPS\Desktop\hw_git> git status

On branch master

Changes not staged for commit:

    modified:   main.py



  (use "git add <file>..." to include in what will be committed)

    hw.md

no changes added to commit (use "git add" and/or "git commit -a")

PS C:\Users\301FPS\Desktop\hw_git> git add . 

[master efc570f] add all files

 2 files changed, 83 insertions(+)

 create mode 100644 hw.md

PS C:\Users\301FPS\Desktop\hw_git> git status

nothing to commit, working tree clean

fatal: No remote for the current branch.

PS C:\Users\301FPS\Desktop\hw_git> git branch

PS C:\Users\301FPS\Desktop\hw_git> git checkout -b feature/logic

Switched to a new branch 'feature/logic'

PS C:\Users\301FPS\Desktop\hw_git> gti branch

gti : Имя "gti" не распознано как имя командлета, функции, файла сценария или выполняемой 

после чего повторите попытку.

строка:1 знак:1

+ gti branch

    + CategoryInfo          : ObjectNotFound: (gti:String) [], CommandNotFoundException

    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\301FPS\Desktop\hw_git> git branch

* feature/logic

  master

PS C:\Users\301FPS\Desktop\hw_git> git status

On branch feature/logic

Changes not staged for commit:

  (use "git add <file>..." to update what will be committed)

  (use "git restore <file>..." to discard changes in working directory)

    modified:   main.py



no changes added to commit (use "git add" and/or "git commit -a")

PS C:\Users\301FPS\Desktop\hw_git> git commit -m "commit in new branch"

On branch feature/logic

Changes not staged for commit:

  (use "git add <file>..." to update what will be committed)

  (use "git restore <file>..." to discard changes in working directory)

    modified:   main.py



no changes added to commit (use "git add" and/or "git commit -a")

PS C:\Users\301FPS\Desktop\hw_git> git add .

PS C:\Users\301FPS\Desktop\hw_git> git commit -m "commit in new branch"

[feature/logic 0e09257] commit in new branch

 1 file changed, 3 insertions(+), 3 deletions(-)

PS C:\Users\301FPS\Desktop\hw_git> git status

On branch feature/logic

nothing to commit, working tree clean

PS C:\Users\301FPS\Desktop\hw_git> git branch -a

* feature/logic

  master

PS C:\Users\301FPS\Desktop\hw_git> git log --oneline --graph --all

* 0e09257 (HEAD -> feature/logic) commit in new branch

* efc570f (master) add all files

* e237cfd Add main.py

* cdead55 frist commit

PS C:\Users\301FPS\Desktop\hw_git> git checkout master

Switched to branch 'master'

PS C:\Users\301FPS\Desktop\hw_git> git status

On branch master

nothing to commit, working tree clean

PS C:\Users\301FPS\Desktop\hw_git> git merge feature/logic

Updating efc570f..0e09257

Fast-forward

 main.py | 6 +++---

 1 file changed, 3 insertions(+), 3 deletions(-)

PS C:\Users\301FPS\Desktop\hw_git> git status

On branch master

nothing to commit, working tree clean

PS C:\Users\301FPS\Desktop\hw_git> git commit -m "Merge branch 'feature/logic' into master" 



On branch master

nothing to commit, working tree clean

PS C:\Users\301FPS\Desktop\hw_git> git log

commit 0e09257aa5e143bbddfa53d463926cf9cbff50d8 (HEAD -> master, feature/logic)

Author: Casper3354 <denisganiev3354@gmail.com>

Date:   Mon Feb 9 20:59:44 2026 +0300



    commit in new branch



commit efc570f06851ec333a382df4101785d191034e99

Author: Casper3354 <denisganiev3354@gmail.com>

Date:   Mon Feb 9 20:53:49 2026 +0300



    add all files



commit e237cfd370a9904c9cd8e506c99d426229d4d82a

Author: Casper3354 <denisganiev3354@gmail.com>

Date:   Mon Feb 9 20:01:54 2026 +0300



    Add main.py



commit cdead553b9f70dc073a13a1e33e768f738dfe084

Author: Casper3354 <denisganiev3354@gmail.com>

Date:   Mon Feb 9 19:57:40 2026 +0300



    frist commit

PS C:\Users\301FPS\Desktop\hw_git>

PS C:\Users\301FPS\Desktop\hw_git> git status
On branch master
Changes not staged for commit:
        modified:   main.py

  (use "git add `<file>`..." to include in what will be committed)
        hw.md
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\301FPS\Desktop\hw_git> git add .
[master efc570f] add all files
 2 files changed, 83 insertions(+)
 create mode 100644 hw.md
PS C:\Users\301FPS\Desktop\hw_git> git status
nothing to commit, working tree clean
fatal: No remote for the current branch.
PS C:\Users\301FPS\Desktop\hw_git> git branch
PS C:\Users\301FPS\Desktop\hw_git> git checkout -b feature/logic
Switched to a new branch 'feature/logic'
PS C:\Users\301FPS\Desktop\hw_git> gti branch
gti : Имя "gti" не распознано как имя командлета, функции, файла сценария или выполняемой
после чего повторите попытку.
строка:1 знак:1

+ gti branch
  + CategoryInfo          : ObjectNotFound: (gti:String) [], CommandNotFoundException
  + FullyQualifiedErrorId : CommandNotFoundException
    PS C:\Users\301FPS\Desktop\hw_git> git branch

* feature/logic
  master
  PS C:\Users\301FPS\Desktop\hw_git> git status
  On branch feature/logic
  Changes not staged for commit:
  (use "git add `<file>`..." to update what will be committed)
  (use "git restore `<file>`..." to discard changes in working directory)
  modified:   main.py

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\301FPS\Desktop\hw_git> git commit -m "commit in new branch"
On branch feature/logic
Changes not staged for commit:
  (use "git add `<file>`..." to update what will be committed)
  (use "git restore `<file>`..." to discard changes in working directory)
        modified:   main.py

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\301FPS\Desktop\hw_git> git add .
PS C:\Users\301FPS\Desktop\hw_git> git commit -m "commit in new branch"
[feature/logic 0e09257] commit in new branch
 1 file changed, 3 insertions(+), 3 deletions(-)
PS C:\Users\301FPS\Desktop\hw_git> git status
On branch feature/logic
nothing to commit, working tree clean
PS C:\Users\301FPS\Desktop\hw_git> git branch -a

* feature/logic
  master
  PS C:\Users\301FPS\Desktop\hw_git> git log --oneline --graph --all
* 0e09257 (HEAD -> feature/logic) commit in new branch
* efc570f (master) add all files
* e237cfd Add main.py
* cdead55 frist commit
  PS C:\Users\301FPS\Desktop\hw_git> git checkout master
  Switched to branch 'master'
  PS C:\Users\301FPS\Desktop\hw_git> git status
  On branch master
  nothing to commit, working tree clean
  PS C:\Users\301FPS\Desktop\hw_git> git merge feature/logic
  Updating efc570f..0e09257
  Fast-forward
  main.py | 6 +++---
  1 file changed, 3 insertions(+), 3 deletions(-)
  PS C:\Users\301FPS\Desktop\hw_git> git status
  On branch master
  nothing to commit, working tree clean
  PS C:\Users\301FPS\Desktop\hw_git> git commit -m "Merge branch 'feature/logic' into master"

On branch master
nothing to commit, working tree clean
PS C:\Users\301FPS\Desktop\hw_git> git log
commit 0e09257aa5e143bbddfa53d463926cf9cbff50d8 (HEAD -> master, feature/logic)
Author: Casper3354 <denisganiev3354@gmail.com>
Date:   Mon Feb 9 20:59:44 2026 +0300

    commit in new branch

commit efc570f06851ec333a382df4101785d191034e99
Author: Casper3354 <denisganiev3354@gmail.com>
Date:   Mon Feb 9 20:53:49 2026 +0300

    add all files

commit e237cfd370a9904c9cd8e506c99d426229d4d82a
Author: Casper3354 <denisganiev3354@gmail.com>
Date:   Mon Feb 9 20:01:54 2026 +0300

    Add main.py

commit cdead553b9f70dc073a13a1e33e768f738dfe084
Author: Casper3354 <denisganiev3354@gmail.com>
Date:   Mon Feb 9 19:57:40 2026 +0300

    frist commit
PS C:\Users\301FPS\Desktop\hw_git>
