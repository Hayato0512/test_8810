#Hi

#Hello my name is hayato

#new branch that I added after branching

#so this sentense is not affecting anything to the master branch




#hey I am in newBranch right now, so lets write something.
I guess this is pretty cool feature to be able to keep track of changes that I make to the code, but first I need to be used to use this system, to be able to use it with my actual projects, otherwise its gonna mess up both.
so this line is branching, a.k.a kind of experimenting sentenses so , it should not affect main branch until I am 100 % sure that this works and i want to add this change to the master branch. anyway, I will push this change , so first I type like "git add." this add all the file in the stage, like manaita. and if I commit, everything in this stage area will be pushed to the track.lets try by typing "git commit -m "add long sentense to the new branch"

#Ok, I think I want to merge this sentense, so lets try to marge again including this sentese to the master branch. dont screw it , you can do it.

























#hayatokoyama@HayatoKoyamaMAC Desktop % cd test_repo
hayatokoyama@HayatoKoyamaMAC test_repo % ls
hayatokoyama@HayatoKoyamaMAC test_repo % git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint: 	git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint: 	git branch -m <name>
Initialized empty Git repository in /Users/hayatokoyama/Desktop/test_repo/.git/
hayatokoyama@HayatoKoyamaMAC test_repo % ls
hayatokoyama@HayatoKoyamaMAC test_repo % git commit
On branch master

Initial commit

nothing to commit (create/copy files and use "git add" to track)
hayatokoyama@HayatoKoyamaMAC test_repo % cd ..
hayatokoyama@HayatoKoyamaMAC Desktop % ls
295ASS3SUBMIT						Screen Shot 2022-01-19 at 19.11.59 PM.png
ACADEMICJOURNAL						Screen Shot 2022-01-19 at 19.12.18 PM.png
C++Output						Screen Shot 2022-02-01 at 12.36.59 PM.png
C++TUT							Screen Shot 2022-02-08 at 16.59.43 PM.png
DIving							Screen Shot 2022-02-14 at 10.29.21 AM.png
MichelleBurnaby1.JPG					Screen Shot 2022-02-15 at 08.50.10 AM.png
MichelleBurnaby3.JPG					Screen Shot 2022-02-15 at 08.50.13 AM.png
SFU IMPORTANT						ToGoToCSIL
SFU_COURSES						USEFULPDFS
SHOTS							data-abstraction-and-problem-soving_6_th_edition.pdf
Screen Shot 2022-01-13 at 09.56.11 AM.png		michelle1.JPG
Screen Shot 2022-01-17 at 13.16.22 PM.png		michelle3.JPG
Screen Shot 2022-01-17 at 13.22.58 PM.png		sfuhome
Screen Shot 2022-01-17 at 13.24.06 PM.png		stack-LL
Screen Shot 2022-01-17 at 20.43.19 PM.png		test_repo
Screen Shot 2022-01-18 at 17.25.13 PM.png		なつき.JPG
Screen Shot 2022-01-18 at 20.20.06 PM.png
hayatokoyama@HayatoKoyamaMAC Desktop % git commit
fatal: not a git repository (or any of the parent directories): .git
hayatokoyama@HayatoKoyamaMAC Desktop % cd test_repo
hayatokoyama@HayatoKoyamaMAC test_repo % cls
zsh: command not found: cls
hayatokoyama@HayatoKoyamaMAC test_repo % git add readme.md
hayatokoyama@HayatoKoyamaMAC test_repo % ls
readme.md
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   readme.md

hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "added readme.md file"
[master (root-commit) b0e023b] added readme.md file
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch master
nothing to commit, working tree clean
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   readme.md

hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "added some new sentense"
[master 09790bf] added some new sentense
 1 file changed, 3 insertions(+), 1 deletion(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch master
nothing to commit, working tree clean
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout -b newBranch
Switched to a new branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "added some change after branching"
[newBranch 9f67a85] added some change after branching
 1 file changed, 4 insertions(+), 1 deletion(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
Switched to branch 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git add .                                        
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "came back to the master branch and made some sentense"
[master bb427be] came back to the master branch and made some sentense
 1 file changed, 3 insertions(+), 1 deletion(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch                                            
Switched to branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  master   
Switched to branch 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch
Switched to branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch
Already on 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git merge master
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
Automatic merge failed; fix conflicts and then commit the result.
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
readme.md: needs merge
error: you need to resolve your current index first
hayatokoyama@HayatoKoyamaMAC test_repo % git merge newBranch
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
hayatokoyama@HayatoKoyamaMAC test_repo % ls
readme.md
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch newBranch
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
	both modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
readme.md: needs merge
error: you need to resolve your current index first
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch
readme.md: needs merge
error: you need to resolve your current index first
hayatokoyama@HayatoKoyamaMAC test_repo % git add ..             
fatal: ..: '..' is outside repository at '/Users/hayatokoyama/Desktop/test_repo'
hayatokoyama@HayatoKoyamaMAC test_repo % git add .              
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "Some error happended so I am just commiting"
[newBranch 6c5d21d] Some error happended so I am just commiting
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch                                    
Already on 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  master   
error: Your local changes to the following files would be overwritten by checkout:
	readme.md
Please commit your changes or stash them before you switch branches.
Aborting
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch
M	readme.md
Already on 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  master   
error: Your local changes to the following files would be overwritten by checkout:
	readme.md
Please commit your changes or stash them before you switch branches.
Aborting
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch
M	readme.md
Already on 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "I did commit but it says to commit so i am "
On branch newBranch
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
hayatokoyama@HayatoKoyamaMAC test_repo % git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
	add
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "I think I did commit but I am messing this up i guess"
[newBranch b1aa7d7] I think I did commit but I am messing this up i guess
 1 file changed, 4 insertions(+), 1 deletion(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  master                                                 
Switched to branch 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout  newBranch
Switched to branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
Switched to branch 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "added some new sentense in master"
[master e414eef] added some new sentense in master
 1 file changed, 3 insertions(+), 1 deletion(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout newBranch
Switched to branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "added fucking long sentense to the newBranch, I am not sure to merge this into master, so lets just commit for now"
[newBranch b3b66a1] added fucking long sentense to the newBranch, I am not sure to merge this into master, so lets just commit for now
 1 file changed, 5 insertions(+), 1 deletion(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
Switched to branch 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout newBranch
Switched to branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch newBranch
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
error: Your local changes to the following files would be overwritten by checkout:
	readme.md
Please commit your changes or stash them before you switch branches.
Aborting
hayatokoyama@HayatoKoyamaMAC test_repo % git add . 
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "added sentense before i marge newbranch to the master
dquote> "
[newBranch 978a5bc] added sentense before i marge newbranch to the master
 1 file changed, 2 insertions(+)
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
Switched to branch 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git merge newBranch
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
Automatic merge failed; fix conflicts and then commit the result.
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "just merged newbranch to the master
dquote> "
[master 1a7e00b] just merged newbranch to the master
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout newBranch
Switched to branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
Switched to branch 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git remote add origin https://github.com/Hayato0512/test_8810.git
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout master
M	readme.md
Already on 'master'
hayatokoyama@HayatoKoyamaMAC test_repo % git push -u origin master
Username for 'https://github.com': Hayato0512
Password for 'https://Hayato0512@github.com': 
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
fatal: Authentication failed for 'https://github.com/Hayato0512/test_8810.git/'
hayatokoyama@HayatoKoyamaMAC test_repo % git remote add origin https://github.com/Hayato0512/test_8810.git
error: remote origin already exists.
hayatokoyama@HayatoKoyamaMAC test_repo % git push -u origin master                                        
Username for 'https://github.com': Hayato0512
Password for 'https://Hayato0512@github.com': 
Enumerating objects: 30, done.
Counting objects: 100% (30/30), done.
Delta compression using up to 4 threads
Compressing objects: 100% (18/18), done.
Writing objects: 100% (30/30), 3.01 KiB | 616.00 KiB/s, done.
Total 30 (delta 9), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (9/9), done.
To https://github.com/Hayato0512/test_8810.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
hayatokoyama@HayatoKoyamaMAC test_repo % git config --global user.name "Hayato"
hayatokoyama@HayatoKoyamaMAC test_repo % git pull origin master
hint: Pulling without specifying how to reconcile divergent branches is
hint: discouraged. You can squelch this message by running one of the following
hint: commands sometime before your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 791 bytes | 131.00 KiB/s, done.
From https://github.com/Hayato0512/test_8810
 * branch            master     -> FETCH_HEAD
   1a7e00b..8ed2203  master     -> origin/master
Updating 1a7e00b..8ed2203
error: Your local changes to the following files would be overwritten by merge:
	readme.md
Please commit your changes or stash them before you merge.
Aborting
hayatokoyama@HayatoKoyamaMAC test_repo % git status
On branch master
Your branch is behind 'origin/master' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m ""
Aborting commit due to empty commit message.
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "haha"
[master d502cbb] haha
 1 file changed, 5 insertions(+), 3 deletions(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git pull origin master
hint: Pulling without specifying how to reconcile divergent branches is
hint: discouraged. You can squelch this message by running one of the following
hint: commands sometime before your next pull:
hint: 
hint:   git config pull.rebase false  # merge (the default strategy)
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
From https://github.com/Hayato0512/test_8810
 * branch            master     -> FETCH_HEAD
Auto-merging readme.md
CONFLICT (content): Merge conflict in readme.md
Automatic merge failed; fix conflicts and then commit the result.
hayatokoyama@HayatoKoyamaMAC test_repo % git add .             
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "haha"  
[master d20455b] haha
hayatokoyama@HayatoKoyamaMAC test_repo % git add .
hayatokoyama@HayatoKoyamaMAC test_repo % git commit -m "change"
[master 25c8ca4] change
 1 file changed, 1 insertion(+), 1 deletion(-)
hayatokoyama@HayatoKoyamaMAC test_repo % git push
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 1005 bytes | 502.00 KiB/s, done.
Total 9 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To https://github.com/Hayato0512/test_8810.git
   8ed2203..25c8ca4  master -> master
hayatokoyama@HayatoKoyamaMAC test_repo % ls
readme.md
hayatokoyama@HayatoKoyamaMAC test_repo % ls
readme.md
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout new
error: pathspec 'new' did not match any file(s) known to git
hayatokoyama@HayatoKoyamaMAC test_repo % git checkout newBranch
Switched to branch 'newBranch'
hayatokoyama@HayatoKoyamaMAC test_repo % git push origin newBranch
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'newBranch' on GitHub by visiting:
remote:      https://github.com/Hayato0512/test_8810/pull/new/newBranch
remote: 
To https://github.com/Hayato0512/test_8810.git
 * [new branch]      newBranch -> newBranch
hayatokoyama@HayatoKoyamaMAC test_repo % 