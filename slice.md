
---
```go
import "fmt"
```
---
Create from an array

---
```go
array := [4]int{1,2,3,4}
slice := array[:3]
fmt.Println("array:", array)
fmt.Println("slice:", slice)
```
```output
array: [1 2 3 4]
slice: [1 2 3]
```
---
Shorthand initializer

---
```go
slice := []int{10, 0, 0}
fmt.Println(slice)
```
```output
[10 0 0]
```
---
Initialize with make

---
```go
slice := make([]int, 3)
fmt.Println(slice)
```
```output
[0 0 0]
```
---
Append two slices together

---
```go
a := []int{10, 20, 30}
b := []int{1, 2: 3, 4, 5: 10}
c := append(a, b...)
fmt.Println(c)
```
```output
[10 20 30 1 0 3 4 0 10]
```
---
Use the make function for predefined size each element initilized to 0

---
```go
e := make([]int, 5)
fmt.Printf("%v len: %v cap %v\n", e, len(e), cap(e))
```
```output
[0 0 0 0 0] len: 5 cap 5
```
---
Sets the capacity, which saves the runtime doing work to incease size if it's known ahead of time

---
```go
f := make([]int, 5, 32)
fmt.Printf("%v len: %v cap %v", f, len(f), cap(f))
fmt.Println()
```
```output
[0 0 0 0 0] len: 5 cap 32
```
---
