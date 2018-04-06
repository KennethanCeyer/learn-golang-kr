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
    - 해당 메뉴를 이용하세요: [공식 설치문서](https://golang.org/doc/install)
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
  - [The Go Forum](https://forum.golangbridge.org/) - 여러 주제에 대해 다루는 Go 커뮤니티.
  - [Gophers Slack Channel](http://gophers.slack.com/) - 실시간 대화가 가능한 Go 커뮤니티 ([슬랙 가입요청은 이곳에](http://blog.gopheracademy.com/gophers-slack-community/)).
  - [Golang News](http://golangnews.com) - Go 프로그래밍에 대한 알림을 원하실 때 이용하세요.
  - [/r/golang](http://reddit.com/r/golang) Go에 대해 다루는 레딧 커뮤니티.
  - 트위터를 사용하신다면, [@golang](https://twitter.com/golang) 계정을 팔로우하시고 [#golang](https://twitter.com/search?q=%23golang&src=typd) 해시태그를 주시해주세요.
  - [Stack Overflow](http://stackoverflow.com/tags/go)에서 Go 관련 Q&A가 활발히 이루어지고 있습니다.
  - 매트릭스(Matrix) 사용자분들은 [#Go:matrix.org](https://riot.im/app/#/room/#Go:matrix.org)를 이용해주세요.
  - [Discord Gophers](https://discord.gg/VF92f7M)에서 디스코드(Discord)를 이용하시는 유저들을 환영합니다. 
- 메일링 리스트
  - Go 사용자들을 위한 메일링 리스트입니다 [golang-nuts](https://groups.google.com/forum/#!forum/golang-nuts) - 엄청 활발합니다!
    - 스택오버플로에 질문을 남기기전에, [이미 있는 질문은 아닌가요?](http://stackoverflow.com/tags/go)를 읽어주세요, 읽고나서 [어떤 질문이 좋은 질문일까요](HowToAsk)도 읽어주세요
  - 핵심 Go 오픈소스 프로젝트에 대한 토론을 원하시면 [golang-dev](https://groups.google.com/forum/#!forum/golang-dev)를 이용해주세요.
  - Go 릴리즈 정보를 얻을려면, [golang-announce](https://groups.google.com/forum/#!forum/golang-announce)에 참여하세요.
- 사용자 그룹 & 밋업 - [많은 도시에 밋업이 열리고 있습니다](http://www.meetup.com/find/?allMeetups=false&keywords=golang&radius=Infinity&userFreeform=Sunnyvale%2C+CA&mcId=z94086&mcName=Sunnyvale%2C+CA&sort=recommended&eventFilter=mysugg)
    - [GoBridge](http://golangbridge.org) - Go와 관련하여 소수 커뮤니티에게 전문 기술을 가르치고 다양성을 육성하는 자원봉사 단체입니다.
    - [Women Who Go](http://www.womenwhogo.org/)
    - [Go 사용자 그룹과 관련한 더 많은 정보는 이곳에서 살펴보세요.](GoUserGroups)
- [컨퍼런스](Conferences) - A list of upcoming and past Go conferences and major events.
- [Go를 사용하는 업체](GoUsers) - A comprehensive list of companies using Go throughout the world.
- [Go Gopher images](Gopher)에 대해 더 많이 알아보세요 출처: by Renee French.

## Go 툴체인

  - Start with the standard documentation for the `go` command [available here](https://golang.org/cmd/go/)
  - Start here for to learn about [vendoring](https://golang.org/cmd/go/#hdr-Vendor_Directories).
  - See also [PackageManagementTools](PackageManagementTools) for package management tools.
  - [Cross Compilation](https://rakyll.org/cross-compilation/)
  - Shared libraries and Go (buildmode)
    - [Go Shared Libraries](https://github.com/jbuberel/buildmodeshared) - Examples for creating and using shared libraries from Go and Python.
    - [Sharing Go Packages with C](http://blog.ralch.com/tutorial/golang-sharing-libraries/) - by [@ralch](https://twitter.com/ralch).
    - [Calling Go libraries from Python](https://blog.filippo.io/building-python-modules-with-go-1-5/) - by Filippo Valsorda
    - [Calling Go libraries from Ruby](http://c7.se/go-and-ruby-ffi/) - by Peter Hellberg
    - [Calling Go libraries from Swift](https://rakyll.org/swift/) - by Jaana Burcu Dogan
    - [Build a Ruby Gem with a Go native extension](http://blog.paracode.com/2015/08/28/ruby-and-go-sitting-in-a-tree) - by @jondot
    - [gohttplib](https://github.com/shazow/gohttplib) - An experiment in using Go 1.5 buildmode=c-shared.
  - See the wikis below for additional details:
    - [GoGetTools](GoGetTools)
    - [GoGetProxyConfig](GoGetProxyConfig)
    - [cgo](cgo)
    - [CompilerOptimizations](CompilerOptimizations)
    - [GccgoCrossCompilation](GccgoCrossCompilation)
    - [GcToolchainTricks](GcToolchainTricks)
    - [GoGenerateTools](GoGenerateTools)
    - [Go Tooling Essentials](https://rakyll.org/go-tool-flags/) - by Jaana Burcu Dogan
    
## Go의 또 다른 위키들

  - [Go가 제너릭을 지원하지 않는 이유: 제너릭 의견 요약](https://docs.google.com/document/d/1vrAy9gMpMoS3uaVphB32uVXX4pi-HnNjkMEgyAHX4N4/preview) - Start here before you join the debate.
  - 동시성 제어
    - [Timeouts](https://github.com/golang/go/wiki/Timeouts) - Abandon async calls that take too long
    - [LockOSThread](https://github.com/golang/go/wiki/LockOSThread)
    - [MutexOrChannel](https://github.com/golang/go/wiki/MutexOrChannel) - When to use one vs the other
    - [RaceDetector](https://github.com/golang/go/wiki/RaceDetector) - How to detect and fix race conditions
  - 데이터베이스 사용하기
    - [database/sql](http://go-database-sql.org/) - Online tutorial for working with the database/sql package.
    - [TUGTBDDAwG](https://vividcortex.com/resources/building-database-driven-apps-with-go/) - Guide to building data driven apps.
    - [SQLDrivers](https://github.com/golang/go/wiki/SQLDrivers)
    - [SQLInterface](https://github.com/golang/go/wiki/SQLInterface)
  - 다른 언어 개발자를 위한
    - [Go for Java Programmers](http://yourbasic.org/golang/go-java-tutorial/)
    - [Go for C++ Programmers](https://github.com/golang/go/wiki/GoForCPPProgrammers)
  - 문자열
    - [GoStrings](https://github.com/golang/go/wiki/GoStrings)
    - [String Matching](http://blog.gopheracademy.com/advent-2014/string-matching/)
  - [Comments](https://github.com/golang/go/wiki/Comments)
  - [CommonMistakes](http://blog.gopheracademy.com/advent-2014/string-matching/)
  - [Errors](https://github.com/golang/go/wiki/Errors)
  - [GcToolchainTricks](https://github.com/golang/go/wiki/GcToolchainTricks)
  - [Hashing](https://github.com/golang/go/wiki/Hashing)
  - [HttpFetch](https://github.com/golang/go/wiki/HttpFetch)
  - [HttpStaticFiles](https://github.com/golang/go/wiki/HttpStaticFiles)
  - [InterfaceSlice](https://github.com/golang/go/wiki/InterfaceSlice)
  - [Iota](https://github.com/golang/go/wiki/Iota)
  - [MethodSets](https://github.com/golang/go/wiki/MethodSets)
  - [PanicAndRecover](https://github.com/golang/go/wiki/PanicAndRecover)
  - [Range](https://github.com/golang/go/wiki/Range)
  - [RateLimiting](https://github.com/golang/go/wiki/RateLimiting)
  - [Rationales](https://github.com/golang/go/wiki/Rationales)
  - [SendingMail](https://github.com/golang/go/wiki/SendingMail)
  - [SignalHandling](https://github.com/golang/go/wiki/SignalHandling)
  - [SimultaneousAssignment](https://github.com/golang/go/wiki/SimultaneousAssignment)
  - [SliceTricks](https://github.com/golang/go/wiki/SliceTricks)
  - [Switch](https://github.com/golang/go/wiki/Switch)
  - [TableDrivenTests](https://github.com/golang/go/wiki/TableDrivenTests)


## Go로 동작하는 서비스들

If you're looking for services that support Go, here's a list to get you started.

  - Cloud Computing - Go is well supported on most cloud service providers.
    - [Amazon Web Services](https://github.com/aws/aws-sdk-go)
    - [Azure](https://github.com/Azure/azure-sdk-for-go)
    - [Digital Ocean](https://github.com/digitalocean/godo)
    - [GE Predix](https://github.com/geaviation/goboot-starter)
    - [Google Cloud Platform for Go](https://cloud.google.com/go)
    - [Heroku](https://github.com/heroku/heroku-buildpack-go)
    - [IBM Bluemix](https://developer.ibm.com/bluemix/2015/10/28/getting-started-with-golang-on-bluemix/)
    - [OpenStack](https://github.com/openstack/golang-client)
    - [Vscale](https://github.com/vscale/go-vscale)
    - See here for [information on additional providers](ProviderIntegration)
  - [Continuous Integration and Continuous Deployment](HostedContinuousIntegration) - Go is well supported by most CI/CD frameworks
  - Monitoring/Logging
    - [DeferPanic](http://deferpanic.com) - Dedicated Go application performance monitoring.
    - [OpsDash](https://www.opsdash.com/) - Go-based cluster monitoring platform.
  - Package and Dependency Management
    - [Gopkg.in](http://labix.org/gopkg.in) is a source for stable Go libraries, provided by Gustavo Niemeyer.
    - [Stable Lib](https://stablelib.com/) is a service that provides stable Go packages with long-term support.

## Go를 이용한 프로덕션에서의 문제해결

  - Understand the performance of your Go apps using the [pprof package](http://blog.golang.org/profiling-go-programs)
  - Heap Dumps
    - [heapdump13](heapdump13)
    - [heapdump14](heapdump14)
    - [heapdump15](https://github.com/golang/go/wiki/heapdump15)

## Go 프로젝트에 기여

  - Start by reading the [Go Contribution Guidelines](https://golang.org/doc/contribute.html)
  - If you'd like to propose a change to the Go project, start by reading the [Go Change Proposal Process](https://github.com/golang/proposal)
    -  An archive of [design documents is also available](DesignDocuments)
  - Go releases happen on ~6 month intervals. [See here for more information](Go-Release-Cycle)
  - Want to know more about how the [Go source sub-repositories are structured?](SubRepositories)
  - The Go project requires that all code be reviewed before it is submitted.
    - Read more about our [code review practices](CodeReview)
    - If you're commenting on code under review, please read [these guidelines](CodeReviewComments)
  - Issues
    - Bug reports and feature requests should be filed using the [GitHub issue tracker](https://github.com/golang/go/issues)
    - Want to understand how we [handle issues that are reported?](HandlingIssues)
  - Project Dashboards
    - [Go Builds Dashboard info](DashboardBuilders)
    - [Performance Dashboard info](PerfDashboard)

## 플랫폼 관련 정보

  - 현재 Go에서 요구하는 [플랫폼 최소요구사항](MinimumRequirements)을 살펴보세요.
  - Go를 새로운 플랫폼에 포팅하시기를 고려하시나요? [먼저 포팅 정책을 읽어봐주세요](PortingPolicy)
  - [Mobile](Mobile)
  - [Ubuntu](Ubuntu)
  - [Windows](Windows)
    - [WindowsBuild](WindowsBuild)
    - [WindowsCrossCompiling](WindowsCrossCompiling)
    - [WindowsDLLs](WindowsDLLs)
  - [GoArm](GoArm)
  - [ChromeOS](ChromeOS)
  - [Darwin](Darwin)
  - [DragonFly BSD](DragonFly-BSD)
  - [FreeBSD](FreeBSD)
  - [Linux](Linux)
  - [NativeClient](NativeClient)
  - [NetBSD](NetBSD)
  - [OpenBSD](OpenBSD)
  - [Plan 9](Plan9)
  - [Solaris](Solaris)

## 릴리즈 관련 정보

  - [Go1point1Gotchas](Go1point1Gotchas)
  - [OlderVersions](OlderVersions)

안내:

- 이 문서는 [golang/go Wiki 문서](https://github.com/golang/go/wiki)를 번역하였습니다.