# 개요

GOPATH 환경변수는 Go 프로젝트와 해당 바이너리의 소스를 가지는 $GOROOT의 의부 디렉토리를 지정하는데 사용됩니다.

더 다양한 정보를 위해 [go command](http://golang.org/cmd/go/#hdr-GOPATH_environment_variable) and [go/build package](http://golang.org/pkg/go/build/) 문서를 확인해보시기 바랍니다.

$GOPATH 변수는 리스트가 될 수 있기에, 이 문서의 나머지 부분은 별도로 명시하지 않는 한 첫 번째 요소는 $GOPATH를 의미합니다.

## 통합 GOPATH

OS X 또는 Linux (bash)에서 다음의 값을 PATH에 추가하면 모든 $GOPATH/bin이 추가됩니다.
```
${GOPATH//://bin:}/bin
```

## 디렉토리 구성

`"X/Y/Z"` 형태의 import 경로를 가진 패키지 소스는 아래와 같은 디렉토리 구성을 갖습니다.
```
$GOPATH/src/X/Y/Z
```

`"X/Y/Z"` 형태의 import 경로를 가진 바이너리 패키지는 아래와 같은 디렉토리 구성을 갖습니다.
```
$GOPATH/pkg/$GOOS_$GOARCH/X/Y/Z.a
```

소스가 `$GOPATH/src/A/B`에 위치한 바이너리 명령어는 아래와 같은 디렉토리 구성을 갖습니다.
```
$GOPATH/bin/B
```

## 리포지토리 통합 및 "go gettable" 프로젝트 생성
When fetching a package the go tool looks at the package's import path to discover a URL. For instance, if you attempt to
```
go get github.com/go-kit/kit
```
the go tool will get the source from the project hosted at https://github.com/go-kit/kit/. It will clone the repository to
```
$GOPATH/src/github.com/go-kit/kit
```

As a result, if (from your repository project) you import a package that is in the same repository, you need to use its "full" import path - the place "go get" puts it. In this example, if something else wants to import the "kit" package, it should import "github.com/go-kit/kit" rather than "kit".

## Tips and tricks

### Use a single GOPATH

Even though the GOPATH may be a list of directories, it is generally sufficient to use a single GOPATH for all Go code on your machine.  Since all packages retrieved with "go get" have a unique URL (and thus a unique path on disk), having more than one GOPATH is almost never necessary when building with the Go tool.

## FAQ
### Why won't ` $GOPATH/src/cmd/mycmd/*.go ` build?
When the go command is looking for packages, it always looks in ` $GOROOT ` first.  This includes directories, so if it finds (as in the case above) a ` cmd/ ` directory in ` $GOROOT ` it won't proceed to look in any of the GOPATH directories.  This prevents you from defining your own ` math/matrix ` package as well as your own ` cmd/mycmd ` commands.