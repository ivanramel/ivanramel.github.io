---
layout: essay
type: essay
title: "The questions people don't dare to ask"
# All dates must be YYYY-MM-DD format!
date: 30 Jan 2025
published: true
labels:
  - Software Engineering
---

<img width="500px" class="rounded float-start pe-4" src="../img/markthequestionmarkguy.png">

## Questioning your question
How do you ask a question? Do you ask for a yes or no? Or do you ask a question that expands beyond your original one? These are things we don't think enough about because people asking for simple yes or no questions probably are not there to learn, but to get pass a roadblock they think won't be a problem down the road. This opens upon another slew of avenues of questions. If you ask yourself "is this question stupid" or "will it make me look dumb". Then you are only limiting yourself as other people around you are probably thinking the same idea, and eventually everyone will make a fool of themselves if no one speaks up to ask the question on everyone's mind. This is where asking smart questions are important as not only will you manage to get more information than you hoped for, but it will build good habits in furthur your education or knowledge of a particular subject.

Now you might be wondering what this has to do with software engineering. Well it has everything to do with them. As you should know by now one of the key things you should or will learn in your software engineering is that communication is key. This is mainly prevalent when working in groups as people would need to communicate with each other to breed new and innovative ideas which can lead to a great product or software as the end result. 

## Smart Question Analysis: Code Implementation
Linked below is a post from StackOverflow that I will be analyzing on whether or not it qualifies as a smart question:
[Polymorphism giving error when using variable C#](https://stackoverflow.com/questions/79401749/polymorphism-giving-error-when-using-variable-c-sharp)

In this question the poster explains their situation, acknowledges their current knowledge around the problem, and the question they have. In this case the poster wants how they could implement various child classes without having variables present in the base class:
```
using System;

class Program
{
    public interface A {}

    public class B : A
    {
        public int value = 0;
    }

    public class C : A
    {
        public int value = 1;
    }
    static void Main(string[] args)
    {
        A myB = B();
        A.value = 3; //error her
    }
}

```

Would this question be considered a smart question? Personally, this question does not qualify as a smart question because other than it being basic, it also seems to be a question easily answered when you know the basics. While I am not one to talk about the basics about this particular piece of code since it seems to be coded in C#, a language I have no experience in whatsoever, if we take a look at the highlighted answer to this post it says something along the lines of asking him questions before telling him is three options of, using a dynamic variable, declaring/casting the variable as certain type, or extending it use case to inherit its properties. 

## In conclusion...
Asking smart questions is not only a benefit to the asker who gains more insight into a problem they probably have been mulling over for a few days, but also to the person who answered it as they could test their knowledge on the topic further their understanding because if one can teach it they understand it. This also made me think about the type of questions I ask, or lack thereof. Since I don't ask many questions I believe I understand it, but in reality I don't understand it at all as I am not asking questions, even smart ones. So one take away I can gain from this would be to ask more questions, especially smart ones to further my personal understanding of my education and to keep instructors on their toes if they don't know the answer to my question.
