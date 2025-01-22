# Grundlagen und Commands in Go

## Einleitung
In diesem Markdown-Dokument findest du eine strukturierte Übersicht über die wichtigsten Grundlagen und Befehle der Programmiersprache Go. Jeder Begriff wird entweder erklärt, anhand eines Beispiels demonstriert oder mit anderen Begriffen verknüpft, um die Logik dahinter verständlicher zu machen. Lass uns eintauchen! 🚀

---

### 1. Go
**Definition:** Eine Open-Source-Programmiersprache, die von Google entwickelt wurde, bekannt für ihre Einfachheit, Effizienz und Unterstützung von Nebenläufigkeit.
**Beispiel:**
```go
package main
import "fmt"

func main() {
    fmt.Println("Hallo, Go!")
}
```
**Erklärung:** Dieses einfache Programm gibt "Hallo, Go!" auf der Konsole aus. Es zeigt, wie minimalistisch Go ist.

---

### 2. Go Module
**Definition:** Ein Paket-Management-System für Go, das Abhängigkeiten organisiert und verwaltet.
**Verknüpfung:** Wird oft in Kombination mit `go mod init` und `go get` verwendet.
**Beispiel:**
```bash
go mod init meinprojekt
```

---

### 3. go run
**Definition:** Führt eine Go-Datei direkt aus, ohne eine ausführbare Datei zu erstellen.
**Beispiel:**
```bash
go run main.go
```

---

### 4. go build
**Definition:** Kompiliert den Quellcode zu einer ausführbaren Datei.
**Beispiel:**
```bash
go build main.go
./main
```

---

### 5. go fmt
**Definition:** Formatiert den Go-Code gemäß den Standardrichtlinien.
**Erklärung:** Es stellt sicher, dass der Code sauber und einheitlich ist.

---

### 6. go mod init <modulname>
**Definition:** Initialisiert ein neues Go-Modul.
**Beispiel:**
```bash
go mod init github.com/username/meinmodul
```

---

### 7. go get
**Definition:** Lädt und installiert Go-Abhängigkeiten.
**Beispiel:**
```bash
go get github.com/gin-gonic/gin
```

---

### 8. go install
**Definition:** Kompiliert und installiert ausführbare Programme.
**Beispiel:**
```bash
go install github.com/username/meinprogramm
```

---

### 9. go test
**Definition:** Führt Tests für Go-Pakete aus.
**Beispiel:**
```bash
go test ./...
```

---

### 10. package main
**Definition:** Definiert das Hauptpaket eines Programms.
**Erklärung:** Jedes ausführbare Go-Programm benötigt das `main`-Paket.

---

### 11. import
**Definition:** Importiert Pakete in den Quellcode.
**Beispiel:**
```go
import "fmt"
```

---

### 12. func
**Definition:** Deklariert eine Funktion in Go.
**Beispiel:**
```go
func add(a int, b int) int {
    return a + b
}
```

---

### 13. fmt.Println
**Definition:** Gibt Text in der Konsole aus.
**Beispiel:**
```go
fmt.Println("Das ist ein Beispiel!")
```

---

### 14. var
**Definition:** Deklariert eine Variable.
**Beispiel:**
```go
var name string = "Go"
```

---

### 15. :=
**Definition:** Kurznotation für die Deklaration und Initialisierung von Variablen.
**Beispiel:**
```go
name := "Go"
```

---

### 16. const
**Definition:** Deklariert eine Konstante.
**Beispiel:**
```go
const PI = 3.14
```

---

### 17. if und else
**Definition:** Kontrollstrukturen für Bedingungen.
**Beispiel:**
```go
if x > 10 {
    fmt.Println("Größer als 10")
} else {
    fmt.Println("Kleiner oder gleich 10")
}
```

---

### 18. for
**Definition:** Erstellt eine Schleife in Go.
**Beispiel:**
```go
for i := 0; i < 5; i++ {
    fmt.Println(i)
}
```

---

### 19. range
**Definition:** Iteriert über Arrays, Slices, Strings oder Maps.
**Beispiel:**
```go
for index, value := range []string{"a", "b", "c"} {
    fmt.Println(index, value)
}
```

---

### 20. switch
**Definition:** Führt bedingte Anweisungen basierend auf Werten aus.
**Beispiel:**
```go
switch day := "Montag"; day {
case "Montag":
    fmt.Println("Start der Woche")
default:
    fmt.Println("Nicht Montag")
}
