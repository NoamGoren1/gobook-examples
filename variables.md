
---
```go
import "fmt"
```
---
Declare and initialize

---
```go
var a int = 10
```
---
Inferred type

---
```go
var b = 10
```
---
Initialized to 0

---
```go
var c int
```
---


---
```go
fmt.Println(c)
```
---


Multi initializer

---
```go
var d, e int = 10, 20
```
---
Inferred multi

---
```go
var f, g = 10, "wow cool"
```
---
Multiline initializer

---
```go
var (
	h    int
	i        = 20
	j    int = 30
	k, l     = 40, "hello"
	m, n string
)
```
---


---
```go
fmt.Println(h, i, j, k, l, m, n)
```
---


Shorthand initializer

---
```go
o := 10
p, q := 30, "hello"
fmt.Println(o, p, q)
```
---
Const declaration

---
```go
const (
	idKey   string = "id"
	nameKey        = "name"
)
```
---
---
```go
fmt.Println(idKey, nameKey)
```
---



