# Module 1

## Studios
We are providing instructions formatted as comments that you can copy over to the IDE.

### Class 1 Studio: Donuts
```
/**
  * Filename: donuts.c
  * Save in Folder: ~/workspace/module1/studios/donuts
  * 
  * Write a program which greets the user, introduces the flavor of the day, and 
  * takes the user's order . 
  * 
  * Taking their order involves asking two questions: 
  * "How many donuts?" and "How much do you want to pay?"
  * Finally, inform the user of the total cost of their order. 
  * Don't forget to include sales-tax, which is, let's say, 5%.
  * 
  * Example:
  *      $ ./donuts
  *      Welcome to the Loop Hole!
  *      Today's Manager's Special is:
  *      Crunch Jelly: A traditional jelly donut in which the jelly filling is made entirely of Capn' Crunch Berries (Just Berries)
  *      How many would you like? 3.33333
  *      How much would you like to pay per donut (suggested price is $4.35 each)? 2.5
  *      Ok, let me prepare that for you....
  *      After tax, your total is: $8.74999125 
  *      Thank you for snacking! Loop back around here soon!
  * 
  * Remember, don't worry about rounding and your result may have a slightly
  * different number of decimal places than the example program due to imprecision.
  *
  */
```

### Class 2 Studio: Guess
This studio will be made up of three separate programs, (`guess.c`, `guess5.c`, and `guessfive.c`) The instructions for all 3 programs are included here. You will start with the first program `guess.c` and follow the directions for the other 2 programs.

```
 /**
  * Filename: guess.c
  * Save in Folder: ~/workspace/module1/studios/guess
  * 
  * Part 1
  * Write a "guessing game" program that allows the user to guess a number between 1 and 10.
  * The program should continuously reprompt the user until they get the correct answer.
  * 
  * You can simply decide on a "correct answer" and hard-code that number into your code. 
  * Supposing for example that you decide to make 4 the correct answer, you will probably have a line like this:
  *     
  *     int answer = 4;
  * 
  * Notice that you'll need to keep track of how many guesses have happened so far, so that you can properly print "Guess #<n>"
  * Example: 
  * 
  *     I'm thinking of a number between 1 and 10. Can you guess what it is?
  *     Guess #1: 5
  *     Wrong!
  *     Guess #2: 9
  *     Wrong!
  *     Guess #3: 4
  *     Correct!
  * 
  */
```
```
 /**
  * Part 2
  * Filename: guess5.c
  * Save in Folder: ~/workspace/module1/studios/guess5
  * 
  * Write another program called guess5, which gives the user only 5 chances to get the answer:
  * This should only involve some minor tweaking, so you can make a copy of your guess.c file using the cp command:
  *        $ cp guess.c guess5.c
  * Open up guess5.c and make changes there.
  *
  * Example:
  *     $ ./guess5
  *     I'm thinking of a number between 1 and 10. Can you guess what it is?
  *     Guess #1: 8
  *     Wrong!
  *     Guess #2: 5
  *     Wrong!
  *     Guess #3: 1
  *     Wrong!
  *     Guess #4: 7
  *     Wrong!
  *     Guess #5: 6
  *     Wrong!
  *     Sorry, you ran out of guesses.
  * 
  */
 ```
 ```
 /**
  * PART 3 
  * Filename: guessfive.c
  * Save in Folder: ~/workspace/module1/studios/guessfive
  *
  * Most likely, you've been using a while loop so far. Let's now refactor, and use a for loop instead, just for kicks.  
  * Write another program in a file called guessfive.c, which behaves exactly like guess5, but is implemented with a for loop. 
  * (But if you did use a for loop in guess5, then use a while loop here.)
  * 
  */
```

### Class 2 Studio: Lovely Rectangle

```
  /**
   * Filename: rectangle.c
   * Save in Folder: ~/workspace/module1/studios/rectangle
   * 
   * Write a program that "draws" a rectangle made of hearts "<3" on the console.
   * Your program should prompt the user for a width and a height, and then
   * print the corresponding rectangle.
   * 
   * Example:
   *    $ ./rectangle
   *    Width: 8
   *    Height: 3
   *    <3<3<3<3<3<3<3<3
   *    <3<3<3<3<3<3<3<3
   *    <3<3<3<3<3<3<3<3
   * 
   */
```
### Class 3 Studio: Repeat

```
  /**
   * Filename: repeat.c
   * Save in Folder: ~/workspace/module1/studios/repeat
   *
   * In a file called repeat.c write a program that repeats a phrase multiple times. 
   * You program should prompt the user for both a phrase, and a number of repeats.
   * 
   * Example:
   * $ ./repeat
   * Give me a phrase: I am NOT a talking robot!
   * How many times should I say it? 5
   * I am NOT a talking robot!
   * I am NOT a talking robot!
   * I am NOT a talking robot!
   * I am NOT a talking robot!
   * I am NOT a talking robot!
   * 
   * Twist 1: VALIDATE - Your program should only accept values that are at least 1, and no greater than 100 
   * for the "how many times" argument. If the user fails supply a number within that range, 
   * the program should continue prompting until they do.
   * 
   * Example:
   * $ ./repeat
   * Give me a phrase: Oh na na, what's my name.
   * How many times should I say it? (between 1 and 100): -4
   * How many times should I say it? (between 1 and 100): 238
   * How many times should I say it? (between 1 and 100): 2
   * Oh na na, what's my name.
   * Oh na na, what's my name.
   * 
   * Twist 2: ROUND - Modify your program to accept a double type, rather than an int, 
   * for the "how many times" argument. This means that the user's input might not be a whole number. 
   * So in order to decide how many times to repeat the phrase, your program should 
   * take the input value and round it to the nearest integer.
   *
   * Example: 
   * Give me a phrase: I <3 LaunchCode
   * How many times should I say it? (Positive number please): 1.7
   * I <3 LaunchCode
   * I <3 LaunchCode
   * Hint: use the round function (reference here). Note that you'll need to 
   * include the Math library at the top of your .c file
   * 
   */
```

### Class 3 Studio: Dollars and Cents

```
  /**
   * Filename: dollarsandcents.c
   * Save in Folder: ~/workspace/module1/studios/dollarsandcents
   *
   * Another useful function from <math.h> is round. This function takes a floating point number, 
   * and returns the nearest integer:
   * 
   *     int x = round(4.7);
   *     // the value of x is 5
   * 
   *     int y = round(4.4);
   *     // the value of y is 4 
   * 
   * Remember when your donut shop was charging customers crazy fractional dollar amounts, 
   * like $7.2494328374? Now we're able to do a better job in that sort of situation.
   * 
   * Write a program that prompts the user for a floating point dollar amount, 
   * and then tells them the actual dollar amount:
   * 
   * Example:
   * $ ./dollarsandcents
   * Gimme a dollar amount: 7.2494328374
   * Oh, I think you mean $7.250000000
   * (It still looks stupid because of the trailing 0s but thats ok. We'll learn how to fix that some other time.)
   *
   * Of course, in this case we do not want to round all the way down to the nearest integer. Doing so would have 
   * given us $7.00. Instead we want to round to the nearest 2 decimal places. Unfortunately, round isn't 
   * fancy enough to do that. But with a little bit of clever arithmetic, you can get around this no problem!
   * 
   * As a bonus, the work you do here will be very helpful for last section of Pset 1.
   * 
   */
```
## Follow Alongs
We are providing pseudocode for the follow along tasks so you can start writing the program before watching the video.  You will find instructions to complete the task in the video.
The pseudocode will be formatted as comments so you can copy it over to the CS50 IDE. And if you are ever confused :confused:  about what to do, you can always refer to the video for help.

### Class 1 Task: Hello-0
This is your first follow-along and we are providing pseudocode for the follow along tasks so you can start writing the program before watching the video.  Please refer to the <a href="../CS50-IDE/file-management-resource.md" target="_blank">File Management Resource</a> if you need a refresher.  
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder. If you’re not sure how to write the program, check <a href="http://cdn.cs50.net/2015/fall/lectures/1/w/notes1w/notes1w.html#c" target="_blank">here</a> for a reminder. 

```
 /**
  * Filename: hello-0.c
  * Save in Folder: ~/workspace/module1/follow_alongs/hello
  * 
  * Include the stdio library
  * Add main method
  * Add { }
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.
  *
  */
```
### Class 1 Task: Hello-1
If you’re not sure what to do check <a href="http://cdn.cs50.net/2015/fall/lectures/1/w/notes1w/notes1w.html#c" target="_blank">here</a> for a reminder. 
```
 /**
  * Filename: hello-1.c
  * Save in Folder: ~/workspace/module1/follow_alongs/hello
  * 
  * Include the stdio library
  * Add main method
  * (Hint: Don't forget to add curly braces { }) 
  *    Print "hello, world" and a new line (Hint: \n)
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.  
  *
  */
```

### Class 1 Task: Hello-2
If you’re not sure what to do check <a href="http://cdn.cs50.net/2015/fall/lectures/1/w/notes1w/notes1w.html#c" target="_blank">here</a> for a reminder. 
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder.
```
 /**
  * Filename: hello-2.c
  * Save in Folder: ~/workspace/module1/follow_alongs/hello
  * 
  * Include the stdio library
  * Add main method
  * (Hint: Don't forget to add curly braces { })
  *    Print "State your name: "
  *    Print "hello, " and a new line 
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.
  *
  */
```

### Class 1 Task: Adder
If you forgot how to declare a variable check <a href="http://cdn.cs50.net/2015/fall/lectures/1/w/notes1w/notes1w.html#writing_code" target="_blank">here</a>. 
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder.
```
 /**
  * Filename: adder.c
  * Save in Folder: ~/workspace/module1/follow_alongs/adder
  * 
  * Include the stdio library
  * Include the cs50 library
  * Add main method
  * (Hint: Don't forget to add curly braces { })
  *    Print "Please give me an int: "
  *    Declare a variable called x of type int 
  *    Declare a variable called y of type int 
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.
  *
  */
```

### Class 1 Task: F2C
If you forgot how to assign a variable look <a href="http://cdn.cs50.net/2015/fall/lectures/1/w/notes1w/notes1w.html#writing_code" target="_blank">here</a> or to get user input of type float check <a href="https://reference.cs50.net/cs50.h/GetFloat" target="_blank">here</a>. 
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder.  
```
 /**
  * Filename: f2c.c
  * Save in Folder: ~/workspace/module1/follow_alongs/f2c
  * 
  * Include the stdio library
  * Include the cs50 library
  * Add main method
  * (Hint: Don't forget to add curly braces { })
  *    Print "Temperature in F: "
  *    Declare a variable called f of type float and assign the user input to it.
  *    (Hint: We can get user input of type float using the cs50 library function GetFloat())
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.
  *
  */
```

### Class 2 Task: Conditions-0
If you forgot how to assign a variable look <a href="http://cdn.cs50.net/2015/fall/lectures/1/w/notes1w/notes1w.html#writing_code" target="_blank">here</a> or to get user input of type int check <a href="https://reference.cs50.net/cs50.h/GetInt" target="_blank">here</a>. 
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder.
```
 /**
  * Filename: conditions-0.c
  * Save in Folder: ~/workspace/module1/follow_alongs/conditions
  * 
  * Include the stdio library
  * Include the cs50 library
  * Add main method
  * (Hint: Don't forget to add curly braces { })
  *    Print "Please give me an int: "
  *    Declare a variable called n of type int and assign the user input to it.
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.  
  *
  */
```

### Class 2 Task: Conditions-1
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder.
```
 /**
  * Filename: conditions-1.c
  * Save in Folder: ~/workspace/module1/follow_alongs/conditions
  * 
  * Include the stdio library
  * Include the cs50 library
  * Add main method
  * (Hint: Don't forget to add curly braces { })
  *    Print "Please give me an int: "
  *    Declare a variable called n of type int and assign the user input to it.
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.  
  *
  */
```

### Class 2 Task: Positive
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder.
```
 /**
  * Filename: positive.c
  * Save in Folder: ~/workspace/module1/follow_alongs/positive
  * 
  * Include the stdio library
  * Include the cs50 library
  * Add main method
  * (Hint: Don't forget to add curly braces { })
  *    Declare a variable called n of type int and assign the user input to it.
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.
  * 
  */
```

### Class 2 Task: Debugging with Dan Armendiz
Copy the pseudocode to the CS50 IDE and use the information below to name the file and place it in the correct folder.
```
 /**
  * Filename: count.c
  * Save in Folder: ~/workspace/module1/follow_alongs/count
  * 
  * Include the stdio library
  * Include the cs50 library
  * Add main method
  * (Hint: Don't forget to add curly braces { })
  *    Print "Please enter a number: "
  *    Declare a variable called num of type int and assign the user input to it.
  *    Assign the expression num / 2 to the variable num
  *    Print "Your halved number is: %i\n" using num as the value for the placeholder %i
  * 
  * You will find instructions to complete this task in the video. 
  * You will be modifying this code as you go along.
  * 
  */
```
