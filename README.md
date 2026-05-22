### `$ ./fourteen`

```go
package main

import "fmt"

type Engineer struct {
	Alias    string
	Role     string
	Location string
	Project  string
	Contact  string
}

func New() *Engineer {
	return &Engineer{
		Alias:    "Fourteen",
		Role:     "Full-stack engineer & sysadmin",
		Location: "Malta",
		Project:  "SafetyNet",
		Contact:  "contact@safetynet.at",
	}
}

func (e *Engineer) SayHi() {
	fmt.Printf("> hi, I'm %s\n", e.Alias)
	fmt.Printf("> %s — based in %s\n", e.Role, e.Location)
	fmt.Printf("> currently building %s\n", e.Project)
	fmt.Printf("> reach me at %s\n", e.Contact)
}

func main() {
	New().SayHi()
}
```

```text
$ go run fourteen.go
> hi, I'm Fourteen
> Full-stack engineer & sysadmin — based in Malta
> currently building SafetyNet
> reach me at contact@safetynet.at
```
