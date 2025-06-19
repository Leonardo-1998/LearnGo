# My Learning GoLang in Udemy

## Day 1 (Set up Awal)

Pada Visual Studio code cari dan install extension **go** by **Go Team at Google**

Buat file dengan nama app.go (Extension go)
Dalam file buatlah package main

```go
package main
// nama package main digunakan untuk menunjukan go dimana execution dimulai
```

### Print Hello World (Terminal)

```go
import "fmt"

func main (){
    fmt.Print("Hello World")
    // Gunakan "" agar di anggap sebagai string
    // '' (Kutip satu tidak di anggap sebagai string di GoLang)
}
```

Module (Project)
1 Moduke bisa memiliki beberapa file yang memiliki 1 package yang sama
Untuk 1 package yang

Untuk mengubah project menjadi module perlu menggunakan command

```js
go mod init <PATH>
```

Setelah melakukan init maka kita dapat melakukan build dengan command

```js
go build
```

Yang kemudian akan membuat file .exe yang dapat dijalankan dengan memasukan PATH file kedalam terminal

## Day 2

### func main(){}

Dalam 1 package yang sama yang boleh ada 1 function yang bernama main
Funcion ini di berikan nama main agar **Go** tau function apa yang harus dijalankan ketika file .exe di jalankan

### GoLang Data Type

- int (Non-Decimal Number)
- float64 (Decimal Number)
- string (Text)
- bool (True or False)
- uint (Unsigned Integer => Non - Negative Number)
- int32 (32-bit signed integer) https://id.wikipedia.org/wiki/32-bit
- rune (Unicode Code Point) https://www.geeksforgeeks.org/go-language/rune-in-golang/
- unint32 (32-bit unsinged integer)
- int64 (64-bit number)

### Development

Untuk menjalanakan program kita dalam development cukup gunakan

```go
go run .
go run <FILE_NAME>
```

### Variable

Untuk mengasssign data type ke suatu variabel cukup memberikan data typenya setelah nama variable

Digunakan jika kita ingin mengassign secara manual data type

```go
var investmentAmount float64 = 1000
var expectedReturnRate float64 = 5.5
var years float64 = 10
```

Digunakan jika kita ingin mengassign secara otomatis oleh **Go** data type

```go
investmentAmount := 1000
expectedReturnRate := 5.5
years := 10
```

Bisa mengdekralasi beberapa variable dalam 1 line yang sama

```go
// Tipe data menjadi sama semua, yaitu float64
var investmentAmount, years float64 = 1000, 10

// Tipe data sesuai dengen data yang dimasukkan
var investmentAmount2, years2 = 1000, "10"
var expectedReturnRate float64 = 5.5
```
