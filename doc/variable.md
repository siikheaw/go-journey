# Variable
In Go (Golang), variables are used to store data values. Here's an overview of how variables work in Go:

## Variable Declaration
### Basic syntax:
```go
var name type
var name type = value
```

### Examples:
```go
var age int
var name string = "John"
var isActive bool = true
```

### Short Variable Declaration
Go provides a shorthand syntax using := (only inside functions):
```go
age := 25
name := "Alice"
isActive := true
```

### Multiple Variable Declaration
```go
// Multiple variables of same type
var x, y, z int

// Multiple variables with initialization
var a, b = 1, 2

// Short declaration
x, y := 10, 20
```

### Zero Values
Go automatically initializes variables with zero values if not explicitly set:

```go
int: 0
string: ""
bool: false
float: 0.0
Pointers, slices, maps, channels, functions, interfaces: nil
```

## Variable Scope

- Package level: Declared outside functions, accessible throughout the package
- Function level: Declared inside functions, only accessible within that function
- Block level: Declared inside blocks (if statements, loops), only accessible within that block

## Type Inference
Go can automatically infer types:
```go
var number = 42        // inferred as int
var pi = 3.14         // inferred as float64
var message = "Hello" // inferred as string
```

## Constants
Use const for unchanging values:
```go
const Pi = 3.14159
const MaxUsers = 100
```
Variables in Go are statically typed, meaning their type is determined at compile time and cannot change during runtime.
