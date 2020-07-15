---
layout: post
title: 100 days of swiftui - day 2
author: “Gurcan Gulec“
categories: programming
tags: [swift, tuples, arrays, array, tuple, enums, enum, set, sets, swiftui, hackingwithswift]
image:
---
Here is what I learnt today, or what I already knew but I got to go over it one more time.

`let cars = ["bmw", "mercedes", "honda"]` -> This is how you declare an array.

`cars[0]` -> This is how you read the value “bmw” inside the array. Array positions count from 0.

`let bikes = Set([“honda”, “suzuki”, “ducati”])` -> This is how you create a set. The items inside a set are unordered and items will only appear once. So even if we have duplicate values in it, they will be ingnored and values cannot be read with numerical positions.

`var name = (first: “Paul”, last: “Hudson”)` -> This is how you create a tuple. Tuples are fixed in size, not possible to add or remove items. The **types** of the items inside a tuple cannot be changed. It is possible to access items in a tuple with numerical positions or by naming them. Like `name.0` or `name.first`.

## But, the question is: Where and when to use them?
When we need a specific, fixed collection of data where each of them needs to have a precise location or name -> Tuple

When the data in a collection must be unique and should be able to checked really quickly if the item is there -> Set

When you need a collection of data that needs to be in a certain order or that can contain duplicates -> Array

```
let computerParts = [
    “graphics card”: 299,
    “ram”: 159
]
```

And this is how you create a dictionary. And then we can read the data with the “graphics card” value like `computerParts["graphics card"]`. “graphics card” here is an identifier and these **identifiers** are called **keys**.

If we try to read a value for “cpu”, we would get nil. Meaning Swift doesn’t have a value for “cpu” key. But instead of that we could provide a default value like `computerParts["cpu", default: "Unknown"]`

`var teams = [String: String]()` -> This is how you create an empty dictionary with strings for keys.

`teams[“Kobe”] = “Lakers”` -> This is how you add an entry to an empty dictionary.

`var results = [Int]()` -> This is how you create an empty array to store integers.

`var words = Set<String>()` -> This is how you create an empty set.

```
enum Result {
    case success
    case failure
}
```

This is how you create an enum. It is used when we want a type to have some certain values. In the example, result can only have two values, “success” or “failure”.
`let result4 = Result.failure` -> This is how you use an enum.

```
enum Activity {
    case bored
    case running(destination: String)
    case talking(topic: String)
    case singing(volume: Int)
}
```

Here is an example of enum associated values. These values are “destination”, “topic” and “volume”. Basically, they let us attach more information to our enums.

`let talking = Activity.talking(topic: “programming”)` -> This is how we use associated values.

```
enum Planet: Int {
    case mercury
    case venus
    case earth
    case mars
}
```

And last but not least. This is how you create an enum that stores integer values for each of its cases. 

`let earth = Planet(rawValue: 2)` This is how you create an instance of an enum case.

All these makes sense to me now, but when it comes to using these, I know I will struggle a lot. But let’s see. If I understand them better somehow in the future, I will come back and explain these better. 
