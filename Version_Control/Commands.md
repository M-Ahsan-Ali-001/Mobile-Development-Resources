# Making a bash file in linux  
~~~
#!/bin/bash
echo "Test print";

// './ file-name.sh' to run bash file
~~~
# Pipes
~~~
cat file | wc -w //counts total number of words
~~~

# Redirection
~~~
//standard input(stdin (0))
//standard output(stdout (1))
//standard error (stderr (2))

cat > input.txt //taking input and savinf that input to input.txt
cat < input.txt //displays text from entered from keyborad

2>//stores errors
2>&1 // stores both std out and error
~~~
# Grep 
~~~
grep  Sam name.txt  //check for all the name sma in name.txt file.
grep -i Sam name.txt //ignore case
~~~
# Git Clone 
~~~
// dir is uswedin cmd to list the files and directories

git version // print the version of git 
git clone https:"URL" // put URL of repo you want to clone.
~~~
# Git Status
~~~
git status // return the branch we are on and all the commits and changes.
~~~

# Git add
~~~
git add 'file-name' // git commandthat marks a file to be included as part of code commit.
~~~

# Git restore
~~~
git restore --stage test.txt // to remove added file from stage area.
~~~

# git commit 
~~~
git commit -m  "adding a new file for testing" //(-m means message)
~~~
# Git checkout 
~~~
git checkout -B feature/lesson // used to create a new branch and switch to that new branch 
git checkout main //used to switch to a repo.
~~~
# Git Branch
~~~
git branch  // tells about the current branch we are in
~~~
# Git push
~~~
git push -u origin feature/lesson // push to specific branch
~~~
# Git pull
~~~
git pull // get the latest changes
~~~

# Git init
~~~
git init  //used to create a a repository on local system
~~~

# Git remote
~~~
git remote -v // list connection we have with other repos.
git remote add origin 'URI' // used to add a connection to new repo
~~~
# git log 
~~~
git log --merge // prints the merge conflict
~~~
