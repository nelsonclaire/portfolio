# Week 10

_A weekly journal to keep track of the work I am doing towards each of the goals._

[Weekly outline](https://github.com/makersacademy/course/blob/master/week_outlines.md/)

------

## Goals

By the end of this week I can:

Solve a challenging technical problem by writing well crafted code?
By "well crafted code", we mean code that is well tested, easy to read and easy to change.

Secondary goals
By the end of the week, you should:

Feel more confident in your ability to complete a tech test.
Have developed a structured process to approaching complex problems, utilising TDD and good OO design skills.
Structure of the week
This week, you'll work solo to complete different technical challenges. A self assessment form will help you reflect on the quality of your code, and coaches will review your code once you believe you have achieved professional quality.

This week, you'll also come up with ideas for final projects.

Processes
This week is especially good for focusing on the question, "am I a better developer than I was yesterday?"

There are up to three tech tests this week. This means you can start from scratch three times. It means you can reflect on what was good and what was bad three times. And it means you can try new things to improve three times.

Code reviews from your coach
Your coach will tell you how to request code reviews.

Language
You can use Ruby or JavaScript for any of the challenges.

1. Bank Tech Test
    - [Bank](https://github.com/nelsonclaire/bank)

Feedback from Makers:

- Comprehensive ReadMe, and formatted well - easy to read and understand

- The user passes in the date - can you think of a way you could use the JS Date object to automate this instead? This would open up your project to less risk / external interference

- If you’re pushing each individual new transaction into this.transactions, do you also need to return something at the end of your function?

- In your account tests, you pass in mock transactions, but on lines 12 and 21 of your account class, you re-assign the transaction variable to a new - real - Transaction object. This means that any mock transactions you pass in as an argument will be reassigned

- Great separation of concerns between Bank and Statement - nice work

- As a stretch goal - you’re currently updating the balance after each transaction is made, alongside the amount of the transaction. This is a duplication of code, as the balance history can be generated with just the transaction history instead. 

- What would you need to refactor in order to just use the transaction history?

