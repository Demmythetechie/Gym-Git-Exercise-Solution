BUNDLE 1 
#Exercise 1

C:\Users\Ejitade Isaac\Downloads\cmder
λ mkdir Gym-Git-Exercise-Solutions

C:\Users\Ejitade Isaac\Downloads\cmder
λ git init Gym-Git-Exercise-Solutions
Initialized empty Git repository in C:/Users/Ejitade Isaac/Downloads/cmder/Gym-Git-Exercise-Solutions/.g it/

C:\Users\Ejitade Isaac\Downloads\cmder
λ cd Gym-Git-Exercise-Solutions

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(master)
λ git branch -m master main

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ cat > README.md
BUNDLE 1
Exercise 1

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add -A
warning: LF will be replaced by CRLF in README.md.
The file will have its original line endings in your working directory

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git commit -m "Created a readme file"
[main (root-commit) ca18913] Created a readme file
1 file changed, 2 insertions(+)
create mode 100644 README.md

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCybrs7J8MVAxoBzkxJ7GWquNpoQ6A1TEJOHTeSeFduSpwFi4BMta8QFTMlfK/183Tx AeS/UNKyHkoOQ1n/WzUdJhZf7Di3Sf+ewkhiJc9umsCohwVYbpazK+pQgBBg5qHGfxoPqjEdyNWcyrECugfCbqtbvugs+f4PxmZG8iSD Nb0jKSjcBLh3Fyr9yoAwOrhOUe+9fkehRhzpZidqUDe7xr+HdOe2hiL1jerdZ9KpZg/mtoRIXRsdT/YBI+tS9Du1pEvkGTTdLz+IwhkE..............

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git remote add orgin git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git push git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 240 bytes | 80.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:Demmythetechie/Gym-Git-Exercise-Solution.git

[new branch] main -> main
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git branch dev

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git checkout dev
Switched to branch 'dev'

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(dev)
λ git branch test

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(dev)
λ git branch -d test
Deleted branch test (was ca18913).

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(dev)
λ git branch

dev
main


BUNDLE 1
#Exercise 2

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ cat > home.html
<!DOCTYPE html>
<html lang="en">
        <head>
                <title>Home</html>
        </head>
        <body>
                <div>
                        <p>This is the home page</p>
                </div>
        </body>
</html>

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add home.html
warning: LF will be replaced by CRLF in home.html.
The file will have its original line endings in your working directory

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git stash
Saved working directory and index state WIP on main: df0bae3 deleted

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ cat > about.html
<!DOCTYPE html>
<html lang="en">
        <head>
                <title>Home</html>
        </head>
        <body>
                <div>
                        <p>This is the about page</p>
                </div>
        </body>
</html>

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add about.html
warning: LF will be replaced by CRLF in about.html.
The file will have its original line endings in your working directory

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git stash
Saved working directory and index state WIP on main: df0bae3 deleted

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ cat > team.html
<!DOCTYPE html>
<html lang="en">
        <head>
                <title>Home</html>
        </head>
        <body>
                <div>
                        <p>This is the team page</p>
                </div>
        </body>
</html>

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add team.html
warning: LF will be replaced by CRLF in team.html.
The file will have its original line endings in your working directory

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git stash
Saved working directory and index state WIP on main: df0bae3 deleted

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add -A

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git stash list
stash@{0}: WIP on main: df0bae3 deleted
stash@{1}: WIP on main: df0bae3 deleted
stash@{2}: WIP on main: df0bae3 deleted

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ ls
README.md

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git stash pop stash@{1}
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (c62da0414bdbc6ddad3321d099d89e397ca3e321)

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add -A

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git commit -m "about.html file was unstashed"
[main 90cc27b] about.html file was unstashed
 1 file changed, 11 insertions(+)
 create mode 100644 about.html

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git stash pop --index 1
<stdin>:14: trailing whitespace.
                        <p>This is the home page</p>
warning: 1 line adds whitespace errors.
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped refs/stash@{1} (2eef36cd5ae77bf6666512c87c6d6cf3f195fc5d)

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add -A

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git commit -m "home.html file was unstashed"
[main 5585050] home.html file was unstashed
 1 file changed, 11 insertions(+)
 create mode 100644 home.html

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git push git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 638 bytes | 212.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
To github.com:Demmythetechie/Gym-Git-Exercise-Solution.git
   df0bae3..5585050  main -> main

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git stash pop --index 0
<stdin>:14: trailing whitespace.
                        <p>This is the team page</p>
warning: 1 line adds whitespace errors.
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (0110c5af826fc0d9e08f6534c0f4fde5040caa69)

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git reset --hard
HEAD is now at 5585050 home.html file was unstashed

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ ls
about.html  home.html  README.md



BUNDLE 2
#e[2Exercise 1
                  
BUNDLE 2
# Exercise 1

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git branch ft/bundle-2

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
M       README.md

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/bundle-2)
λ cat > services.html
<!DOCTYPE html>
<html lang="en">
        <head>
                <title>Home</html>
        </head>
        <body>
                <div>
                        <p>This is the service page</p>
                </div>
        </body>
</html>

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/bundle-2)
λ cat >> README.md

BUNDLE 2
#Exercise 1

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/bundle-2)
λ git add services.html README.md
warning: LF will be replaced by CRLF in README.md.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in services.html.
The file will have its original line endings in your working directory

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/bundle-2)
λ git commit -m "created a new branch and added some changes"
[ft/bundle-2 3563c8b] created a new branch and added some changes
 2 files changed, 15 insertions(+)
 create mode 100644 services.html

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/bundle-2)
λ git push git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 543 bytes | 271.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Demmythetechie/Gym-Git-Exercise-Solution/pull/new/ft/bundle-2
remote:
To github.com:Demmythetechie/Gym-Git-Exercise-Solution.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

BUNDLE 2
#Exercise 2 

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/bundle-2)
λ git checkout main                                                           
Switched to branch 'main'                                                     
                                                                              
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)       
λ git pull git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git        
remote: Enumerating objects: 8, done.                                         
remote: Counting objects: 100% (8/8), done.                                   
remote: Compressing objects: 100% (4/4), done.                                
remote: Total 4 (delta 1), reused 0 (delta 0), pack-reused 0                  
Unpacking objects: 100% (4/4), 1.44 KiB | 49.00 KiB/s, done.                  
From github.com:Demmythetechie/Gym-Git-Exercise-Solution                      
 * branch            HEAD       -> FETCH_HEAD                                 
Updating 01f65ad..ddac3ae                                                     
Fast-forward                                                                  
 README.md     |  5 +++++                                                     
 services.html | 11 +++++++++++                                               
 2 files changed, 16 insertions(+)                                            
 create mode 100644 services.html                                             
                                                                              
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)       
λ git branch ft/service-redesign                                              
                                                                              
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)       
λ git checkout ft/service-redesign                                            
Switched to branch 'ft/service-redesign'  

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ nl services.html
     1  <!DOCTYPE html>
     2  <html lang="en">
     3          <head>
     4                  <title>Home</html>
     5          </head>
     6          <body>
     7                  <div>
     8                          <p>This is the service page</p>
     9                  </div>
    10          </body>
    11  </html>

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ sed -i "8 a \\t\t\t<p>No services rendered for now<p>" services.html

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)               
λ git add services.html                                                                              
                                                                                                     
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)               
λ git commit -m "changes added to services.html in ft/service-redesign branch"                       
[ft/service-redesign c7c139f] changes added to services.html in ft/service-redesign branch           
 1 file changed, 2 insertions(+), 1 deletion(-)                                                      
                                                                                                     
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)               
λ git push git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git                               
Enumerating objects: 5, done.                                                                        
Counting objects: 100% (5/5), done.                                                                  
Delta compression using up to 4 threads                                                              
Compressing objects: 100% (3/3), done.                                                               
Writing objects: 100% (3/3), 353 bytes | 176.00 KiB/s, done.                                         
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0                                                 
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.                                
remote:                                                                                              
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:                       
remote:      https://github.com/Demmythetechie/Gym-Git-Exercise-Solution/pull/new/ft/service-redesign
remote:                                                                                              
To github.com:Demmythetechie/Gym-Git-Exercise-Solution.git                                           
 * [new branch]      ft/service-redesign -> ft/service-redesign

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ git checkout main
Switched to branch 'main'

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ sed -i "8 a \\t\t\t<p>we are back to the main branch for now</p>" services.html

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git add services.html                                                
                                                                       
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git commit -m "changes added to services.html in main branch"        
[main fac44e9] changes added to services.html in main branch           
 1 file changed, 3 insertions(+), 2 deletions(-)                       
                                                                       
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git push git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git 
Enumerating objects: 5, done.                                          
Counting objects: 100% (5/5), done.                                    
Delta compression using up to 4 threads                                
Compressing objects: 100% (3/3), done.                                 
Writing objects: 100% (3/3), 356 bytes | 178.00 KiB/s, done.           
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0                   
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.  
To github.com:Demmythetechie/Gym-Git-Exercise-Solution.git             
   ddac3ae..fac44e9  main -> main                                      
                                                                       
C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(main)
λ git checkout ft/service-redesign                                     
Switched to branch 'ft/service-redesign'                               

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ cat services.html
<!DOCTYPE html>
<html lang="en">
        <head>
                <title>Home</html>
        </head>
        <body>
                <div>
                        <p>This is the service page</p>
<<<<<<< HEAD
                        <p>No services rendered for now<p>
                </div>
=======
                        <p>we are back to the main branch for now</p>
                </div>
>>>>>>> main
        </body>
</html>

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ git add -A

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ git commit -m "resolved conflicts about to merge"
[ft/service-redesign 3ca8dae] resolved conflicts about to merge

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ git merge main
Already up to date.

C:\Users\Ejitade Isaac\Downloads\cmder\Gym-Git-Exercise-Solutions(ft/service-redesign)
λ git push git@github.com:Demmythetechie/Gym-Git-Exercise-Solution.git
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 388 bytes | 64.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:Demmythetechie/Gym-Git-Exercise-Solution.git
   c7c139f..3ca8dae  ft/service-redesign -> ft/service-redesign
