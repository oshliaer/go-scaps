# go-scaps
<!-- TOC -->

- [google.golang.org](#googlegolangorg)
  - [drive/v3](#drivev3)

<!-- /TOC -->

## Apps
### Static web-server
- [ran](https://github.com/m3ng9i/ran)

## google.golang.org
### drive/v3
https://stackoverflow.com/a/34830165/1393023
```go
import "google.golang.org/api/drive/v3"
func InsertFile(d *drive.Service, title string, description string, mimeType string, filename string) (*drive.File, error) {
    f := &drive.File{Name: filename, Description: description, MimeType: mimeType}
    return d.Files.Create(f).do()
}
```
