---
layout: post
title: Day 2: 100 days of swiftui
author: “Gurcan Gulec“
categories: programming
tags: [swift, tuples, arrays, array, tuple, enums, enum, set, sets, swiftui, hackingwithswift]
image: 100-days-of-swiftui2.jpg
---

It’s time for me to share what I learnt. 

Swift, like many other programming languages, have arithmetic operators for adding(+), subtracting(-), multiplying(*) and dividing(/). And we can use % to find the remainder of a division.

We can use + operator to sum integers but we can also use it for joining strings like:
```
let time = "what time "
let time2 = time + "is it?"  
```
This is called **operator overloading**.

`score += 5` -> If we defined “score” earlier, this is how we increment it by 5.  += is a **compound operator** example. This can also be used to add one string to another.

And if we take a look at the **comparison operators** shortly, == checks if the values on the each side are equal, != does the opposite. < means smaller than, > means greater than, <= means smaller or equal to, >= means greater or equal to.

```
if firstCard + secondCard == 2 {
    print("Aces – lucky!")
} else if firstCard + secondCard == 21 {
    print("Blackjack!")
} else {
    print("Regular cards")
}
```
This is how you use **if statement**s in Swift. It’s pretty self explanatory if you have some programming background.

It is possible to combine conditions with **combining operators**. These operators are || and &&.  With && (pronounced “and”), statement inside if will only be run when both the conditions are true. With || (pronounced “or”), statement inside if will run if one of the conditions are true.

The **ternary operator** could give me some hard times. It’s easy but could be hard to remember. It has three values. It checks the condition for the first value,  and if it is true, returns the second value, if it is false, returns the third value. So far, everything is familiar, but not the ternary operator. 

Here is an example:
```
let firstCard = 11
let secondCard = 10
print(firstCard == secondCard ? "Cards are the same" : "Cards are different")
```
It checks if the cards are equal to each other and according to that, second or the third statement will be printed. In the example, we will get “Cards are different”, since the firstCard and secondCard are not equal.

Then we have the switch statement.
```
switch weather {
	case "rain":
	print("Bring an umbrella")
	case "snow":
	print("Wrap up warm")
	fallthrough
	default:
	print("Enjoy your day!")
}
```
Alright, at least this is familiar. If we have many conditions, instead of using if, if else, we can use switch structure. It’s really important to give a default value at the end of the switch condition. If weather is anything other than the conditions we defined, it will use the default value. fallthrough keyword can be used if we want the next case the be ran as well. In the example, if we choose “snow” as weather value, execution will continue with the next case.  But if we choose “rain” as the value, it will not go to next case because ‘case “rain”’ doesn’t have “fallthrough” keyword.

The last thing I wanna mention, or we could say I learnt with the third day is range operators which is something I am kinda unfamiliar with. Half open range operator (..<) creates range up to but excludes the last value and closed range operator (…) creates range up to and includes the last value as well.  `1..<5` includes the numbers from 1 to 4. 1…5 include the numbers from 1 to 5. They are helpful with switch blocks.

Alright, note to myself at the end of the day. I know I need to take a look at the syntax of ternary operator. Everything else is clear. Or is it? 

Before I finish I would like to state that I am following [100 days of SwiftUI](https://www.hackingwithswift.com/100/swiftui) and most of the examples are taken from [hackingwithswift.com](https://www.hackingwithswift.com). If you haven’t visited Paul Hudson’s great website. Check it out and support the guy. He has tons of free Swift content. It’s a great place to start learning Swift. 

And be persistent!
