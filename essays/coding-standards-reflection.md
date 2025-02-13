---
layout: essay
type: essay
title: "Coding Standards"
# All dates must be YYYY-MM-DD format!
date: 12 Feb 2025
published: true
labels:
  - Software Engineering
---

<img width="400px" class="rounded float-start pe-4" src="../img/eslint-logo.png">

“Quality is more important than quantity. One home run is much better than two doubles.” – Steve Jobs

## To what standards are we held to?
Once I started using ESLint with VSCode, it became a pain as the way I type code directly conflicts. Take this piece of code for example which uses ESLint:

```Typescript
function fib(): number[] {
  let i: number = 1;
  const fibList: number[] = [0, 1];
  while (fibList.length !== 50) {
    fibList.push(fibList[i] + fibList[i - 1]);
    i++;
  }
  return fibList;
}
console.log(fib());

```
Now while this nice and plain, lets compare this with how I would usually code it:

```Typescript
function fib(): number[]{
  let i: number = 1;
  const fibList: number[] = [0, 1];
  while(fibList.length !== 50){
    fibList.push(fibList[i] + fibList[i - 1]);
    i++;
  }

  return fibList;
}

console.log(fib());
```
Now whie this may seem the same, it's because it pretty much is. I might have slighty exaggerated that ESLint clashes with my coding style because it really doesn't. It only affects the way I space things. As you can see I don't usually have a space before my opening curly brackets, or loops. And not to mention a lack of a new line before the end of the code. 

The more I code with ESLint, the more I will get use to it. When I look at my code after dealing with all the ESLint errors, it looks much nicer and readable compared to how I coded it before. But that doesn't mean its still not a pain to use as for example when doing a practice wod I wanted to do another attempt. And because of that I wanted to try and make a new branch with my current workspace but with the code cleared out. While that did work, I noticed that when coding that it did not give me any errors, even with the lack of a newline at the end of the code. The solution I found was to just run ESLint everytime I finished a block of code, or at the end to ensure it fits the coding standards set by ESLint.

## Standards, shamdards. Whats the point?
So if the way I code, and the way ESLint wants me to code is the same, why should it matter that I follow ESLint to make my code more *prettier*? This is pretty much a surface level question as this does not address or acknowledge how other people will read your code. I say this because once we start working on bigger projects we will have to work in teams, which means eventually working on the same code. Now how will someone improve or fix your code if its unreadable or not presentable? They won't. It would be a waste of time shifting through terrible code only to figure out the problem could have been solved in a few minutes had it been more organize and concise. 

Code is like humor. When you have to explain it, it’s bad. – Cory House

In essence, once you code something it should be pretty much be readable and understandable from the very first go through from looking at it, under the assumption that the reader knows their stuff. When the reader has to look something up, or ask you personally about the code you messed up somewhere, and it most likey is about the way you code things, setting aside lack of comments.

## Where do we go from here?
So after learning the errors of your ways and implementing ESLint or some other coding standard of your choice what is their left to improve your code other than the standard of relearning the basics from that one coding class? Well, you improve upon and critize your own standard. Is it good enough? Why is it strict on one thing and not the other? Like most things in life there is room for improvement and that is a cycle that well never end, kind of like the software development cycle. 
