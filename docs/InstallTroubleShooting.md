(TODO: Add table of contents.)

# 개요

여러분이 Go를 (소스 또는 바이너리 배포판 등에서) 설치하면서, 여러분의 Go는 의도한대로 동작하지 않을 수 있습니다. 이 페이지는 비교적 일반적이거나 진단하기 어려운 문제에 대한 몇 가지 해결 방법들을 수집하고 팁과 솔루션을 제공하는 것을 목적으로 하고 있습니다.

# 팁 (Tips)
## 환경 (Environment)

시작하려면 먼저 다음을 확인해주세요:

  * GOROOT
    * 이것은 **반드시** 여러분이 바이너리 배포판을 사용하고 그것이 기본 위치에 설치되지 않았을때만 설치되어야 합니다.
  * [GOPATH](http://golang.org/cmd/go#GOPATH_environment_variable)
    * 여러분이 원하는 소스의 디렉토리에 설정해야 합니다. (서드파티(third party) 패키지에서도 적용).
    * `:`로 구분된 절대 경로 목록으로 설정할 수도 있습니다. (또는 윈도우즈 에서는 `;`).
    * Note that ~/some/path is not absolute and will probably not work the way you expect (try $HOME/some/path instead).
    * GOPATH should not be set to or contain GOROOT
  * GOBIN
    * This should only be set if you _really_ know what you're doing... The default should be fine.
  * GOOS, GOARCH, GOHOSTOS, GOHOSTARCH
    * You shouldn't need to set these in normal cases.

Under linux and darwin, make sure that any of the above variables which are set are actually exported.  When you run the ` env | grep GO ` command, they should be listed.  You can also check your environment with the ` go env ` command.  In bash, this is done with the ` export GOPATH ` (if it's already set) or ` export GOPATH=/path/to/gopath ` command (similarly for the other variables), usually in your .bashrc or .bash\_profile.

## GOROOT vs GOPATH
Packages under GOROOT store their source files in

` $GOROOT/src/pkg/import/path/*.go `

Notice that this is ` src/pkg `; under GOPATH, source files are stored in

` $GOPATH/src/import/path/*.go `

Because of this inconsistency, it is generally not recommended that GOPATH be set to or contain GOROOT; its directories will be searched automatically for imports regardless of the GOPATH setting.

# 문제 해결하기(Troubleshooting)
#### ` go build ` 명령어가 말을 안들어요!
` go build ` 명령어는 오직 바이너리 파일을 생성합니다. 만약 여러분이 go build를 패키지 디렉토리에서 실행시켰다면, 패키지를 정상적으로 빌드할 것입니다 (그리고 컴파일에 문제 또한 보여줄 겁니다), 하지만 빌드한 파일을 설치해주지는 않습니다. 정상적인 설치를 원한다면, ` go install ` 명령어를 사용해야 합니다. 만약 여러분이 바이너리 파일 생성을 의도했지만 아무것도 만들어지지 않은 경우, 여러분의 프로젝트가 ` main ` 패키지 안에 있는지 그리고 GOBIN을 세팅하지 않았는지 확인해주세요.

#### Why does ` go get ` report ` "Fetching https://runtime/cgo?go-get=1" `?
If you have a source distribution, make sure that your packages are up-to-date.  Also double check the environment above.

#### When cross compiling, I get ` "runtime/extern.go:135: undefined: theGoos" `
Read [[WindowsCrossCompiling]] for some helpful scripts.  You can also use the ` --no-clean ` argument when you're building the cross-compile toolchain via ` make.bash `.

#### Why does ` go get ` work for some packages and report ` permission denied ` in ` $GOROOT ` for some others (with GOPATH set properly)?
If you at any point installed the package in ` GOROOT ` (either by having no ` GOPATH ` set or by including ` GOROOT ` itself in ` GOPATH `) then there might still be a directory in ` $GOROOT ` (which is always checked first) that is overriding your ` GOPATH `.  To verify, run ` go list -f {{.Dir}} importpath ` and if it reports a directory under ` $GOPATH ` try deleting that first.

## Still need help?
Visit us on IRC or ask on the mailing list.  You will want to provide the output of the following commands, in addition to any errors you are getting:
```
go version
go env
env | grep GO
```