# Week 1 Lab Report
## Step 1: Installing VScode


Here's the link for the instructions about downloading VScode: https://code.visualstudio.com/. Since I've already had my VScode downloaded on my laptop, I skipped this step. However, for those who don't have VScode yet, remember to restrictly follow the steps and check whether you can open VScode. When it's installed on your laptop, you should be able to see an interface like the following picture.


![屏幕截图 2023-01-15 165949](https://user-images.githubusercontent.com/122576524/212577536-590cde53-70db-43ed-b6b0-5f1e519352e7.png)


## Step 2: Remotely Connecting


There are a bunch of things you need to get your remote connection. Steps include:

* **Set up your CSE15L Account**

  Since the CSE department has already created an account for you, you can directly go to https://sdacs.ucsd.edu/~icc/index.php to check your account.
  
  
  If you want to reset your password, which is what I did, strictly follow the steps here: [[How to Reset Your Password]](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit)
  
* **Installing git for Windows**

  **Remark:If your are using a Mac, just ignore this step. This step is only for the one who's using Windows.**


  You need to first install git here: https://gitforwindows.org/. Onced you've installed, you have to link the git to your VScode. How you can do this could be found   on the following website [[Using bash for Windows]](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994). After you've done, make sure you could see bash here:
  
  
  ![03da39823663532cb6bff752ba56825](https://user-images.githubusercontent.com/122576524/212581363-9ac83820-d228-42bf-8856-314a6971e58e.jpg)


* log in to your account on your VScode

  Open a new terminal in you VScode, type ```ssh cs15lwi23aus@ieng6.ucsd.edu``` into the terminal, and remember to replace ```aus``` with your own course-specific account. If you don't know your account yet, you should go beck and check the instructions under **Set up your CSE15L Account**.


  You should now enter your account password into the terminal. It's normal that you cannot see anything you're typing. If you're not confident in your typing, you can type your password somewhere else and copy paste it into the terminal.
  
  
  If it's the first time you log in your server, there will be a message saying "Are you sure you want to connect?". Just type ```yes``` in the terminal. Then, you should see something like this
  
  
  ![屏幕截图 2023-01-15 175644](https://user-images.githubusercontent.com/122576524/212582635-a1638374-c5a5-48c8-9bb1-66a870262c1e.png)


## Step 3: Trying Some Commands
