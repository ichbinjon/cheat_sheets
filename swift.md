# iOS Swift learning

## Swift classes vs structs

A swift `class` is passed by reference. A `struct` is passed by value.

```swift
// Assuming Dog is a predefined struct

let dog = Dog()
let newdog = dog

// dog and newdog are different instances of Dog!
```

```swift
// Assuming Dog is a predefined struct
let dog = Dog()
let dogs = [Dog]
dogs.append(dog)
dogs.append(dog)

// two different instaces of Dog is inside dogs! Appending / assigning is by value on structs.
```
