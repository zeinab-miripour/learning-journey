🌱 My Learning Journey

Hello! I'm a Computer Engineering student.

This repository documents my learning journey as I continuously improve my technical skills and work toward becoming a better software engineer through consistent learning and practice.

I have basic knowledge of Python, C++, Java, HTML, and CSS, and my goal is to strengthen these skills while continuously learning new technologies.

I am starting this journey with Git. Along the way, I will share my notes, practice, projects, and progress.

📅 Day 1 – Git

What I learned today

- What Git is
- What a commit is
- The philosophy behind commits
- How to write a good commit message

Key Takeaway

Today I learned that Git is much more than a tool for storing code. It is a version control system designed to track changes, make development safer, simplify collaboration, and allow developers to experiment with confidence without worrying about losing their work.

---

📅 Day 2 

📘 Git Learning Journey – Session 2

Today, I learned the core concepts of Git and several essential commands.

What I Learned

- Initialized a Git repository using git init.
- Learned that git init creates a hidden .git folder, which stores Git metadata and the project's history.
- Used git --version to check the installed Git version and verify the installation.
- Used git status to check the current state of a repository.
- Learned that git add starts tracking files and prepares changes for a commit.
- Used git commit -m "message" to save staged changes in Git history.
- Used git log to view the commit history.

Basic Terminal Commands

- mkdir – Create a new directory.
- ls -a – List all files, including hidden files.
- echo "text" > file.txt – Create a new file or overwrite its content.
- echo "text" >> file.txt – Append text to the end of a file.
- cat file.txt – Display the contents of a file.
- rm file.txt – Delete a file.

Key Takeaway

Git gives me full control over my project's history. I decide what to track, stage, and commit, making it easier to manage changes, collaborate, and safely return to previous versions whenever needed.
------------------------------------------

📅 Day 3 – Git

Today, I deepened my understanding of Git branching, merging, and Git installation.
What I Learned
Reviewed Git fundamentals, including repositories, staging, and commits.
Learned how branches allow developers to work independently without affecting the main project.
Practiced creating, switching, and deleting branches.
Learned how git merge integrates changes from one branch into another.
Understood what a Merge Conflict is, why it happens, and how to resolve it manually.
Learned additional Git commands:
git diff
git restore
git reset
git stash
.gitignore
Studied the Git installation process, including the purpose of the main installation options and which settings are recommended for development.
Key Takeaway
Today I learned that branches make collaboration safer and more organized. I also understood that merge conflicts must be resolved by the developer, and I became familiar with the recommended Git installation settings for a professional development environment.


# Today's Practical Git Practice
## Today's Git Practical Practice
Today, I practiced Git commands and concepts through hands-on exercises, including repository creation, commits, branches, and merging.

----my git bash
JEI@DESKTOP-79F36FF MINGW64 ~/Desktop
$ mkdir new

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop
$ cd new

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new
$ git init
Initialized empty Git repository in C:/Users/RAMONA/Desktop/new/.git/

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git --version
git version 2.55.0.windows.3

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ echo "git" > newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        newfile.txt

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git add newfile.txt
warning: in the working copy of 'newfile.txt', LF will be replaced by CRLF the next time Git touches it

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   newfile.txt


JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   newfile.txt


JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git commit -m newfile.txt
[master (root-commit) 4d410b9] newfile.txt
 1 file changed, 1 insertion(+)
 create mode 100644 newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master
nothing to commit, working tree clean

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git log
commit 4d410b90d3249f04a0e6e2e11502641aea486261 (HEAD -> master)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:10:23 2026 +0330

    newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ echo "git" > welcom!

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        welcom!

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        welcom!

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git add welcome!
fatal: pathspec 'welcome!' did not match any files

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ ls
 newfile.txt  'welcom!'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ rm welcome!
rm: cannot remove 'welcome!': No such file or directory

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ rm newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    newfile.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        welcom!

no changes added to commit (use "git add" and/or "git commit -a")

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ ls
'welcom!'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git reset --hard HEAD~1
fatal: ambiguous argument 'HEAD~1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ gt log --online
bash: gt: command not found

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git log --online
fatal: unrecognized argument: --online

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git log --onelog
fatal: unrecognized argument: --onelog

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ git log --oneline
4d410b9 (HEAD -> master) newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new (master)
$ rm -rf .git

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new
$ git status
fatal: not a git repository (or any of the parent directories): .git

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new
$ mkdir new

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new
$ cd new

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new
$ git init
Initialized empty Git repository in C:/Users/RAMONA/Desktop/new/new/.git/

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ echo "git" > file.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file.txt

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git add file.txt
warning: in the working copy of 'file.txt', LF will be replaced by CRLF the next time Git touches it

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git commit -m "made a new file."
[master (root-commit) ebb7c2e] made a new file.
 1 file changed, 1 insertion(+)
 create mode 100644 file.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ echo "git" >> file1.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file1.txt

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git add file1.txt
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git commit -m "made an another file."
[master 7ee95cc] made an another file.
 1 file changed, 1 insertion(+)
 create mode 100644 file1.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git status
On branch master
nothing to commit, working tree clean

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git log
commit 7ee95cc3e6f3b0d1acd1e182d50028ca0b8b15cd (HEAD -> master)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:52:54 2026 +0330

    made an another file.

commit ebb7c2e2b2ae8f69ac8b0d18b0fd45431a8acbc7
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:51:30 2026 +0330

    made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch
* master

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch new-b

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git status
On branch master
nothing to commit, working tree clean

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch
* master
  new-b

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch checkout

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch
  checkout
* master
  new-b

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout -b new-b
fatal: a branch named 'new-b' already exists

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout new-b
Switched to branch 'new-b'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git branch
  checkout
  master
* new-b

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git checkoutmaster
git: 'checkoutmaster' is not a git command. See 'git --help'.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git checkout master
Switched to branch 'master'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch
  checkout
* master
  new-b

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch -d new-b
Deleted branch new-b (was 7ee95cc).

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch
  checkout
* master

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git diff

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git diff file2.txt
fatal: ambiguous argument 'file2.txt': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git branch checkout -b new-b
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --[no-]verbose    show hash and subject, give twice for upstream branch
    -q, --[no-]quiet      suppress informational messages
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --[no-]set-upstream-to <upstream>
                          change the upstream info
    --[no-]unset-upstream unset the upstream info
    --[no-]color[=<when>] use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --[no-]abbrev[=<n>]   use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --[no-]delete     delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --[no-]move       move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    --[no-]omit-empty     do not output a newline after empty formatted refs
    -c, --[no-]copy       copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --[no-]list       list branch names
    --[no-]show-current   show current branch name
    --[no-]create-reflog  create the branch's reflog
    --[no-]edit-description
                          edit the description for the branch
    -f, --[no-]force      force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --[no-]column[=<style>]
                          list branches in columns
    --[no-]sort <key>     field name to sort on
    --[no-]points-at <object>
                          print only branches of the object
    -i, --[no-]ignore-case
                          sorting and filtering are case insensitive
    --[no-]recurse-submodules
                          recurse through submodules
    --[no-]format <format>
                          format to use for the output


JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout -b new-b
Switched to a new branch 'new-b'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ echo "git" > newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git status
On branch new-b
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        newfile.txt

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git add newfile.txt
warning: in the working copy of 'newfile.txt', LF will be replaced by CRLF the next time Git touches it

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git commit -m "made a new file in a new branch"
[new-b 5603074] made a new file in a new branch
 1 file changed, 1 insertion(+)
 create mode 100644 newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git log
commit 5603074a738fdb73b24b4d3c65d6a742e20e722a (HEAD -> new-b)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:03:13 2026 +0330

    made a new file in a new branch

commit 7ee95cc3e6f3b0d1acd1e182d50028ca0b8b15cd (master, checkout)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:52:54 2026 +0330

    made an another file.

commit ebb7c2e2b2ae8f69ac8b0d18b0fd45431a8acbc7
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:51:30 2026 +0330

    made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git status
On branch new-b
nothing to commit, working tree clean

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git checkout master
Switched to branch 'master'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git statsus
git: 'statsus' is not a git command. See 'git --help'.

The most similar command is
        status

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout new-b
Switched to branch 'new-b'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ echo "hello" >> newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git status
On branch new-b
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   newfile.txt

no changes added to commit (use "git add" and/or "git commit -a")

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git add newfile.txt
warning: in the working copy of 'newfile.txt', LF will be replaced by CRLF the next time Git touches it

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git commit -m "newfile.txt changed"
[new-b fbb2a40] newfile.txt changed
 1 file changed, 1 insertion(+)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git status
On branch new-b
nothing to commit, working tree clean

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ ls
file.txt  file1.txt  newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git log
commit fbb2a40d1ad3b638cc7b5610ecda8d2491532ac0 (HEAD -> new-b)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:14:34 2026 +0330

    newfile.txt changed

commit 5603074a738fdb73b24b4d3c65d6a742e20e722a
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:03:13 2026 +0330

    made a new file in a new branch

commit 7ee95cc3e6f3b0d1acd1e182d50028ca0b8b15cd (master, checkout)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:52:54 2026 +0330

    made an another file.

commit ebb7c2e2b2ae8f69ac8b0d18b0fd45431a8acbc7
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:51:30 2026 +0330

    made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git diff

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git log --onelog
fatal: unrecognized argument: --onelog

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git log --oneline
fbb2a40 (HEAD -> new-b) newfile.txt changed
5603074 made a new file in a new branch
7ee95cc (master, checkout) made an another file.
ebb7c2e made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git checkout master
Switched to branch 'master'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git log --oneline
7ee95cc (HEAD -> master, checkout) made an another file.
ebb7c2e made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout new-b
Switched to branch 'new-b'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git merge main
merge: main - not something we can merge

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git merge master
Already up to date.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (new-b)
$ git checkout master
Switched to branch 'master'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git log --oneline
7ee95cc (HEAD -> master, checkout) made an another file.
ebb7c2e made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git log
commit 7ee95cc3e6f3b0d1acd1e182d50028ca0b8b15cd (HEAD -> master, checkout)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:52:54 2026 +0330

    made an another file.

commit ebb7c2e2b2ae8f69ac8b0d18b0fd45431a8acbc7
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:51:30 2026 +0330

    made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git merge new-b
Updating 7ee95cc..fbb2a40
Fast-forward
 newfile.txt | 2 ++
 1 file changed, 2 insertions(+)
 create mode 100644 newfile.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git log --oneline
fbb2a40 (HEAD -> master, new-b) newfile.txt changed
5603074 made a new file in a new branch
7ee95cc (checkout) made an another file.
ebb7c2e made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ echo "git" > story.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        story.txt

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git add story.txt
warning: in the working copy of 'story.txt', LF will be replaced by CRLF the next time Git touches it

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git commit -m "new file added"
[master 3741243] new file added
 1 file changed, 1 insertion(+)
 create mode 100644 story.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git status
On branch master
nothing to commit, working tree clean

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ echo "welcome" >> story.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git log
commit 3741243c6fdca77010422607b34ac0ae704c4608 (HEAD -> master)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:21:59 2026 +0330

    new file added

commit fbb2a40d1ad3b638cc7b5610ecda8d2491532ac0 (new-b)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:14:34 2026 +0330

    newfile.txt changed

commit 5603074a738fdb73b24b4d3c65d6a742e20e722a
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:03:13 2026 +0330

    made a new file in a new branch

commit 7ee95cc3e6f3b0d1acd1e182d50028ca0b8b15cd (checkout)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:52:54 2026 +0330

    made an another file.

commit ebb7c2e2b2ae8f69ac8b0d18b0fd45431a8acbc7
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:51:30 2026 +0330

    made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout -b newbb
Switched to a new branch 'newbb'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ echo "git" > story.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ echo "hello" >> story.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git checkout master
M       story.txt
Switched to branch 'master'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (master)
$ git checkout newbb
M       story.txt
Switched to branch 'newbb'

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ add git story.txt
bash: add: command not found

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git status
On branch newbb
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   story.txt

no changes added to commit (use "git add" and/or "git commit -a")

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git add story.txt
warning: in the working copy of 'story.txt', LF will be replaced by CRLF the next time Git touches it

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git commit -m "story.txt was made."
[newbb 3eb06f4] story.txt was made.
 1 file changed, 1 insertion(+)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ checkout master
bash: checkout: command not found

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git merge newbb
Already up to date.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git log
commit 3eb06f4db38a87529fcb2fb2dd2616a658534837 (HEAD -> newbb)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:25:59 2026 +0330

    story.txt was made.

commit 3741243c6fdca77010422607b34ac0ae704c4608 (master)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:21:59 2026 +0330

    new file added

commit fbb2a40d1ad3b638cc7b5610ecda8d2491532ac0 (new-b)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:14:34 2026 +0330

    newfile.txt changed

commit 5603074a738fdb73b24b4d3c65d6a742e20e722a
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 19:03:13 2026 +0330

    made a new file in a new branch

commit 7ee95cc3e6f3b0d1acd1e182d50028ca0b8b15cd (checkout)
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:52:54 2026 +0330

    made an another file.

commit ebb7c2e2b2ae8f69ac8b0d18b0fd45431a8acbc7
Author: z <miripourzeinab@gmail.com>
Date:   Sat Jul 18 18:51:30 2026 +0330

    made a new file.

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git chekout master
git: 'chekout' is not a git command. See 'git --help'.

The most similar command is
        checkout

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ echo "Hello" > con.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ add con.txt
bash: add: command not found

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git add con.txt
error: open("con.txt"): No such file or directory
error: unable to index file 'con.txt'
fatal: adding files failed

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ echo "git" > con.txt

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ status
bash: status: command not found

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git status
On branch newbb
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        con.txt

nothing added to commit but untracked files present (use "git add" to track)

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$ git add con.txt
error: open("con.txt"): No such file or directory
error: unable to index file 'con.txt'
fatal: adding files failed

JEI@DESKTOP-79F36FF MINGW64 ~/Desktop/new/new (newbb)
$

More updates coming soon... 🚀
