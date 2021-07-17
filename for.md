
---
```go
import (
	"fmt"
	"math/rand"
)
```
---
Standard for statement

---
```go
for i:= 0; i < 10; i++ {
	fmt.Println(i)
}
```
```output
0
1
2
3
4
5
6
7
8
9
```
---
Condition only (while loop)


---
```go
i := 1
for i < 100 {
	fmt.Println(i)
	i = i * 2
}
```
```output
1
2
4
8
16
32
```
---
Infinite Loop

---
```go
x := 0
for {
	x++
	fmt.Println(x)
	if x == 5 {
		break
	}
}
```
```output
64
1
2
3
4
5
```
---
For range with the moon emoji skipping 4 iterations

It converts the UTf-8 representation to a 32-bit number, and the offset is incremented by the number of bytes in a rune

---
```go
x := "moon🌜y"
```
---
---
```go
for i, v := range x {
	fmt.Printf("%2v %8v %-5v\n", i, v, string(v))
}
```
```output
 0      109 m    
 1      111 o    
 2      111 o    
 3      110 n    
 4   127772 🌜    
```
---
Notes
The value returned in a for-range loop is a copy, not a reference 

---
```go
Labels
```
---
---
```go
func main() {
	samples := []string{"hello", "apple_π!"}
outer:
	for _, sample := range samples {
		for i, r := range sample {
			fmt.Println(i, r, string(r))
			if r == 'l' {
				continue outer
			}
		}
		fmt.Println("Outer")
	}
}

```
---
Goto

---
```go
func gotoer() {
	a := rand.Intn(10)
	for a < 100 {
		if a%5 == 0 {
			goto done
		}
		a = a*2 + 1
	}
	fmt.Println("do something when the loop completes normally")
done:
	fmt.Println("do complicated stuff no matter why we left the loop")
	fmt.Println(a)
}
```
---
---
```go
gotoer()
```
```output
do something when the loop completes normally
do complicated stuff no matter why we left the loop
159
```
---

