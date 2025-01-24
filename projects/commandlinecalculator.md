---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Command Line Calculator"
date: 2024
published: true
labels:
  - C
summary: "Gets the user's input, using command line arguments, of a basic single digit math operation and calculates it. Uses array of pointers to make an array of functions to store functions within an array."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
</div>

The command line calculator is a program I made during my ICS 212 class in the Fall 2024 semester as a 2nd year. The purpose of this program was to make a simple calculator that could perform single digit math on two integers based on the user's input. This was to teach us about taking command line arguments from main and either perform addition, subtraction, multiplication, or division on the user inputted integers.

While this may seem like a basic C program it taught me alot about receiving command line arguments from the main function in C. This was due in part with the fact that this program and all my other programs made in ICS 212 were made in a command prompt and with my case since I was using a Mac OS computer I used terminal. This helped me get used to command line with things ranging from changing directories to resolving a crash from my program.

Here is a sample of my code that can be seen below:

```c
 // For-loop containing error checks before we proceed with the math operation
  for(i = (argc - 1); i >= 0; i--) {
    // Error check: checking if there is two numbers and a math operator present in the command line argument
    if(argc != 4){
      printf("ERROR: 4 command line arguments are needed, %d are present\n", argc);
      return 1;
    }
    // Error check: checking if the 1st command line argument is a character between '0' and '9'
    if(argv[1][0] < '0' || argv[1][0] > '9'){
      printf("ERROR: %c is not an integer between 0 - 9\n", argv[1][0]);
      return 1;
    }
    // Error check: checking if the 2nd command line argument is a valid math operation symbol
    if(argv[2][0] != '+' && argv[2][0] != '-' && argv[2][0] != '.' && argv[2][0] != '/'){
      printf("ERROR: %c is not a valid math operation. Use + - . /\n", argv[2][0]);
      return 1;
    }
    //Error check: checking if the 3rd command line argument is a character between '0' and '9'
    if(argv[3][0] < '0' || argv[3][0] > '9'){
      printf("ERROR: %c is not an integer between 0 - 9\n", argv[3][0]);
      return 1;
    }
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
