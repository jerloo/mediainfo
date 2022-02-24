# mediainfo

Copied from https://gist.github.com/phelian/81bbb30cd78aceb05c8d467243edb217 for my personal use.

## Usage

```go
import "github.com/jerloo/mediainfo"

created, err := mediainfo.GetVideoCreationTimeMetadataFromFile(movieFile)
if err!=nil {
    return err
}
if err != nil {
    fmt.Println(err.Error())
    return
}

fmt.Printf("Movie created at (%s)\n", created)
```