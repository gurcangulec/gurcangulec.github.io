---
layout: post
title: 100 days of swiftui
author: “Gurcan Gulec“
categories: programming
tags: [documentation]
image: 100-days-of-swiftui.jpg
---
Although I started doing [100 Days of SwiftUI](https://www.hackingwithswift.com/100/swiftui/1) a while ago. I stopped doing it after day 20-something. Then I decided I will stick with it this time and I will let people know about my progress each time I complete a “day”. I am not saying I will finish it in 100 days or I will keep updating everyone *everyday*. That’s something humanely impossible.  But I will observe where it takes me when I complete it.

## But, what is 100 Days of SwiftUI?
I would say it’s an excellent initiative by [Paul Hudson](https://twitter.com/twostraws). This guy is a developer who tries to help people make their way into Swift programming with his online content and books. He has tons of free stuff as well and one of them is 100 Days of SwiftUI. 

Alright, let’s get to it!

Since I already have some programming experience, first day was not much of a struggle. I will shortly summarise it though.

`var interpolation = "something"`  -> This is how you declare a variable.

`str = "change"` -> This is how you change it. No need to type _var_ again.

`str = 38` -> This is how you mess it up. Cannot be change to an integer because it’s a string.
```
var str = """
This is how
you create
multi-line strings
"""
```
`var pi = 3.14` -> This is how you create a double.

`var awesome = true` -> This is how you create a boolean.

`var str = "This is how string \(interpolation) works."` -> Value of variable **interpolation** will be replaced in the string. Output will be “This is how string something works.”

`let another = "thing"` -> This is how you create a constant. Constant cannot be changed later on.

So far Swift was able to **infer** the type as we declare variables. But we can be specific about the type.

`let year: Int = 1990` -> This is an example of type annotation. It’s how you explicitly declare a variable.

That’s all so far for the first day. It took me about two [pomodoro](https://en.wikipedia.org/wiki/Pomodoro_Technique)s to write these down. I will keep you updated as much as I can. 
