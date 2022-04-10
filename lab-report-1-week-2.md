# TUTORIAL FOR INCOMING 15L STUDENTS 
---
## 1. Installing VScode 
Download VScode here:
[VScode](https://code.visualstudio.com/download)
Once you've downloaded VScode, it should look like this: 
![Image](vscode.png)
---

## 2. Install OpenSSH 
If you have Windows, install a program called OpenSSH
---

## 3. Course-specific account for CSE15L 
You can look up your course-specific account here:
[CSE 15L ACC](https://sdacs.ucsd.edu/~icc/index.php)
---

## 4. Connecting to remote computers in VScode
1. Open the terminal in VScode by doing (Ctrl + `)
2. Type in this command: $ ssh cs15lsp22zzz@ieng6.ucsd.edu 
Keep in mind to replace the zzz with your personal coure-specific account you found in step 3
3. If it is your first time connecting to this server, you willl get a message asking "Are you sure you want to continue connecting (yes/no/[fingerprint])?
4. Type yes and give your password 
5. It should look somewhat like this: 
![Image](step4.png)
Your terminal is now connnected to a computer in the CSE basement. 

---

## 5. Practice some commands!! 
try:
1. cs 
2. ls -lat
3. ls -a 
4. etc... 

---

## 6. Moving files over SSH with scp 
1. Create a file on VScode called WhereAmI.java and put the following inside:
class WhereAmI {
public static void main(String[] args) {
System.out.println(System.getProperty("os.name"));
System.out.println(System.getProperty("user.name"));
System.out.println(System.getProperty("user.home"));
System.out.println(System.getProperty("user.dir"));
}
}

2. Run this inside the terminal:
scp WhereAmI.java cs15lsp22zzz@ieng6.ucsd.edu:~/
Keep in mind to replace the zzz with your course-specific account 

3. It will prompt you to enter a password, so do so
4. It should look somewhat like this: 
![Image](scp.png)



