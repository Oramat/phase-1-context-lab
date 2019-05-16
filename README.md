# JavaScript Advanced Functions: Context Lab

## Learning Goals

* Explicitly override context with `call` and `apply`

## Introduction

In this lab, we're going to build the time-card and payroll application using
the record-oriented approach again. This lab will feature the same topic and
area of work as the previous lab; _however_, _how_ we call and use functions
will change with our new knowledge. While the code will stay _mostly_ the same,
you're going to need to use `this` a lot more.

The tests guide you to implementing a time card system: when someone enters the
company's state of the art technical office, the employee has to insert their
card in a time-clock which will record the time they came in. When it's time to
leave, the employee will "punch out."

For simplicity's sake, we'll make these assumptions:

1. Assume that employees always check in and check out
2. Assume employees always check in and our on the hour
3. The time is represented on a 24-hour clock (1300 is 1:00 pm); this keeps the
   math easier and is the standard in most of the world
4. When timestamps are needed, they will be provided as Strings in the form:
   "YYYY-MM-DD 800" or "YYYY-MM-DD 1800" e.g. "2018-01-01 2300"
5. Employees will never work across days i.e. in at 2200 and out at 0400 the
   next day.

The lab tests will guide you toward a solution. Keep in mind, the goal is to
understand how to "grow" an application in "record-oriented" fashion in
JavaScript, as well as pass the lab. Make sure you're learning about this app
design while you pass the solutions.

As before, if you find yourself having extra time, use the guidance in the
previous lab to make your application more robust.

Take advantage of your collection-processing strengths that you trained up over
the last few lessons.

Put your code in `index.js`.

## A Mystery on the Horizon

You'll notice that in this lab we give you the implementation of `allWagesFor`.
As part of writing this challenge, we ran right smack into one of the most
famous bugs in JavaScript land: "the lost context bug." Because we've not
taught you to deal with it, we've "given" you this function. We think you can
solve the other tests with this little piece having been given to you.

If you find yourself having extra time, try researching this topic on your own.
We'll tell you all about it in our next lesson, though.

## Conclusion

This is one of the hardest topics in JavaScript. But you have hands-on
experience with the why and motivations of it! You're so much better off than
most JavaScript hackers who _never_ quite get the hang of it. It's been a lot
of growth, but this hard-won knowledge is going to help you do staggeringly
cool things

## Resources

* [`bind`][bind]
* [`call`][call]
* [`apply`][apply]

[bind]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Function/bind
[call]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Function/call
[apply]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_objects/Function/apply