# Git Merging

Git Commands for merging: 
- `git merge branchname` : Merging in Git creates a special commit that has two unique parents. A commit with two parents essentially means 
   "I want to include all the work from this parent over here and this one over here, and the set of all their parents."

<div align="center">
  
![image](https://user-images.githubusercontent.com/83855905/171159965-72ed05b7-2d0e-4978-a380-ca5dd3066693.png)
  
</div>

The `main` branch now points to a commit that has two parents. If you follow the arrows up the commit tree from `main`, you will hit every commit along the way to the root. 
This means that `main` contains all the work in the repository now.
