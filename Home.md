# 목차

+ [Go를 시작하며](#getting-started-with-go)
+ [Go로 작업하기](#working-with-go)
+ [Go에 대해 더 알아보기](#learning-more-about-go)
+ [Go 커뮤니티](#the-go-community)
+ [Go 툴체인](#using-the-go-toolchain)
+ [Go의 또 다른 위키들](#additional-go-programming-wikis)
+ [Go로 동작하는 서비스들](#online-services-that-work-with-go)
+ [Go를 이용한 프로덕션에서의 문제해결](#troubleshooting-go-programs-in-production)
+ [Go 프로젝트에 기여](#contributing-to-the-go-project)
+ [플랫폼 관련 정보](#platform-specific-information)
+ [릴리즈 관련 정보](#release-specific-information)

## Go를 시작하며

  - [Go 둘러보기](http://tour.golang.org) is the best place to start.
  - [이펙티브 Go](https://golang.org/doc/effective_go.html) will help you learn how to write idiomatic Go code.
  - [Go 스탠다드 라이브러리 문서](https://golang.org/pkg/) to familiarize yourself with the standard library.
  - [Go Playground](http://play.golang.org)를 이용하여 Go 프로그램을 웹에서 확인해보세요.
  - 여전히 모르겠나요? [Go 사용자들](GoUsers)과 그들의 [성공 사례](SuccessStories)를 확인해보세요. 또한 여러분이 왜 Go를 사용해야하는지 여러가지 이유들을 정리해봤습니다 [왜 Go를 사용해야 할까요?](whygo).
  - [다른언어에서 Go](https://github.com/golang/go/wiki/FromXToGo)로 전환한 회사들을 살펴보세요.

## Go로 작업하기

Ready to write some Go code of your own? Here are a few links to help you  get started.

  - Install and Setup your Environment
    - Start here: [Official Installation Documentation](https://golang.org/doc/install)
    -  If you prefer to install from source, [read this first](https://golang.org/doc/install/source).
      - [InstallFromSource](InstallFromSource) - Additional tips on source installs.
    - Windows user? [Install and configure Go, Git and Atom for Windows](https://github.com/abourget/getting-started-with-golang)
    - Mac user? [How I start - Go](https://howistart.org/posts/go/1) - A step-by-step guide to installing Go and building your first web service.
    - Having installation problems? [InstallTroubleShooting](InstallTroubleShooting)
    - Make sure you have your [$GOPATH environment variable set correctly](https://golang.org/doc/install/source#gopath)
      - If you need additional tips on using [$GOPATH, go here](GOPATH).
    - [MultipleGoRoots](MultipleGoRoots) - More advanced information on working with multiple go installations and the `$GOROOT` variable.
  - [Go IDEs and Editors](IDEsAndTextEditorPlugins) - Information on how to use your favorite editor with Go.
  - [Tools for working with Go code](CodeTools) - Formatting, linting, vetting, refactoring, navigation and visualization.
  - Finding Go Libraries and Packages
    - Start here: [Go open source projects](Projects).
    - Search for Go packages: [godoc.org](http://godoc.org)
    - Visualization of the [Go open source package graph](https://anvaka.github.io/pm/#/galaxy/gosearch?l=1)
  - [Managing your dependencies](PackageManagementTools) - An overview of the tools you can use to manage third-party packages (vendoring).
  - Publishing Go Packages as Open Source
    - Getting ready to publish your package? [Start here.](PackagePublishing)
    - [The Go Checklist](https://github.com/matttproud/gochecklist) - A comprehensive guide for publishing a project.
    - [How to layout your GitHub repo](GitHubCodeLayout) to make it easy to for other Go programmers to use with the `go get` command.
    - [Go Package, Go](https://johnsto.co.uk/blog/go-package-go) - A few recommendations for making Go packages easy to use.

## Learning more about Go

Once you have an overview of the language, here are resources you can use to learn more.

  - [Learning Go](Learn) - A collection of resources for learning Go - beginner to advanced.
    - [Best Practices for a New Go Developer](https://medium.com/@IndianGuru/best-practices-for-a-new-go-developer-8660384302fc) - Insights from Go community members.
    - [Server programming](LearnServerProgramming) - Building web, mobile, and API servers.
    - [More on concurrency](LearnConcurrency)
    - [More on error handling](LearnErrorHandling)
    - [More on testing](LearnTesting)
    - [More on mobile - Android and iOS](Mobile)
  - [Books](Books) - A list of Go books that have been published (ebook, paper)
  - [Blogs](Blogs) - Blogs about Go
    - [Podcasts](Podcasts) - Podcasts and episodes featuring Go
  - Videos, Talks and Presentations
    - [GopherVids](http://gophervids.appspot.com/) is a searchable index of videos about Go.
    - [GoTalks](GoTalks) - A collection of talks from Go conferences and meetups.
    - [Screencasts](Screencasts)
  - [Articles](Articles) - A collection of articles to help you learn more about Go.
  - [Training](Training) - Free and commercial, online and classroom training for Go.
  - [University Courses](Courses) - A list of CS programs and classes using Go.    
  - [Resources for non-English speakers](NonEnglish)

## The Go Community

Here are some of the places where you can find Gophers online. To get a sense of what it means to be a member of the Go community, read [Damian Gryski's keynote from the GolankUK 2015 conference](https://medium.com/@dgryski/the-go-community-f0d00e3a19e) or watch [Andrew Gerrand's closing keynote from GopherCon 2015](https://www.youtube.com/watch?v=0ht89TxZZnk).


- Where Gophers hangout online:
  - [The Go Forum](https://forum.golangbridge.org/) - An all-purpose discussion forum for the Go community.
  - [Gophers Slack Channel](http://gophers.slack.com/) - For real-time chat ([request membership](http://blog.gopheracademy.com/gophers-slack-community/)).
  - [Golang News](http://golangnews.com) - For curated links about Go Programming.
  - There is also a [/r/golang](http://reddit.com/r/golang) sub-reddit.
  - On Twitter, follow the [@golang](https://twitter.com/golang) account and keep tabs on the [#golang](https://twitter.com/search?q=%23golang&src=typd) hashtag.
  - We've also got a landing page on [Stack Overflow](http://stackoverflow.com/tags/go) for Go Q&A.
  - Matrix enthusiasts are invited to join [#Go:matrix.org](https://riot.im/app/#/room/#Go:matrix.org).
  - Discord users are welcome at the [Discord Gophers](https://discord.gg/VF92f7M) server. 
- Mailing Lists
  - The mailing list for Go users is [golang-nuts](https://groups.google.com/forum/#!forum/golang-nuts) - very high traffic.
    - Before you post, [check to see if it's already been answered](http://stackoverflow.com/tags/go), then read [these tips on how to ask a good question](HowToAsk)
  - For discussions about the core Go open source project, join [golang-dev](https://groups.google.com/forum/#!forum/golang-dev).
  - To get just our release announcements, join [golang-announce](https://groups.google.com/forum/#!forum/golang-announce)
- User Groups & Meetups - There are [Go Meetups in many cities](http://www.meetup.com/find/?allMeetups=false&keywords=golang&radius=Infinity&userFreeform=Sunnyvale%2C+CA&mcId=z94086&mcName=Sunnyvale%2C+CA&sort=recommended&eventFilter=mysugg)
    - [GoBridge](http://golangbridge.org) - Volunteers helping underrepresented communities to teach technical skills and to foster diversity in Go.
    - [Women Who Go](http://www.womenwhogo.org/)
    - See here for [additional information GoUserGroups](GoUserGroups)
- [Conferences](Conferences) - A list of upcoming and past Go conferences and major events.
- [Companies using Go](GoUsers) - A comprehensive list of companies using Go throughout the world.
- Learn more about the [Go Gopher images](Gopher) by Renee French.

## Using the go toolchain

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
    
## Additional Go Programming Wikis

  - [Why Go doesn't Support Generics: A Summary of Go Generics Discussions](https://docs.google.com/document/d/1vrAy9gMpMoS3uaVphB32uVXX4pi-HnNjkMEgyAHX4N4/preview) - Start here before you join the debate.
  - Concurrency
    - [Timeouts](Timeouts) - Abandon async calls that take too long
    - [LockOSThread](LockOSThread)
    - [MutexOrChannel](MutexOrChannel) - When to use one vs the other
    - [RaceDetector](RaceDetector) - How to detect and fix race conditions
  - Working with Databases
    - [database/sql](http://go-database-sql.org/) - Online tutorial for working with the database/sql package.
    - [TUGTBDDAwG](https://vividcortex.com/resources/building-database-driven-apps-with-go/) - Guide to building data driven apps.
    - [SQLDrivers](SQLDrivers)
    - [SQLInterface](SQLInterface)
  - From other languages
    - [Go for Java Programmers](http://yourbasic.org/golang/go-java-tutorial/)
    - [Go for C++ Programmers](GoForCPPProgrammers)
  - Strings
    - [GoStrings](GoStrings)
    - [String Matching](http://blog.gopheracademy.com/advent-2014/string-matching/)
  - [Comments](Comments)
  - [CommonMistakes](CommonMistakes)
  - [Errors](Errors)
  - [GcToolchainTricks](GcToolchainTricks)
  - [Hashing](Hashing)
  - [HttpFetch](HttpFetch)
  - [HttpStaticFiles](HttpStaticFiles)
  - [InterfaceSlice](InterfaceSlice)
  - [Iota](Iota)
  - [MethodSets](MethodSets)
  - [PanicAndRecover](PanicAndRecover)
  - [Range](Range)
  - [RateLimiting](RateLimiting)
  - [Rationales](Rationales)
  - [SendingMail](SendingMail)
  - [SignalHandling](SignalHandling)
  - [SimultaneousAssignment](SimultaneousAssignment)
  - [SliceTricks](SliceTricks)
  - [Switch](Switch)
  - [TableDrivenTests](TableDrivenTests)


## Online Services that work with Go

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

## Troubleshooting Go Programs in Production

  - Understand the performance of your Go apps using the [pprof package](http://blog.golang.org/profiling-go-programs)
  - Heap Dumps
    - [heapdump13](heapdump13)
    - [heapdump14](heapdump14)
    - [heapdump15](https://github.com/golang/go/wiki/heapdump15)

## Contributing to the Go Project

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

## Platform Specific Information

  - See [MinimumRequirements](MinimumRequirements) for minimum platform requirements of current Go ports.
  - Considering porting Go to a new platform? [Read our porting policy first](PortingPolicy)
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

## Release Specific Information

  - [Go1point1Gotchas](Go1point1Gotchas)
  - [OlderVersions](OlderVersions)

안내:

- 이 문서는 [golang/go Wiki 문서](https://github.com/golang/go/wiki)를 번역하였습니다.