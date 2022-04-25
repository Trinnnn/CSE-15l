# CSE 15L Spring 2022: Lab Report 2
## Bug, Symptom, and Failure-inducing Input

**Hello CSE 15L students!** Today I am going to depict the relationship between bug, symptom, and failure-inducing input. 

---

**1. Infinite Loop**

![image](8.png)

- The image above is the code change in order to fix the infinite loop when encountering this [failure-inducing input](https://github.com/Trinnnn/markdown-parser/blob/main/test-file2.md?plain=1) regarding a different formatted link.



- The 


---

**2. Image Link Inclusion**

![image](10.png)
![image](9.png)

 
- The first step is to open up the terminal and enter this command. Remember to replace zz with the letters in your course-specific account. 

```
$ ssh cs15lsp22zz@ieng6.ucsd.edu
```
- You will see the following message when you are connecting to a new server for the first time. Please answer yes for the message and type in your password. Then, you should be logged in.

```
$ ssh cs15lsp22zz@ieng6.ucsd.edu

The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.

RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.

Are you sure you want to continue connecting (yes/no/[fingerprint])?
```
- This is the result when you successfully connected to the remote computer / server! You can use it as a reference. 

---

**3. Index out of bound with Wrong Content Inclusion**

![image](7.png)

- Try to run the following commands on both your computer and the remote computer. I marked their function next to the commands.

```
cd ~ // change back to home directory

cd // change directory

pwd // output the full path name of your current directory

ls -lat // list all files including entries starting with ‘.’ in the long format along with the times when they were modified.

ls -a // list all the existing files including entries starting with ‘.’

cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/ 
//cp is a command that copy the file. But it will be permission denied since you are not allow to access code created by other people

cat /home/linux/ieng6/cs15lsp22/public/hello.txt 
// cat is a command that create or view a file. But it will be permission denied because you are not allow to create or view a file at the another person's directory.
```

- This is our sample result after running the command **ls -lat**.

Note: To logout of the remote server in the terminal, you can: 
1. Ctrl-D
1. Run the command exit
