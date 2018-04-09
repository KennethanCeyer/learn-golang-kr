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
패키지를 가져 올 때 Go 도구는 패키지의 임포트 경로를 확인하여 URL을 찾습니다. 예를들어 여러분이 아래와 같은 커맨드라인을 사용할 때
```
go get github.com/go-kit/kit
```
go 도구는 https://github.com/go-kit/kit/에 호스트된 프로젝트에서 소스를 가져옵니다. 이때 리포지토리를 아래 경로로 클론합니다.
```
$GOPATH/src/github.com/go-kit/kit
```

결과적으로, (리포지토리 대상 프로젝트에서) 동일한 리포지토리에있는 패키지를 가져 오는 경우 여러분은 "전체" 임포트 경로를 사용해야합니다 - 이 예제에 "kit" 패키지를 불러오기를 원하는 경우 "kit" 보다는 "github.com/go-kit/kit"을 임포트 하는 것이 좋습니다.

## 팁과 트릭들

### 단일 GOPATH를 사용하세요

GOPATH가 디렉토리 목록일 수 있더라도 일반적으로 시스템의 모든 Go 코드에 대해 단일 GOPATH를 사용하는 것으로 충분합니다. "go get"으로 검색된 모든 패키지는 고유한 URL(그리고 각 디스크의 고유한 경로)을 갖기 때문에 Go 도구를 사용하여 빌드 할 때 둘 이상의 GOPATH 설정이 필요한 경우는 거의 존재하지 않습니다.

## FAQ
### `$GOPATH/src/cmd/mycmd/*.go`가 빌드되지 않는 이유가 뭔가요?
Go 커맨드가 패키지를 찾을 때 대부분 `$GOROOT`를 먼저 찾습니다. This includes directories, so if it finds (as in the case above) a ` cmd/ ` directory in ` $GOROOT ` it won't proceed to look in any of the GOPATH directories.  This prevents you from defining your own ` math/matrix ` package as well as your own ` cmd/mycmd ` commands.