# 德尔 Go 语言编码规范

### 关于 go test

每一个导出对象都需要写测试

go test ./...

go test -cover ./...

测试覆盖率不能低于80%

### 关于 import

按照字母排序

建议分为三组：标准库、第三方库、本地库

```go
import (
  "fmt"
  "os"

  "go.uber.org/atomic"
  "golang.org/x/sync/errgroup"
  
  "com.deer/test"
)
```



### 关于 golint

每一个导出对象都需要在头部加入注释 注意空格

golint ./...

### 关于新建项目

新建项目都要基于 go module 模式

go env -w GO111MODULE=on

go mod init projectname

go mod tidy

### 关于 git

提交必须写注释

提交前必须执行如下命令 要求通过

```go
go fmt ./...
go vet ./...
golint ./...
go test ./...
```


[Uber Go 语言编码规范]: https://github.com/xxjwxc/uber_go_guide_cn


