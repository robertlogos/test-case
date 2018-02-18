## Test case for issue with git/github and case-insensitive filesystem

Cloning this repository to a case-insensitive filesystem (e.g. default MAC APFS configuration) replaces automatically `myFile.txt` with `myfile.txt` 
    
```bash
$ ls
README.md  myfile.txt

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.

Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git checkout -- <file>..." to discard changes in working directory)

    modified:   myFile.txt

no changes added to commit (use "git add" and/or "git commit -a")
```

