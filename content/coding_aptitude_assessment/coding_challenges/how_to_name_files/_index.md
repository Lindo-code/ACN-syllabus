---
_db_id: 755
content_type: topic
ready: true
title: IMPORTANT!! Naming your files and functions
---

This is **REALLY IMPORTANT!**

**Good coders pay close attention to detail and read specifications properly.**


We use a bot to mark these projects. The bot requires that your code is laid out in a very specific way. If your code is not laid out in this way then the bot will mark the code as incorrect.

But don't panic :) The code layout is very straight-forward.

## Python

If you are doing the coding challenge in Python then you should make a separate file for each task. The files should be named according to the following pattern:

Task 1 should be in a file named `task1.py`, task 2 should be in a file named `task2.py`, etc.

The files should be in the root directory of your repo. You should not have any extra directories. In other words, all your task files should be in the same directory as the README.md file that was automatically created in your repo.

Each task will require that you write a single function. Please name the functions according to the same convention as the files.

Task 1's function should be named `task1` (so you will start off by writing `def task1(`), and task 2's function should be named `task2`, etc.

## Javascript

If you are doing the coding challenges in Javascript then you should make a separate file for each task. The files should be named according to the following pattern:

Task 1 should be in a file named `task1.js`, task 2 should be in a file named `task2.js`

The files should be in the root directory of your repo. You should not have any extra directories. In other words, all your task files should be in the same directory as the README.md file that was automatically created in your repo.

Each task will require that you write a single function. Please name the functions according to the same convention as the files.

Task 1's function should be named `task1`  (so you will start off by writing `function task1(`), and task 2's function should be named `task2`, etc.



### Exports - CRITICAL INFO FOR JAVASCRIPT LEARNERS

> This is only necessary for JavaScript developers.

This is also very important. If you don't do this then the bot wont be able to access your functions!

At the end of every one of your task files you need to `export` the function. You do this by including an export statement like this.

```
module.exports = { YOUR_FUNCTION_NAME };
```

So for task 1, you will create a file named task1.js. Inside that file you will have the following:

```
function task1(){
    // YOUR FUNCTION CODE
}

module.exports = { task1 };

```
## Java 

If you are doing the coding challenges in Java then you should make a separate file per task. Each file must contain one class.

For task 1 the file should be names `Task1.java`. Inside that file, you should have a class named `Task1`. Inside that class you should have a function called `task1`.

If you want to test out your code then feel free to make a `main` function as well. For example, your final Task1.java file could look something like this:

```
public class Task1 {
    public static void main(String[] args) {
        // Optional: write code that calls your task1 function to make sure that it works as you expect it to
    }

    public static void task1() {
        // Required: implement task 1 code here
    }
}
```

### Do not declare a package

If you put your code inside a package then the tests will pass. If you find yourself writing code that looks anything like this then stop.

```
package anything.at.all
```

If this section doesn't make sense to you yet, don't worry. You'll learn about packages later. The important thing is to not use packages in these challenges.

## Check your understanding!

- Why is it important to pay attention to file and function naming conventions in coding challenges?
- If you are doing the coding challenge in Python, what is the naming convention for the files and functions for Task 1?
- What is the naming convention for the files and functions for Task 2 in a Javascript coding challenge?
- For Javascript developers, what is the critical information to include at the end of each task file to ensure the bot can access the functions?