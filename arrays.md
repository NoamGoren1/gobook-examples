
### Initialize array to 0 values

---
```go
a := [3]int{}
println(a)
```
```output
[0 0 0]
```
---
### Initialize with values

---
```go
b := [3]int{10, 20, 30}
println(b)
```
```output

[10 20 30]
```
---
### Set to width of provided literal

---
```go
c := [...]int{5 + 5, 20, 30}
println(c)
```
```output
[10 20 30]
```
---
### Compare arrays

---
```go
println(b == c)
```
```output
true
```
---
### Set by index, blank are initialized to 0

---
```go
d := [6]int{1, 2: 4, 5, 5: 100}
println(d)
```
```output
[1 0 4 5 0 100]
```
---
### Multidimensional array

---
```go
e:= [2][4]int{}
println(e)
```
```output
[[0 0 0 0] [0 0 0 0]]
```
---
