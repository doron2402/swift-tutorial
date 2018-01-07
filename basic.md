## Swift Basic

- [Basic](#basic)
  - [`Constants and Variables`](#constants-and-variables)
  - [`Delcaring Variables`](#delcaring-variables)
  - [`Type Annotations`](#type-annotations)
  - [`Naming Constants and Variables`](#naming-constants-and-variables)
  - [`Print`](#print)
  - [`Comments`](#comments)
  - [`Semicolons`](#semicolons)
  - [`Semicolons`](#semicolons)
  

#### Basic
Swift is a new programming language for iOS, macOS, watchOS, and tvOS app development. Nonetheless, many parts of Swift will be familiar from your experience of developing in C and Objective-C.

Swift provides its own versions of all fundamental C and Objective-C types, including Int for integers, Double and Float for floating-point values, Bool for Boolean values, and String for textual data. Swift also provides powerful versions of the three primary collection types, Array, Set, and Dictionary, as described in Collection Types.

#### Constants and Variables  

Constants and variables associate a name (such as maximumNumberOfLoginAttempts or welcomeMessage) with a value of a particular type (such as the number 10 or the string "Hello"). The value of a constant can’t be changed once it’s set, whereas a variable can be set to a different value in the future.
```swift
let someConstant = "Value goes here"
let anotherContant = 1000
```
** If you're coming from Javascript that will be a little bit confusing since javascript use `const` for constant and `let` is a variable type that is made to be updated.

#### Delcaring Variables 
Constants and variables must be declared before they’re used. You declare constants with the let keyword and variables with the var keyword. 
```swift
let iAmConstantVariable = 1000
var temporaryVariable = 1000
// we can also declare multiple variables in one line
var a = 1, b = 2, c = 2
```

#### Type Annotations
You can provide a type annotation when you declare a constant or variable, to be clear about the kind of values the constant or variable can store. Write a type annotation by placing a colon after the constant or variable name, followed by a space, followed by the name of the type to use.

- String
```swift
var hiMessage: String
```
- Int
```swift
var userAge: Int
// we can also declare mutliple variables
var userAge, userId: Int
```
- Double
```swift
var balance: Double 
```

#### Naming Constants and Variables
Constant and variable names can contain almost any character, including Unicode characters:
```swift
let π = 3.14159
let 你好 = "你好世界"
let 🐶🐮 = "dogcow"
```

#### Print
It's always useful to print your variable when you tired of debugging

```swift
var name = "some name"
print(name)

// Printing a variable with string
print("Hi \(name)")
// also we can use
print("hi", name)
```

#### Comments
Use comments to include nonexecutable text in your code, as a note or reminder to yourself. Comments are ignored by the Swift compiler when your code is compiled.

```swift
// single line comment

/* 
Multi line
Comments
*/
```

#### Semicolons
Unlike many other languages, Swift doesn’t require you to write a semicolon (;) after each statement in your code, although you can do so if you wish. However, semicolons are required if you want to write multiple separate statements on a single line:

```swift
var name = "some name"; print(name);
```