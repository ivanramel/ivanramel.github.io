---
layout: essay
type: essay
title: "Improving the Quality of a Rock, Still Makes It a Rock"
# All dates must be YYYY-MM-DD format!
date: 12 Feb 2025
published: true
labels:
 - Coding Standards
---


<img width="400px" class="rounded float-start pe-4" src="../img/eslint-logo.png">

“Quality is more important than quantity. One home run is much better than two doubles.” – Steve Jobs

## To what standards are we held to?

When I first started using ESLint with VSCode, it felt like a constant struggle. My natural coding style clashed with the formatting rules ESLint enforced. Take this example of ESLint-compliant code:

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
Now compare that to how I would normally write it:

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
In truth, I exaggerated how much ESLint clashed with my style. It mostly just affects spacing and formatting. Still, getting used to it wasn’t seamless. However, I’ve noticed that once I correct all the ESLint warnings, my code looks cleaner and is easier to read. Over time, I'm starting to appreciate that.

## The Growing Pains of Adopting Standards

Using ESLint became particularly frustrating during a Practice WOD. I wanted to make a new branch with a fresh workspace but found that ESLint stopped giving me feedback. Turns out, I forgot to enable it for that new branch. My workaround was to run ESLint manually after every block of code or once I was finished.

That experience taught me that automated tools are only useful if they’re properly integrated into your workflow—and that consistency is more important than I initially thought.



## Standards, shamdards. What's the point?

If my code works and mostly looks the same as the ESLint version, why bother conforming to it? This question is superficial. It ignores one key aspect of professional coding: other people have to read your code.

When you’re working on larger projects with a team, inconsistent or messy code becomes a liability. Poor formatting wastes time and leads to misunderstandings. Nobody wants to debug spaghetti code.

“Code is like humor. When you have to explain it, it’s bad.” – Cory House

Well-formatted code should speak for itself. If your teammates have to ask what something means—or worse, dig through your logic because it’s poorly presented—you’ve failed at communication.

## Where do we go from here?

After learning from these growing pains and integrating ESLint, what’s the next step? Improvement doesn’t stop with the adoption of standards. You have to critique those standards and refine your own practices.

Is your style guide actually readable?

Why enforce some rules and not others?

Can your standards evolve as your team does?

Like the software development lifecycle, improving your code style is an ongoing process. There's always a better, cleaner way to express logic—and the only way to find it is to keep questioning and improving.
