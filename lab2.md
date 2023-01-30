# Lab Report 2

## Part 1

Here's the screenshot of my code:

![屏幕截图 2023-01-29 184908](https://user-images.githubusercontent.com/122576524/215378830-6a332887-7be0-457f-b70b-61684be95d65.png)


After I opened the website in my terminal, I entered the first command in the web browser: ```/add-message?s=Hello```. The result is the following screenshot.

![4](https://user-images.githubusercontent.com/122576524/215379090-3a5e6a77-4077-407d-a893-9c2516fd9c39.png)

In the main method, a variable **port** is created, and I can create our own **port** by typing different number on the command line. I then call ```start(int port, URLHandler handler) which takes the port we define and ```new Handler()``` as the arguments.

In ```handleRequest(URI url)```, we have our own url which is ```http://localhost:4000/add-message?s=How``` as the argument. Since our path of the given url is not ```/``` only, so we directly jump to the else part. ```getPath()``` is called to find the path of the url we input. In this case, it's ```/add-message```. Then ```contains()``` is called to see whether ```/add-message``` is contained in the path of the specific url, which is true in this case. We create a variable **addParameters** which is a list of two strings. These two strings are are seperated by ```=``` in the query of our input url, and note that I find the query by using ```getQuery()```.
