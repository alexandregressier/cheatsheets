---
title: Kotlin, Swift, and TypeScript
layout: 2017/sheet
updated: 2021-05-03
category: Java & JVM
prism_languages: [kotlin, swift, typescript]
intro: |
    Highlight the differences between [Kotlin](https://kotlinlang.org/), [Swift](https://swift.org/), and [TypeScript](https://www.typescriptlang.org/)
---

Variables
---------
{: .-three-column}

### Mutability

Kotlin
```kotlin
val foo = "Foo"
var bar = "Bar"
bar = "Baz"
```
Swift
```swift
let foo = "Foo"
var bar = "Bar"
bar = "Baz"
```
TypeScript
```ts
const foo = "Foo"
let bar = "Bar"
bar = "Baz"
```

### Type annotations

Kotlin
```kotlin
val foo: String = "Foo"
```
Swift
```swift
let foo: String = "Foo"
```
TypeScript
```ts
const foo: string = "Foo"
```

### Comments

All
```kotlin
// Single line comment
/* Multiline
   comment */
```

Strings
-------

### Interpolation

Kotlin
```kotlin
println("My name is $name and I'm ${currentYear - 1997}")
```
Swift
```swift
print("My name is \(name) and I'm \(currentYear - 1997)")
```
TypeScript
```ts
console.log(`My name is ${name} and I'm ${currentYear - 1997}`)
```

Functions
---------
{: .-three-column}

### Single expression 

Kotlin
```kotlin
fun foo(bar: String): String =
    bar
```
Swift
```swift
let foo: (String) -> String = { bar in
    bar
}
```
TypeScript
```ts
const foo = (bar: String) =>
    bar
```

### Regular

Kotlin
```kotlin
fun foo(bar: String): String {
    return bar
}
```
Swift
```swift
func foo(bar: String) -> String {
    return bar
}
```
TypeScript
```ts
function foo(bar: string) {
    return bar
}
```

Classes
-------
{: .-three-column}

### Data classes

Kotlin
```kotlin
data class Person(
    val name: String,
    val age: Int? = null,
)
val alex = Person(name = "Alex")
```
Swift
```swift
struct Person {
    let name: String
    let age: Int? = nil
}
let alex = Person(name: "Alex")
```
TypeScript
```ts
interface Person {
    name: string
    age?: number
}
const alex: Person = {name: "Alex"}
```
