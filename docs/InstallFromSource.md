# 소개

이 페이지는 http://golang.org/doc/install/source를 기준으로 다양한 운영체제에 대한 추가 지침사항을 제공하고 있습니다.

## C 도구 설치

OS X 에서, [Xcode](http://developer.apple.com/Xcode/) 커맨드라인 도구로 C 컴파일러가 번들로 제공됩니다.
Go를 컴파일하기 위해 전체 Xcode를 설치할 필요가 없습니다.
이미 Xcode 4.3 이상을 설치했다면 다운로드 환경 설정 패널의 구성 요소 탭에서
커맨드 라인 도구를 설치할 수 있습니다.
최신 버전의 Xcode에서는 Xcode를 열지 않고도
`xcode-select --install ` 명령으로 커맨드 라인 도구를 설치 할 수 있습니다.
컴파일러가 작동되는지 확인하려면, 새로 생성된 터미널 창에서 그냥 `gcc`를 실행하세요
`"gcc: command not found"` 에러가 보이지 않는 이상 여러분의 go는 준비가 된 것입니다.

우분투(Ubuntu) 데비안(Debian) 에서는, `sudo apt-get install gcc libc6-dev`를 이용하세요.
62비트 환경에서 32비트 바이너리 빌드를 원하시면 `libc6-dev-i386` 패키지가 필요합니다.

레드햇(RedHat) Centos 6에서는, `sudo yum install gcc glibc-devel`를 이용하세요.
62비트 환경에서 32비트 바이너리 빌드를 원하시면
`glibc-devel.i386`와 `glibc-devel.x86_64` 패키지가 필요합니다.

윈도우즈(Windows) 에서는, [TDM-GCC](http://tdm-gcc.tdragon.net/)를 이용해 `gcc`를 설치해주세요.
(설치한 프로그램의 `bin` 서브디렉토리를 `PATH` 변수로 잡았는지 확인해주세요.)
Go는 현재 시그윈(Cygwin) 툴체인을 지원하지 않습니다.
