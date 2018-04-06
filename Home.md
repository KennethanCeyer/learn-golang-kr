아직 번역이 모두 이루어지지 않았습니다.
조금만 기다려주시면 모든 내용이 한글로 읽기쉽게 정리됩니다. :clap:

# 목차

+ [Go를 시작하며](#go를-시작하며)
+ [Go로 작업하기](#go로-작업하기)
+ [Go에 대해 더 알아보기](#go에-대해-더-알아보기)
+ [Go 커뮤니티](#go-커뮤니티)
+ [Go 툴체인](#go-툴체인)
+ [Go의 또 다른 위키들](#go의-또-다른-위키들)
+ [Go로 동작하는 서비스들](#go로-동작하는-서비스들)
+ [Go를 이용한 프로덕션에서의 문제해결](#go를-이용한-프로덕션에서의-문제해결)
+ [Go 프로젝트에 기여](#go-프로젝트에-기여)
+ [플랫폼 관련 정보](#플랫폼-관련-정보)
+ [릴리즈 관련 정보](#릴리즈-관련-정보)

## Go를 시작하며

  - [Go 둘러보기](http://tour.golang.org)를 이용해보세요 처음 시작할 때는 이곳이 제일 좋습니다.
  - [이펙티브 Go](https://golang.org/doc/effective_go.html)는 여러분이 Go를 자유자재로 사용하도록 도와줍니다.
  - [Go 표준 라이브러리 문서](https://golang.org/pkg/)를 보시고 표준 라이브러리와 친해지세요.
  - [Go Playground](http://play.golang.org)를 이용하여 Go 프로그램을 웹에서 확인해보세요.
  - 여전히 모르겠나요? [Go 사용자들](GoUsers)과 그들의 [성공 사례](SuccessStories)를 확인해보세요. 또한 여러분이 왜 Go를 사용해야하는지 여러가지 이유들을 정리해봤습니다 [왜 Go를 사용해야 할까요?](whygo).
  - [다른언어에서 Go](FromXToGo)로 전환한 회사들을 살펴보세요.

## Go로 작업하기

Go로 여러분만의 코드를 작성하실 준비가 되셨나요? 여러분이 시작하시는데 도움을 줄 수 있는 몇가지 링크를 준비했습니다.

  - 설치 및 환경세팅
    - [공식 설치문서](https://golang.org/doc/install)를 살펴보세요.
    -  만약에 소스를 통해 직접 설치를 원하신다면, [먼저 이 링크를 읽어주세요](https://golang.org/doc/install/source).
      - [소스를 통해 설치](InstallFromSource) - 소스 설치방법의 추가적인 팁들입니다.
    - Windows 사용자인가요? [Go 설치 및 설정 및 Windows 사용자를 위한 Git, Atom](https://github.com/abourget/getting-started-with-golang)
    - Mac 사용자인가요? [Go를 어떻게 시작할까요](https://howistart.org/posts/go/1) - Go 설치 및 여러분의 첫 번째 웹 서비스 구축에 대한 단계별 안내입니다.
    - 설치중에 문제가 발생했나요? [설치문제 해결](InstallTroubleShooting)
    - 여러분이 [올바른 $GOPATH 환경변수](https://golang.org/doc/install/source#gopath)를 세팅하였는지 확인해주세요.
      - 이와 관련된 보다 많은 팁을 [여기서 확인하세요](GOPATH).
    - [다중 GOROOT](MultipleGoRoots) - 여러 Go 설치 환경과 `$GOROOT` 환경변수 설정에 대한 자세한 정보를 살펴보실 수 있습니다.
  - [Go IDE와 에디터들](IDEsAndTextEditorPlugins) - Go와 함께 사용하실 수 있는 여러분이 선호하는 에디터에 대한 정보입니다.
  - [Go를 지원하는 도구들](CodeTools) - 포맷, 린트, 베팅, 리팩토링, 네비게이션, 시각화 관련 툴들이 정리되어 있습니다.
  - Go 라이브러리와 패키지들을 살펴보세요
    - 우측 링크를 살펴봐주세요: [Go 오픈소스 프로젝트](Projects).
    - Go 패키지들을 검색해보세요: [godoc.org](http://godoc.org)
    - [Go 오픈소스 패키지 그래프](https://anvaka.github.io/pm/#/galaxy/gosearch?l=1)를 살펴보세요.
  - [의존성 관리](PackageManagementTools) - 여러분의 써드파티 패키지를 관리할 수 있는 도구의 개요입니다.
  - Go 패키지 오픈소스로 배포하기
    - 패키지를 배포할 준비가 되셨나요? [이것을 살펴봐주세요](PackagePublishing)
    - [Go 체크리스트](https://github.com/matttproud/gochecklist) - 프로젝트를 배포하기 위한 포괄적인 안내.
    - [GitHub 리포지토리 설정방법](GitHubCodeLayout) - 다른 개발자들이 여러분의 패키지를 `go get` 명령으로 쉽게 사용할 수 있도록 설정합시다.
    - [Go Package, Go](https://johnsto.co.uk/blog/go-package-go) - Go 패키지를 사용하기 쉽게 만드는 몇가지 방법을 확인하세요.

## Go에 대해 더 알아보기

Go에 대해 대략적으로 이해하셨다면, 아래에서 자세한 내용들을 추가적으로 살펴보세요.

  - [Learning Go](Learn) - Go를 알아가기 위한 내용 모음 - 초급에서 고급까지.
    - [새로운 Go 개발자를 위한 모범사례](https://medium.com/@IndianGuru/best-practices-for-a-new-go-developer-8660384302fc) - Go 커뮤니티 회원들의 인사이트.
    - [서버 프로그래밍](LearnServerProgramming) - Building web, mobile, and API servers.
    - [동시성 제어 추가정보](LearnConcurrency)
    - [에러 핸들링 추가정보](LearnErrorHandling)
    - [테스트 추가정보](LearnTesting)
    - [모바일 개발 추가정보 - Android와 iOS](Mobile)
  - [서적](Books) - Go 관련 서적 모음입니다 (일반서적과 E북)
  - [블로그](Blogs) - Go에 대해서 다루는 블로그들 입니다.
    - [팟캐스트](Podcasts) - Go에 대한 팟캐스트 및 에피소드들 입니다.
  - 비디오, 논의 및 발표
    - [GopherVids](http://gophervids.appspot.com/)는 Go 관련 비디오를 검색할 수 있는 모음집입니다.
    - [GoTalks](GoTalks) - Go에 대해 논의, 밋업을 다룹니다.
    - [스크린샷](Screencasts)
  - [본문들](Articles) - Go에 대해 더 알아갈 수 있도록 도와주는 관련 본문들 모음집입니다.
  - [연습](Training) - 무료 및 유로, Go를 위한 온라인 강의들입니다.
  - [대학 강좌](Courses) - Go를 이용한 CS 프로그램들과 수업 목록입니다.
  - [비 영어권 사용자들을 위한 자료](NonEnglish)

## Go 커뮤니티

은둔고수 Gophers들을 찾을 수 있는 링크들을 모아놓았습니다. Go 커뮤니티 멤버가 되는 것이 어떤 것을 의미하는지 이해하기위해 [Damian Gryski's keynote from the GolankUK 2015 conference](https://medium.com/@dgryski/the-go-community-f0d00e3a19e)글을 읽어보시기 바랍니다. 혹은 [Andrew Gerrand's closing keynote from GopherCon 2015](https://www.youtube.com/watch?v=0ht89TxZZnk)를 시청해보시기 바랍니다.

- Gopher들의 채팅 커뮤니티:
  - [Go 포럼](https://forum.golangbridge.org/) - 여러 주제에 대해 다루는 Go 커뮤니티.
  - [고퍼(Gopher) 슬랙 채널](http://gophers.slack.com/) - 실시간 대화가 가능한 Go 커뮤니티 ([슬랙 가입요청은 이곳에](http://blog.gopheracademy.com/gophers-slack-community/)).
  - [Golang 뉴스](http://golangnews.com) - Go 프로그래밍에 대한 알림을 원하실 때 이용하세요.
  - [/r/golang](http://reddit.com/r/golang) Go에 대해 다루는 레딧 커뮤니티.
  - 트위터를 사용하신다면, [@golang](https://twitter.com/golang) 계정을 팔로우하시고 [#golang](https://twitter.com/search?q=%23golang&src=typd) 해시태그를 주시해주세요.
  - [스택 오버플로우 (Stack Overflow)](http://stackoverflow.com/tags/go)에서 Go 관련 Q&A가 활발히 이루어지고 있습니다.
  - 매트릭스(Matrix) 사용자분들은 [#Go:matrix.org](https://riot.im/app/#/room/#Go:matrix.org)를 이용해주세요.
  - [디스코드 고퍼 (Discord Gophers)](https://discord.gg/VF92f7M)에서 디스코드(Discord)를 이용하시는 유저들을 환영합니다. 
- 메일링 리스트
  - Go 사용자들을 위한 메일링 리스트입니다 [golang-nuts](https://groups.google.com/forum/#!forum/golang-nuts) - 엄청 활발합니다!
    - 스택오버플로에 질문을 남기기전에, [이미 있는 질문은 아닌가요?](http://stackoverflow.com/tags/go)를 읽어주세요, 읽고나서 [어떤 질문이 좋은 질문일까요](HowToAsk)도 읽어주세요
  - 핵심 Go 오픈소스 프로젝트에 대한 토론을 원하시면 [golang-dev](https://groups.google.com/forum/#!forum/golang-dev)를 이용해주세요.
  - Go 릴리즈 정보를 얻을려면, [golang-announce](https://groups.google.com/forum/#!forum/golang-announce)에 참여하세요.
- 사용자 그룹 & 밋업 - [많은 도시에 밋업이 열리고 있습니다](http://www.meetup.com/find/?allMeetups=false&keywords=golang&radius=Infinity&userFreeform=Sunnyvale%2C+CA&mcId=z94086&mcName=Sunnyvale%2C+CA&sort=recommended&eventFilter=mysugg)
    - [GoBridge](http://golangbridge.org) - Go와 관련하여 소수 커뮤니티에게 전문 기술을 가르치고 다양성을 육성하는 자원봉사 단체입니다.
    - [Women Who Go](http://www.womenwhogo.org/)
    - [Go 사용자 그룹과 관련한 더 많은 정보는 이곳에서 살펴보세요.](GoUserGroups)
- [컨퍼런스](Conferences) - 다가오거나 지난 Go 컨퍼런스 및 주요 이벤트들입니다.
- [Go를 사용하는 업체](GoUsers) - 전세계에서 Go를 사용하는 업체들을 정리하였습니다.
- [Go Gopher images](Gopher)에 대해 더 많이 알아보세요 출처: by Renee French.

## Go 툴체인

  - `go` 명령어와 관련된 공식 문서는 [이곳에서](https://golang.org/cmd/go/) 볼 수 있습니다.
  - [vendoring](https://golang.org/cmd/go/#hdr-Vendor_Directories)에 대해서 알아보세요.
  - [패키지 관리 도구](PackageManagementTools)를 통해 패키지 관리 도구들을 살펴보세요.
  - [크로스 컴파일](https://rakyll.org/cross-compilation/)
  - 공유 라이브러리 (buildmode)
    - [Go 공유 라이브러리](https://github.com/jbuberel/buildmodeshared) - Go와 Python의 공유 라이브러리 생성 및 사용예제.
    - [Go 패키지를 C와 공유](http://blog.ralch.com/tutorial/golang-sharing-libraries/) - 출처: by [@ralch](https://twitter.com/ralch).
    - [Python에서 Go 라이브러리 호출](https://blog.filippo.io/building-python-modules-with-go-1-5/) - 출처: by Filippo Valsorda
    - [Ruby에서 Go 라이브러리 호출](http://c7.se/go-and-ruby-ffi/) - 출처: by Peter Hellberg
    - [Swift에서 Go 라이브러리 호출](https://rakyll.org/swift/) - 출처: by Jaana Burcu Dogan
    - [Go 네이티브 확장을 이용한 Ruby Gem 빌드](http://blog.paracode.com/2015/08/28/ruby-and-go-sitting-in-a-tree) - 출처: by @jondot
    - [gohttplib](https://github.com/shazow/gohttplib) - Go 1.5 buildmode=c-shared를 이용한 실험.
  - 자세한 내용은 아래 위키를 참조해주세요:
    - [GoGetTools](GoGetTools)
    - [GoGetProxyConfig](GoGetProxyConfig)
    - [cgo](cgo)
    - [CompilerOptimizations](CompilerOptimizations)
    - [GccgoCrossCompilation](GccgoCrossCompilation)
    - [GcToolchainTricks](GcToolchainTricks)
    - [GoGenerateTools](GoGenerateTools)
    - [Go 필수 도구](https://rakyll.org/go-tool-flags/) - 출처: by Jaana Burcu Dogan
    
## Go의 또 다른 위키들

  - [Go가 제너릭을 지원하지 않는 이유: 제너릭 의견 요약](https://docs.google.com/document/d/1vrAy9gMpMoS3uaVphB32uVXX4pi-HnNjkMEgyAHX4N4/preview) - Start here before you join the debate.
  - 동시성 제어
    - [타임아웃 (Timeouts)](https://github.com/golang/go/wiki/Timeouts) - Abandon async calls that take too long
    - [OS 쓰레드 락](https://github.com/golang/go/wiki/LockOSThread)
    - [뮤텍스 (Mutex) 또는 채널 (Channel)](https://github.com/golang/go/wiki/MutexOrChannel) - When to use one vs the other
    - [레이스(Race) 감지기](https://github.com/golang/go/wiki/RaceDetector) - How to detect and fix race conditions
  - 데이터베이스 사용하기
    - [database/sql](http://go-database-sql.org/) - Online tutorial for working with the database/sql package.
    - [TUGTBDDAwG](https://vividcortex.com/resources/building-database-driven-apps-with-go/) - Guide to building data driven apps.
    - [SQL 드라이버](https://github.com/golang/go/wiki/SQLDrivers)
    - [SQL 인터페이스](https://github.com/golang/go/wiki/SQLInterface)
  - 다른 언어 개발자를 위한
    - [자바 개발자들을 위한 Go](http://yourbasic.org/golang/go-java-tutorial/)
    - [C++ 개발자들을 위한 Go](https://github.com/golang/go/wiki/GoForCPPProgrammers)
  - 문자열
    - [Go 문자열 (Strings)](https://github.com/golang/go/wiki/GoStrings)
    - [문자열 매칭 (String Matching)](http://blog.gopheracademy.com/advent-2014/string-matching/)
  - [주석](https://github.com/golang/go/wiki/Comments)
  - [흔히 발생하는 실수들](http://blog.gopheracademy.com/advent-2014/string-matching/)
  - [에러 (Errors)](https://github.com/golang/go/wiki/Errors)
  - [GC 툴체인 (Toolchain) Tricks](https://github.com/golang/go/wiki/GcToolchainTricks)
  - [해싱 (Hashing)](https://github.com/golang/go/wiki/Hashing)
  - [Http Fetch](https://github.com/golang/go/wiki/HttpFetch)
  - [Http Static Files](https://github.com/golang/go/wiki/HttpStaticFiles)
  - [Interface Slice](https://github.com/golang/go/wiki/InterfaceSlice)
  - [Iota](https://github.com/golang/go/wiki/Iota)
  - [Method Sets](https://github.com/golang/go/wiki/MethodSets)
  - [패닉(Panic)과 복구(Recover)](https://github.com/golang/go/wiki/PanicAndRecover)
  - [Range](https://github.com/golang/go/wiki/Range)
  - [Rate Limiting](https://github.com/golang/go/wiki/RateLimiting)
  - [릴레이션 (Rationales)](https://github.com/golang/go/wiki/Rationales)
  - [Sending Mail](https://github.com/golang/go/wiki/SendingMail)
  - [신호(Signal) 핸들링](https://github.com/golang/go/wiki/SignalHandling)
  - [Simultaneous Assignment](https://github.com/golang/go/wiki/SimultaneousAssignment)
  - [Slice Tricks](https://github.com/golang/go/wiki/SliceTricks)
  - [스위치 (Switch)](https://github.com/golang/go/wiki/Switch)
  - [Table Driven Tests](https://github.com/golang/go/wiki/TableDrivenTests)


## Go로 동작하는 서비스들

여러분이 Go를 지원하는 서비스를 찾고 계신다면, 아래에 모든 것이 수록되어 있습니다.

  - 클라우드 컴퓨팅 - Go는 대부분의 클라우드 서비스들에서 잘 동작하고 있습니다.
    - [아마존 웹서비스(AWS)](https://github.com/aws/aws-sdk-go)
    - [에저 (Azure)](https://github.com/Azure/azure-sdk-for-go)
    - [디지털 오션 (Digital Ocean)](https://github.com/digitalocean/godo)
    - [GE Predix](https://github.com/geaviation/goboot-starter)
    - [구글 클라우드 플랫폼 (GCP)](https://cloud.google.com/go)
    - [히로쿠 (Heroku)](https://github.com/heroku/heroku-buildpack-go)
    - [IBM Bluemix](https://developer.ibm.com/bluemix/2015/10/28/getting-started-with-golang-on-bluemix/)
    - [오픈스택 (OpenStac)k](https://github.com/openstack/golang-client)
    - [Vscale](https://github.com/vscale/go-vscale)
    - [추가적인 클라우드 제공사](ProviderIntegration)를 살펴보세요.
  - [지속적인 통합(CI)과 지속적인 배포(CD)](HostedContinuousIntegration) - Go 대부분의 CI/CD 프레임워크를 잘 지원하고 있습니다.
  - 모니터링/로깅
    - [DeferPanic](http://deferpanic.com) - 전용 어플리케이션 성능 모니터링.
    - [OpsDash](https://www.opsdash.com/) - Go 기반 클러스터 모니터링 플랫폼.
  - 패키지 및 의존성 관리
    - [Gopkg.in](http://labix.org/gopkg.in)는 Niemeyer에서 제공하는 안정된 Go 라이브러리들의 소스입니다.
    - [Stable Lib](https://stablelib.com/)는 장기간 지원되는 안정된 Go 패키지를 제공하는 서비스입니다.

## Go를 이용한 프로덕션에서의 문제해결

  - [pprof 패키지](http://blog.golang.org/profiling-go-programs)를 이용하여 여러분의 Go 앱의 성능을 이해해봅시다.
  - 힙(Heap) 덤프
    - [heapdump13](heapdump13)
    - [heapdump14](heapdump14)
    - [heapdump15](https://github.com/golang/go/wiki/heapdump15)

## Go 프로젝트에 기여

  - [Go 기여 가이드](https://golang.org/doc/contribute.html)를 먼저 읽어주세요.
  - Go 프로젝트에 수정 의견을 제안하고자 하신다면, [Go 수정 제안](https://github.com/golang/proposal)을 읽어주세요.
    -  [문서 디자인](DesignDocuments)에 대한 가이드도 있습니다.
  - Go 릴리즈는 6개월 단위로 이뤄집니다. [여기서 더 자세한 정보를 살펴보세요](Go-Release-Cycle).
  -[Go 하위 리포지토리를 구성하는 방법](SubRepositories)이 무엇인지 알고싶으세요?
  - Go 프로젝트에 수정사항을 제출하기 전에는 모든 코드는 리뷰가 되어야 합니다.
    - [코드 리뷰 사례](CodeReview)를 살펴보세요.
    - 검토중인 코드에 코맨트를 남기고 싶다면, [이 가이드](CodeReviewComments)를 읽어주세요.
  - 이슈
    - 버그 리포팅이나 기능 요청은 [GitHub 이슈트래커(issue tracker)](https://github.com/golang/go/issues)를 이용합니다.
    - [이슈로 올라온 문제 처리](HandlingIssues)를 어떻게 하는지 궁금하세요?
  - 프로젝트 대시보드
    - [Go 빌드 대시보드](DashboardBuilders)
    - [퍼포먼스(Performance) 대시보드](PerfDashboard)

## 플랫폼 관련 정보

  - 현재 Go에서 요구하는 [플랫폼 최소요구사항](MinimumRequirements)을 살펴보세요.
  - Go를 새로운 플랫폼에 포팅하시기를 고려하시나요? [먼저 포팅 정책을 읽어봐주세요](PortingPolicy)
  - [모바일 기기](Mobile)
  - [우분투 (Ubuntu)](Ubuntu)
  - [윈도우즈 (Windows)](Windows)
    - [윈도우즈 빌드](WindowsBuild)
    - [윈도우즈 크로스 컴파일](WindowsCrossCompiling)
    - [윈도우즈 DLL](WindowsDLLs)
  - [GoArm](GoArm)
  - [크롬 OS](ChromeOS)
  - [다윈 (Darwin)](Darwin)
  - [ragonFly BSD](DragonFly-BSD)
  - [FreeBSD](FreeBSD)
  - [리눅스 (Linux)](Linux)
  - [NativeClient](NativeClient)
  - [NetBSD](NetBSD)
  - [OpenBSD](OpenBSD)
  - [Plan 9](Plan9)
  - [솔라리스 (Solaris)](Solaris)

## 릴리즈 관련 정보

  - [Go1point1Gotchas](Go1point1Gotchas)
  - [OlderVersions](OlderVersions)

안내:

- 이 문서는 [golang/go Wiki 문서](https://github.com/golang/go/wiki)를 번역하였습니다.