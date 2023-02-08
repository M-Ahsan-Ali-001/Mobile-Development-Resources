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
grep  Sam name.txt  //check for all the name sma in name.txt file
grep -i Sam name.txt //ignore case
~~~
