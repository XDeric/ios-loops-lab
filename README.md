# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**
var range = 1...150
for i in range {
print(i)
}
***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**
var range = 142...159
for i in range {
print(i)
}
***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**
var range = 15...80
for i in range {
if i % 2 == 0{
print(i)
}
}
***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**
var range = 19...51
for i in range {
if i % 2 != 0{
print(i)
}
}
***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**
var range = 1...100
for i in range {
if i % 10 == 5{
print(i)
}
}***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**
var range = 1...40
for i in range {
if i % 10 == 7{
print(i)
}
}
***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`
var range = 20...150
for i in range {
if i % 3 == 0{
print(i)
}
}
***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`
var range = 20...150
for i in range {
if i % 3 == 0 && i % 2 == 0{
print(i)
}
}***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`
var range = 20...150
for i in range {
if i % 10 == 4{
print(i)
}
}***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`
var range = 20...150

for i in range{
if i == 31 || i == 35{
print(i)
}
if i <= 60 && i >= 40{
print(i)
}

}
***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// It's an infinite loop because i is greater than than 3 and it will increment by 1 and will continue to do so because when it checks back at the conditional it will always be greater than 3.
```

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
var i = 5

while (i > 3 && i < 9) {
i += 1
print(i)
}

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3 && i < 1003) {
    i += 1
}
```
var i = 5

while (i > 3 && i < 1005) {
i += 1
}
***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
var i = 5

while (i > 3 && i < 1005) {
i += 1
if i % 2 == 0{
print(i)
}
}
***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```
The difference is the name where one is repeat and the other is while. Repeat is a do while that does the repetition then it check the condition whereas while check the condition first. the output is the same even though the steps they go about it is different. 
***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

Break ends the loop at where ever it's at or up to whereas continue makes the loop stop where it is at and start from the beginning again kind of like skipping the condition you state.

let puzzleInput = "great minds think alike"
var puzzleOutput = ""
let charactersToRemove: [Character] = ["a", "e", "i", "o", "u", " "]
for character in puzzleInput {
if charactersToRemove.contains(character) {
continue
}
puzzleOutput.append(character)
}
print(puzzleOutput)
// Prints "grtmndsthnklk"

In this example from the reading break will give you the output gr and continue gives you grtmndsthnklk.
***
## Question 17

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```
1
2
3
8
9
10
continue skiped all the numbers that fir the condition and just print out the other numbers.


***
## Question 18

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```
1
2
3


***
## Question 19

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
```
x = 1, y = 1
x = 2, y = 1
x = 3, y = 1

y stays as 1 because of the condition where it checks if y is equal to 2 so it skips it and go back to 1.
***
## Question 20

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

for i in 0...10{
for j in 0...10{
print ("\(i),\(j)", separator: "", terminator: " ")
}
print("")
}
***
## Question 21 

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

for i in 0...10{
for j in 0...10{
if i - j == 5{
print ("\(i),\(j)", separator: "", terminator: " ")
}
}
print("")
}
***
## Question 22

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```
var n = 5
var i = 0
while i <= n{
print(i * i)
i += 1

}

***
## Question 23

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

***
var n = 3
var asterix = 0
var line = ""

for _ in 0..<n{
while asterix < n{
line += "*"
asterix += 1
}
print(line)
}
