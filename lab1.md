# Week 1 Lab Report
## Step 1: Installing VScode


Here's the link for the instructions about downloading VScode: [[How to Downloade VScode]](https://code.visualstudio.com/). Since I've already had my VScode downloaded on my laptop, I skipped this step. However, for those who don't have VScode yet, remember to restrictly follow the steps and check whether you can open VScode. When it's installed on your laptop, you should be able to see an interface like the following picture.


![屏幕截图 2023-01-15 165949](https://user-images.githubusercontent.com/122576524/212577536-590cde53-70db-43ed-b6b0-5f1e519352e7.png)


## Step 2: Remotely Connecting


There are a bunch of things you need to get your remote connection. Steps include:

* **Set up your CSE15L Account**

  Since the CSE department has already created an account for you, you can directly go to [[Account Setup]](https://sdacs.ucsd.edu/~icc/index.php) to check your account.
  
  
  If you want to reset your password, which is what I did, strictly follow the steps here: [[How to Reset Your Password]](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit).
  
* **Installing git for Windows**

  **Remark:If your are using a Mac, just ignore this step. This step is only for the one who's using Windows.**


  You need to first install git here: [[How to install Git]](https://gitforwindows.org/). Onced you've installed, you have to link the git to your VScode. You need to follow these steps:
  
  * At the top of your interface for VScode, you can find ```Terminal```.
  * Click it and then click ```New Terminal```.
  * Use ```Control```+```Shift```+```P``` to open the command palette.
  * Search for ```Select Default Profile```.
  * Click on ```Git Bash```.
  * Click the ```+``` in your terminal.
  
  
  After you've done, you're all set and the page should be like this (**pay attention to the red circle!**)
  
  
  ![03da39823663532cb6bff752ba56825](https://user-images.githubusercontent.com/122576524/212581363-9ac83820-d228-42bf-8856-314a6971e58e.jpg)


* **log in to your account on your VScode**

  Open a new terminal in you VScode, type ```ssh cs15lwi23aus@ieng6.ucsd.edu``` into the terminal, and remember to replace ```aus``` with your own course-specific account. If you don't know your account yet, you should go beck and check the instructions under **Set up your CSE15L Account**.


  You should now enter your account password into the terminal. It's normal that you cannot see anything you're typing. If you're not confident in your typing, you can type your password somewhere else and copy paste it into the terminal.
  
  
  If it's the first time you log in your server, there will be a message saying "Are you sure you want to connect?". Just type ```yes``` in the terminal. Then, you should see something like this
  
  
  ![屏幕截图 2023-01-15 175644](https://user-images.githubusercontent.com/122576524/212582635-a1638374-c5a5-48c8-9bb1-66a870262c1e.png)


## Step 3: Trying Some Commands

Now, you can try some commands on your terminal. Here are some commands that I tried on my own computer:

* ```cat /home/linux/ieng6/cs15lwi23/public/hello.txt``` reads the file in the given directory, which is ```/home/linux/ieng6/cs15lwi23/public/hello.txt``` and write them to the standard output.


  ![1](https://user-images.githubusercontent.com/122576524/212754211-1d2f0ab0-3aee-42f4-aa01-4fa5064f35c4.png)


* ```ls <directory>``` where ```<directory>``` is replaced by ```/home/linux/ieng6/cs15lwi23/cs15lwi23aus``` and ```aus``` should be replaced my your own course-specific account. This command lists the content in the given ```<directory>```.


  ![2](https://user-images.githubusercontent.com/122576524/212754234-38e199ea-1a8e-4240-8956-bf0905d8769a.png)


* ```ls -lat``` displays information about the user, size of the file, date of modification, and time of modification.


  ![3](https://user-images.githubusercontent.com/122576524/212754256-a4f5f1cc-a81d-453b-84b9-66ce26aefada.png)


* ```ls -a``` displays hidden files and files starting with “.”.


  ![4](https://user-images.githubusercontent.com/122576524/212754283-f0660e4a-b330-4534-86f1-a53d311cc0d5.png)


I didn't run into errors for those command. Just follow the guide strictly and I believe you can also do it. You could also try more commands such as ```pwd```, ```mkdir``` etc. You could try them both on your own computer and the remote computer. I didn't do this in my lab but I did try them later on. Those commands are pretty cool.


Finally, you could log out your account by typing ```exit``` in your terminal.
