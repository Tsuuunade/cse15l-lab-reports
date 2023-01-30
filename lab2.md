# Lab Report 2

## Part 1

Here's the screenshot of my code:


![屏幕截图 2023-01-29 184908](https://user-images.githubusercontent.com/122576524/215378830-6a332887-7be0-457f-b70b-61684be95d65.png)


After I opened the website in my terminal, I entered the first command in the web browser: ```/add-message?s=Hello```. The result is the following screenshot.

![4](https://user-images.githubusercontent.com/122576524/215379090-3a5e6a77-4077-407d-a893-9c2516fd9c39.png)

In the main method, a variable **port** is created, and I can create our own **port** by typing different number on the command line. I then call ```start(int port, URLHandler handler) which takes the port we define and ```new Handler()``` as the arguments.

In ```handleRequest(URI url)```, we have our own url which is ```http://localhost:4000/add-message?s=Hello``` as the argument. Since our path of the given url is not ```/``` only, so we directly jump to the else part. ```getPath()``` is called to find the path of the url we input. In this case, it's ```/add-message```. Then ```contains()``` is called to see whether ```/add-message``` is contained in the path of the specific url, which is true in this case. We create a variable **addParameters** which is a list of two strings. These two strings are are seperated by ```=``` in the query of our input url, and note that I find the query by calling ```getQuery()```.

After these steps, I start to consider the output. I create an instance variable **List** as typoe arraylist to store the strings. I call the method ```add(string)``` by passing the argument as ```addParameters[1]``` to add strings to the arraylist. I create a new variable **result** as a string object used for printing the output. Then I use ```equals()``` method to check whether the first part of the query is equal to ```s```. I use a for loop to iterate through **List** and add the strings in **List** to **result**. In this case, the for loop will only run one time and the value of the result is a string reference of ```Hello```.


![5](https://user-images.githubusercontent.com/122576524/215601156-eaf8e428-def9-47aa-ac79-05eb7585a8ab.png)


Through the second screenshot, you can see that I change the argument from ```http://localhost:4000/add-message?s=How``` to ```http://localhost:4000/add-message?s=How are you```. Everything looks similar, but now the instance variable **List** stores two strings because the ```add(string)``` method is called and the respective argument is ```How are you``` this time. Thus, when iterating through the for loop, the line inside runs 2 times and add ```Hello``` and ```How are you``` to **result**. And by using the string notation ```/n```, the output starts the second string in a new line.

## Part 2

```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
        arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```

This piece of code is a buggy code. I'm gonna use it to demonstrate a failure-inducing input and a nonfailure-inducing input.

* **failure-inducing input**
  ```
  int[] input1 = {2, 3, 4};
  assertArrayEquals(new int[]{4, 3, 2}, ArrayExamples.reversed(input1));
  ```
  
* **nonfailure-inducing input**
  ```
  int[] input1 = { };
  assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  ```  

This is what happens when I test the code with JUnit. Note that the test fails when we input the failure-inducing input.


![8](https://user-images.githubusercontent.com/122576524/215605790-3872cd36-11a4-48f8-9c09-44d03c00f7cb.png)


After trying some test cases, I find that only the empty list can pass the test, which means the code itself has significant mistake. Here is the bug:
```
arr[i] = newArray[arr.length - i - 1];
...
return arr;
```

Since I am assigning the values in newArray, which is all 0 by default, to arr, the first element of arr will become 0. This is not what I expected. Also remember that I'm returning a new array, which means I need to ```return newArray``` instead of ```arr```. The following is the fixed code:
```
newArray[i] = arr[arr.length - i - 1];
...
return newArray;
```

## Part 3

I don't know how to start a webpage by java, and I'm shocked when I realize that I can modify the output on the webpage by just modifying the input url. Furthermore, I know how to use JUnit to test my code. I struggled a lot in cse11 when testing my code. With the help of JUnit right now, I can design my own testcases instead of submitting to gradescope over and over again.
