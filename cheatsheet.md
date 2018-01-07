## Swift 4 Cheat Sheet 

- [Variables](#variables)
- [Control Flow](#control-flow)
- [Classes](#classes)
- [Methods](#methods)


### Variables

- Types

| Type        | Values  |
| ------------- |:-------------:|
| String      | "test", "some text..." | 
| Int      | 1, 2, 1000, 99999 | 
| Bool      | true, false       |
| Classname | UIView, UIButton, etc... |
| Float/ Double      | 1.0, 2.0, 10.001, 99.949391 |


-  Variables declaration (Mutable)
```swift
var mutableInt:Int = 1
var mutableFloat:Float = 1.0
var mutableDouble:Double = 1.0

// all valid
mutableInt = 2
mutableFloat = 2.0
mutableDouble = 2.0
```
- Constants
Declaring constants:
```
let [VARIABLE_NAME]:[TYPE] = [VALUE]
```
```swift
let name:String = "some name"
// name = "another name" // error
```
- Optionals

```swift
var optinalName:String? = nil
optinalName = "Test"

if let myName = optinalName {
 optinalName
}
```

### Control Flow
- If / Else
```swift
var condition = 10
if condition < 10 {
    // when condition is less than 10
} else if condition > 10  {
    // when condition is greater than 10
} else {
    // when condition is equal to 10
}

```

- Switch Case
```swift
var val = 5
switch val {
    case 1:
        "foo"
    case 2:
        "bar"
    default:
        "baz"
}
```
- For loop
```swift
var name = ["test1", "test2", "test3"]
for name in names {
    print("Hello, \(name)!")
}

```

### Classes

```swift
class MyClass : OptionalSuperClass,
OptionalProtocol1, OptionalProtocol2 {

    var myProperty:String
    var myOptionalProperty:String?
    // More properties...

    // Only need override if subclassing
    override init() {
        myProperty = "Foo"
    }

    // More methods...
}
```

### Methods
```swift
func sayHi() -> String {
    return  "hi" 
}

func sayHi(name: String) -> String {
    return "Hi " + name
}
```

### Struct
```swift
struct User {
    var username:String = "username"
    var age:Int = 0 
}
```