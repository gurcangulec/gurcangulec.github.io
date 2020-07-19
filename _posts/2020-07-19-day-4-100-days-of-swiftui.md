---
layout: post
title: day 4
author: “Gurcan Gulec“
categories: programming
tags: [loop, loops, for loop, while loop, repeat loop, break, continue, swiftui, hackingwithswift]
image: 100-days-of-swiftui2.jpg
---

I already failed to keep my promise to myself about completing a day of [100 Days of SwiftUI – Hacking with Swift](https://www.hackingwithswift.com/100/swiftui) and writing a blog post. But I don’t give up just yet.

At first I planned to combine two days in this post, but then I decided to go day by day, even though some posts might be short.

Here we go with the loops.
```swift
for number in count {
    print("Number is \(number)")
}
```
This is how you create a **for loop** in Swift considering you defined a range of numbers like `let count = 1...10`. Same approach is possible with arrays as well. And if you don’t use the constant for loop gives you, you can use an underscore so you don’t create a useless value. Simply put, _if you don’t need to use “number” value in that for loop we just created, use an underscore instead._ Although it is simple, this is something I didn’t get a grasp on on my first walkthrough of 100 days of SwiftUI. 

And then, there is while and repeat loops. Even though **while loop** is similar to for loop, **repeat loop** is a little different. If you are familiar with other programming languages, it works like a do while loop. Meaning condition check comes at the end and that means the loop is executed at least once.

You can exit a loop with `break` command.

You can exit multiple loops by giving outer loop a label like:
```swift
outerLoop: for i in 1…10 {
	blah blah
	another loop
}
```
Now you can use `break outerLoop` in the inner loop and exit both loops.

You can use `continue`  command to skip the current item and continue with the next one.

It is possible to create infinite loops with `while true` since true is always true but we need to exit the loop at some point otherwise program will crash at some point.

Here we complete day 4. 

Be persistent!
