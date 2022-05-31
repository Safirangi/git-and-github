# Git Rebase

Rebasing is a process to reapply commits on top of another base trip. It is used to apply a sequence of commits from distinct branches into a final commit. 
It is an alternative of git merge command. It is a linear process of merging.

In other words, Rebasing essentially takes a set of commits, "copies" them, and plops them down somewhere else.

<div align="center">
  
![image](https://user-images.githubusercontent.com/83855905/171162374-993e5b6c-ccee-4450-9e09-5945959a39c5.png)
  
  Here we have two branches yet again, note that the bugFix branch is currently selected (note the asterisk). We would like to move our work from bugFix directly onto the work from main. 
  That way it would look like these two features were developed sequentially, when in reality they were developed in parallel.
  
  ![image](https://user-images.githubusercontent.com/83855905/171162728-e2520610-67ba-4354-a726-10a780ef3f60.png)

   Now the work from our bugFix branch is right on top of main and we have a nice linear sequence of commits. Note that the commit C3 still exists somewhere 
   (it has a faded appearance in the tree), and C3' is the "copy" that we rebased onto main. The only problem is that main hasn't been updated either.
  
  ![image](https://user-images.githubusercontent.com/83855905/171163124-a9c88e71-a755-46a0-81d7-55003eed2b98.png)
  
  Now we are checked out on the main branch. Let's go ahead and rebase onto bugFix.
  
  ![image](https://user-images.githubusercontent.com/83855905/171163250-a037d73f-6f85-4bb3-b956-ffbfb08b20ad.png)
  
  Since main was an ancestor of bugFix, git simply moved the main branch reference forward in history.

</div>

### Git commands for Rebasing: 
- `git rebase main` 
