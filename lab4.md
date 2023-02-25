**Log into ieng6**

![image](https://user-images.githubusercontent.com/122576524/221055270-688454c6-95b7-4eb0-a5d6-877968b48605.png)

key pressed: ```<up><enter>```

The ```ssh cs15lwi23aus@ieng6.ucsd.edu``` command is 1 up in the search history. Since I don't have to type my password for it, it logs into my account automatically


**Clone your fork of the repository from your Github account**

![image](https://user-images.githubusercontent.com/122576524/221055922-2c6e647e-83bc-4fc0-b06c-0da5a4b28952.png)

key pressed: ```git clone <ctrl-v><enter>```

Since ```git clone``` is a short command, I just type it out. I've already copied the url for the repository, so I only need to type ```<ctrl-v>``` to paste it.


**Run the tests, demonstrating that they fail**

![image](https://user-images.githubusercontent.com/122576524/221056532-d6472c15-b80f-473a-81cb-9767357950d1.png)

key pressed: ```cd l<Tab><enter>```, ```<up><up><up><up><up><up><up><up><up><enter>```, ```<up><up><up><up><up><up><up><up><up><enter>```

First I cd into the lab7 directory. I use ```<Tab>``` after I type ```l``` and it auto-fills the rest for me. The command ```javac -cp .:lib/hamcrest-core 1.3.jar:lib/junit-4.13.2.jar *.java``` is 9 up in the search history, so I use ```<up>``` to access it. I do the same thing to find the command ```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests```


**Edit the code file to fix the failing test**

* ```nano L<tab>.j<tab>```

![image](https://user-images.githubusercontent.com/122576524/221060519-598d21cd-94e3-4e87-9cc0-8512f3c9f4e6.png)

```<tab>``` helps me to autofill the rest of information.
 
* ```<ctrl-w> return result <enter>```

![image](https://user-images.githubusercontent.com/122576524/221061053-4bf97df4-00e4-41e6-8247-3e56c549d641.png)

```<ctrl-w>``` helps me to search the string "return result" inside ListExamples.java. So my mouse can get closer to where I want to change.

* ```<up><up><left><left><left><left><left><left><left><left>```

![image](https://user-images.githubusercontent.com/122576524/221061431-f373da98-3b67-48a4-918c-60c9ebb5b031.png)

I change the place of my mouse to a new position.

* ```<backspace>2```

![image](https://user-images.githubusercontent.com/122576524/221061551-f4d0960e-a05e-44ec-be7e-027244feca59.png)

I change ```index1``` to ```index2```.

* ```<ctrl-o><enter><ctrl-x>```

![image](https://user-images.githubusercontent.com/122576524/221061773-0910fec1-ccdd-48f4-beb5-1a1d000b54eb.png)

By pressing ```<ctrl-o>```, I save the file. I use ```<ctrl-x>``` to exit nano.


**Commit and push the resulting change to your Github account**

