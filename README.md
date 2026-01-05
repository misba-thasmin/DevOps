
1.C:\Users\Admin\Desktop\DevOps>git init
Initialized empty Git repository in C:/Users/Admin/Desktop/DevOps/.git/

2.C:\Users\Admin\Desktop\DevOps>code .

3.C:\Users\Admin\Desktop\DevOps>git add config.js

4.C:\Users\Admin\Desktop\DevOps>git commit -m "first commit"
[master (root-commit) 53f53f2] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 config.js

5.C:\Users\Admin\Desktop\DevOps>git lg
git: 'lg' is not a git command. See 'git --help'.

The most similar command is
        log

6.C:\Users\Admin\Desktop\DevOps>git log
commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (HEAD -> master)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:26:13 2026 +0530

    first commit

7.C:\Users\Admin\Desktop\DevOps>git branch new-branch

8.C:\Users\Admin\Desktop\DevOps>git branch
* master
  new-branch

9.C:\Users\Admin\Desktop\DevOps>git checkout new-branch
Switched to branch 'new-branch'

10.C:\Users\Admin\Desktop\DevOps>git add config.js

11.C:\Users\Admin\Desktop\DevOps>git commit -m "second commit"
[new-branch 3cec210] second commit
 1 file changed, 1 insertion(+)

12.C:\Users\Admin\Desktop\DevOps>git log --all --graph
* commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (HEAD -> new-branch)
| Author: misba-thasmin <thasminmisbha@gmail.com>
| Date:   Mon Jan 5 21:29:26 2026 +0530
|
|     second commit
|
* commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
  Author: misba-thasmin <thasminmisbha@gmail.com>
  Date:   Mon Jan 5 21:26:13 2026 +0530

      first commit

13.C:\Users\Admin\Desktop\DevOps>git branch b1

14.C:\Users\Admin\Desktop\DevOps>git branch
  b1
  master
* new-branch

15.C:\Users\Admin\Desktop\DevOps>git checkout b1
Switched to branch 'b1'

16.C:\Users\Admin\Desktop\DevOps>git add config.js

17.C:\Users\Admin\Desktop\DevOps>git commit -m "third commit"
[b1 59786c4] third commit
 1 file changed, 2 insertions(+), 1 deletion(-)

18.C:\Users\Admin\Desktop\DevOps>git branch
* b1
  master
  new-branch

19.C:\Users\Admin\Desktop\DevOps>git log --all --graph
* commit 59786c4d4fd505639a974514a0ef48db589de175 (HEAD -> b1)
| Author: misba-thasmin <thasminmisbha@gmail.com>
| Date:   Mon Jan 5 21:32:12 2026 +0530
|
|     third commit
|
* commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (new-branch)
| Author: misba-thasmin <thasminmisbha@gmail.com>
| Date:   Mon Jan 5 21:29:26 2026 +0530
|
|     second commit
|
* commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
  Author: misba-thasmin <thasminmisbha@gmail.com>
  Date:   Mon Jan 5 21:26:13 2026 +0530

      first commit

20.C:\Users\Admin\Desktop\DevOps>git checkout new-branch
Switched to branch 'new-branch'

21.C:\Users\Admin\Desktop\DevOps>git merge master
Already up to date.

22.C:\Users\Admin\Desktop\DevOps>git log
commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (HEAD -> new-branch)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:29:26 2026 +0530

    second commit

commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:26:13 2026 +0530

    first commit

23.C:\Users\Admin\Desktop\DevOps>git merge new-branch
Already up to date.

24.C:\Users\Admin\Desktop\DevOps>git log
commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (HEAD -> new-branch)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:29:26 2026 +0530

    second commit

commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:26:13 2026 +0530

    first commit

25.C:\Users\Admin\Desktop\DevOps>git merge main
merge: main - not something we can merge

26.C:\Users\Admin\Desktop\DevOps>git log
commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (HEAD -> new-branch)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:29:26 2026 +0530

    second commit

commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:26:13 2026 +0530

    first commit

27.C:\Users\Admin\Desktop\DevOps>git config --global user.name "misba-thasmin"

28.C:\Users\Admin\Desktop\DevOps>git config --global user.email "thasminmisbha@gmail.com"

29.C:\Users\Admin\Desktop\DevOps>git log --all --graph
* commit 59786c4d4fd505639a974514a0ef48db589de175 (b1)
| Author: misba-thasmin <thasminmisbha@gmail.com>
| Date:   Mon Jan 5 21:32:12 2026 +0530
|
|     third commit
|
* commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (HEAD -> new-branch)
| Author: misba-thasmin <thasminmisbha@gmail.com>
| Date:   Mon Jan 5 21:29:26 2026 +0530
|
|     second commit
|
* commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
  Author: misba-thasmin <thasminmisbha@gmail.com>
  Date:   Mon Jan 5 21:26:13 2026 +0530

      first commit

30.C:\Users\Admin\Desktop\DevOps>git checkout b1
Switched to branch 'b1'

31.C:\Users\Admin\Desktop\DevOps>git merge main
merge: main - not something we can merge

32.C:\Users\Admin\Desktop\DevOps>git log
commit 59786c4d4fd505639a974514a0ef48db589de175 (HEAD -> b1)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:32:12 2026 +0530

    third commit

commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (new-branch)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:29:26 2026 +0530

    second commit

commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:26:13 2026 +0530

    first commit

33.C:\Users\Admin\Desktop\DevOps>git merge master
Already up to date.

C:\Users\Admin\Desktop\DevOps>git log
commit 59786c4d4fd505639a974514a0ef48db589de175 (HEAD -> b1)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:32:12 2026 +0530

    third commit

commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (new-branch)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:29:26 2026 +0530

    second commit

commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
Author: misba-thasmin <thasminmisbha@gmail.com>
Date:   Mon Jan 5 21:26:13 2026 +0530

    first commit

34.C:\Users\Admin\Desktop\DevOps>git log --all --graph
* commit 59786c4d4fd505639a974514a0ef48db589de175 (HEAD -> b1)
| Author: misba-thasmin <thasminmisbha@gmail.com>
| Date:   Mon Jan 5 21:32:12 2026 +0530
|
|     third commit
|
* commit 3cec210c3bb9a5821f1c34f5d9b7ae963fefa453 (new-branch)
| Author: misba-thasmin <thasminmisbha@gmail.com>
| Date:   Mon Jan 5 21:29:26 2026 +0530
|
|     second commit
|
* commit 53f53f2b0511d4e7e8d04698bfe07c4f76760d0c (master)
  Author: misba-thasmin <thasminmisbha@gmail.com>
  Date:   Mon Jan 5 21:26:13 2026 +0530

      first commit

35.C:\Users\Admin\Desktop\DevOps>git remote add origin https://github.com/misba-thasmin/DEvOPs-projewct.git

36.C:\Users\Admin\Desktop\DevOps>git push origin
fatal: The current branch b1 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin b1

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


37.C:\Users\Admin\Desktop\DevOps>git push --set-upstream origin b1
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (9/9), 728 bytes | 145.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'b1' on GitHub by visiting:
remote:      https://github.com/misba-thasmin/DEvOPs-projewct/pull/new/b1
remote:
To https://github.com/misba-thasmin/DEvOPs-projewct.git
 * [new branch]      b1 -> b1
branch 'b1' set up to track 'origin/b1'.

38.C:\Users\Admin\Desktop\DevOps>git push -u origin b1
branch 'b1' set up to track 'origin/b1'.
Everything up-to-date
