---
title: Submitting Code Samples
date: 2015-06-06
template: draft.jade
---

Over the past twenty months I've interviewed about as many candidates for my team. As part of the interview process, we ask our candidates to submit a code sample. I've seen some great submissions, and some that could use some work. Here are some tips and best practices based on my experiences.

### Take your time

This can be tricky. Maybe you were asked to spend a couple hours on the assignment, so you could stick to that as a time limit. Perhaps you're doing this after a long day at work, and you're up staying past your bedtime. Whatever the case may be, I've seen a lot of submissions where the candidate stuck to a suggested or self-imposed time limit, and it showed.

If you need to, use version control to commit your work at your time limit, but keep going if you can.

### Submit work you're proud of

You should not only spend as much time as you need, but ultimately, you should submit work you're proud of. It should not be missing anything you'd do for production code, so write tests, refactor, format, and polish. Not to intimidate you, but this sample should be representative of your best work. Don't worry about whether your best is "good enough." Focus on doing what you know how to do, to the best of your ability.

### Prioritize maintainability

In general, the most important priority for *any* code is maintainability. This is especially true when strangers are reading your code. It should be readable and easy to understand. Pay attention to:

* consistent formatting - this should be easy, but you would be surprised
* naming things - obviate comments by choosing verbose, descriptive names
* structure & organization - break apart the problem, don't write one huge function

### Choose your preferred language

You may be tempted to choose a language you saw on the job listing. Do so if that's what the position is about, but often you have a bit of freedom here. You want to demonstrate your skill with a tool, so choose your best tool.

### Use your preferred toolset

Whether it's using a functional library or your favorite testing framework, don't be afraid to have an opinion and demonstrate it. Part of being a well-rounded developer means not only having a strong grasp of your language, but the ecosystem around it.

### Dig in

Think about the problem at a deeper level than what the requirements specify. Research the problem space and consider things like internationalization. You don't need to over-engineer the solution, but your understanding of the domain will show in both your code and the interview.

### Solve it yourself

This may be obvious, but I sometimes hear, "well, if I did this for real, I would research existing solutions." Yeah, you might, but this is about *your* abilities. It's OK to look up docs and APIs, but avoid using someone else's implementation.

### Put it down for a couple days

Coming back to your code after the dust has settled will give you a fresh perspective. You'll spot minor improvements, and potentially, come up with a better design. Your brain has probably been running a subconscious background process since you started, so see what it comes up with.

Even after you've submitted the solution, don't be afraid to keep working on it. Ask if you're not sure, but you can probably make changes until the day of the interview.

### Use branches

Branches can be used to demonstrate multiple approaches as part of a single solution. You may experiment with different designs to find the optimal solution. If you try an approach that doesn't work, keep it around on a branch. I appreciate hearing what a candidate tried, and how they evolved their design.

### Write a README

You're usually writing a self-contained, runnable project. Document how to run your code. It's also useful if it's hosted somewhere public like GitHub, to explain what it's about.

### Be ready to learn

Hopefully the interview process includes you in the code review! *Invite* their feedback and keep a very open mind. This is a learning opportunity in how other engineers reason about code, and with your code no less. It's OK to volunteer improvements and critique yourself, and you may even be asked to.

One of my favorite questions from a candidate: "are there any more suggestions you could offer me?" It's *really hard* to ask for feedback, but this is a strong sign that you're always looking to improve. Even if you don't get the job, you should walk away a better developer.

### Bonus points

These suggestions are not nearly as important as the previous ones, but they could set you apart:

* include a demo/test app
* write build/test/run scripts - and include them in the README
* test accessibility, performance, cross-browser, etc.

### Further reading

Here are some other great tips, all on Stack Exchange (Programmers & Workplace):

* [on clean code](http://programmers.stackexchange.com/a/51155/52486)
* [how to interview with a code sample](http://programmers.stackexchange.com/questions/94492/interview-review-another-developers-code/94507#94507)
* [non-technical concerns](http://workplace.stackexchange.com/a/1315)

I hope this helps you submit better code samples. If you have any questions or your own suggestions to offer, please share them in the comments.
