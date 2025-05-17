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

How do you ask a question? Do you seek a simple yes or no answer, or do you pose a question that expands beyond its original scope? These are considerations we often overlook. When people ask yes-or-no questions, they may not be aiming to truly learn but rather to bypass a perceived roadblock. However, this mindset can limit growth.

Consider this: if you ask yourself, “Is this question stupid?” or “Will this make me look dumb?”, you are only restricting your potential. Chances are, others around you are pondering the same thing. Eventually, someone has to speak up. If no one does, everyone risks remaining in ignorance.

This is why asking smart questions is essential. Not only can it yield more helpful information than expected, but it also cultivates habits that support continued learning and deeper understanding.

## The Role of Smart Questions in Software Engineering

Now, you might wonder what any of this has to do with software engineering. The answer? Everything. As you’ll learn (or already know), communication is one of the most crucial skills in the field.

When working in teams, collaboration thrives on the ability to express ideas clearly, question assumptions, and build upon each other's suggestions. Smart questions help breed innovation and foster the development of quality software.


## Smart Question Analysis: Code Implementation

Let’s analyze a real-world example to explore what does not constitute a smart question. Below is a link to a Stack Overflow post titled [Polymorphism giving error when using variable C#](https://stackoverflow.com/questions/79401749/polymorphism-giving-error-when-using-variable-c-sharp)
The poster presents a scenario involving polymorphism in C# and shares the following code:

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

The poster attempts to assign a value to the value field through an interface-type reference, which causes a compilation error. They want to know how to use child class properties without declaring those fields in the base interface.

## Why It’s Not a Smart Question

Despite including code and stating their issue, this question does not meet the criteria of a smart question. Here's why:

1. Lack of Clarity: The question lacks a clearly defined problem statement and goal.


2. Insufficient Research: It appears that the poster hasn’t reviewed documentation or beginner tutorials, where polymorphism fundamentals are covered.


3.  Basic Knowledge Gaps: The error is due to a misunderstanding of polymorphism and interface usage. Casting or using dynamic types could resolve the issue, but these are basic fixes.

Even though I’m unfamiliar with C# specifically, the top-voted answer explains three approaches:

- Use a dynamic type,

- Cast to the correct child type,

- Redesign the interface to include shared behavior.

Instead of directly addressing the question, the answer begins by asking probing questions—suggesting the original poster hasn’t fully thought through the design.

## Personal Reflection and Insights

This exercise helped me reflect on my own approach to asking questions. Often, I avoid asking because I think I already understand. But if I’m not asking any questions, maybe I don’t understand as well as I think I do. Smart questions help expose blind spots, challenge assumptions, and enhance not just individual understanding, but group learning as well.

Moving forward, I aim to:

- Ask more questions, even when unsure,

- Think critically about how I frame my inquiries,

- Avoid surface-level yes/no queries,

- Embrace the discomfort of not knowing.

This mindset will help me grow not only as a student but as a future software engineer. It also keeps instructors accountable—if they can’t answer a good question, it might signal a gap worth exploring together.


## Final Thoughts

Asking smart questions benefits everyone: the asker gains clarity, the responder deepens their understanding, and the entire team grows. Reflecting on this Stack Overflow post, it's clear that the quality of your question significantly influences the quality of the help you receive.
