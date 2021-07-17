


Notes
+ Map keys can be any comparable type

---
```go
import "fmt"
```
---
Trying to add a key to an unitialized map casuses a panic

---
```go
	var a map[string]int
```
---
Initializing an empty map doesn't cause an error when adding keys

***Adding a new key with ++ doesn't currently work in Gobook***

---
```go
totalWins := map[string]int{}
totalWins["lakers"] = 20
totalWins["suns"]++
fmt.Println(totalWins)
```
```output
map[lakers:20]
```
---
Initialize with map literals

---
```go
x := map[int]string{
	10: "wow cool",
	40: "I like it",
}
fmt.Println(x)
```
```output
map[10:wow cool 40:I like it]
wow cool
```
---
Multi level map literal 

---
```go
	teams := map[string][]string{
		"Orcas":   {"Fred", "Ralph", "Bijou"},
		"Lions":   {"Sarah", "Peter", "Billie"},
		"Kittens": {"Waldo", "Raul", "Ze"},
	}
	fmt.Println(teams)
```
```output
map[Kittens:[Waldo Raul Ze] Lions:[Sarah Peter Billie] Orcas:[Fred Ralph Bijou]]
```
---
Check if the key exists and print it if it does

***checking a key doesn't currently work in Gobook***

---
```go
	v, ok := teams[0]
	if(ok) { 
		fmt.Println(v)
	}
```
---
Delete a key

---
```go
delete(teams, "Orcas")
fmt.Println(teams)
```
---


