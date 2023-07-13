# self-practice
* git does not stores twice it saves only once ( in two folder same data or content it have one commit id)
* even though two repos also hashing will stores git in same content hashing  have same .
* all files are stored in .git/.objects

* name of git is also global information tracker
* 
### hash calculation
 (encrypt some data ,only case the unic number is  equel hash data will be same when code will be same)

![hema](./Images/1.git.png)

### what is branch?

* branch is a reference object which points to same commit id , branch points new commit id 


### tree reprasent folder/directory
### blob reprasents file
![hema](./Images/2.git.png)


### git reset hard && soft

#### rebase

* never rebase public branch with any other branch
            git rebase --continue
            git rebase --abort 
            git rebase --fixed
            git rebase --skip (prefered low)
            git rebase 
    * merge changes history of the parent

### cherry pick
 * cherry picking is required one or sequence of commits from one branch to another 
 * 
            git cherry-pick <commit-id>
            git cherry-pick --continue

    <https://www.atlassian.com/git/tutorials/cherry-pick#:~:text=Cherry%20picking%20is%20the%20act,to%20where%20it%20should%20belong.>

    <https://www.atlassian.com/git/tutorials/using-branches/git-merge#:~:text=Fast%20Forward%20Merge&text=3%2Dway%20merges%20use%20a,tips%20and%20their%20common%20ancestor.> 

* git diff <commit-id-a> .. <commit-id-b>(what is storing in repository and what is changing in your directory)

* git diff <commit-id-a>^..<commit-id-b>(this includes the second commit)

            git show HEAD~1

* HEAD~5( move one commit back)
* HEAD^1
            git rebase -i HEAD~2 (-i  = optional)

*  each commitis a sealed box . then we change the history of commit
   by using  "interactive rebase"
            git rebase --continue
            git log --oneline

   p=pick
   r= reword
   e=edit
   s=squash
   f=fixup
            git commit --amend (you can change your latest commit "only change what head looking")

# exersice 
* find a way using cli to show 
    all the commits done on a file
    find all the commits b/w some dates (ex: sept 11-2022 to jan-6-2022 )
    show the files in a specific commit 




