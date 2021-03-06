## 강의노트
[![강의노트 바로가기](https://upload.wikimedia.org/wikipedia/commons/4/4a/Aviso_%22categor%C3%ADzame%22_%28espa%C3%B1ol%29.svg)](https://github.com/kyagrd/compiler2018Fall/wiki)

## 교수 연락처 및 공용 메신저
* 안기영 kya@hnu.kr
* [잔디 업무용 메신저](https://compiler.jandi.com/)

## 평가
과제 25%, 중간 30%, 기말 45%

## 수업에 사용할 책

* [Compiler Design: Virtual Machines](https://www.amazon.com/Compiler-Design-Machines-Reinhard-Wilhelm/dp/3642149081)

     이 과목의 주교재로 전체적인 수업 내용은 이 책의 내용을 가능한 한 다 다루는 것이다.
     전체적으로 3부분으로 되어 있는데 수업 진행 상황을 보아가며 하나는 제외하고 두 파트만 할 선별해서 수업 내용이 구성될 수도 있다.
     원서이지만 책이 얇아서 영어를 읽는 데 아주 큰 부담은 되지 않을 것이다.
     하지만 얇다고 해서 다루고 있는 내용 자체가 적은 것은 아니며 매우 압축되어 간결하게 설명하는 책이므로 열심히 공부하자.
     이 책을 사놓은 지가 좀 되었는데 아직 제대로 공부하지 못해서 여러분과 함께 이번 학기에 정말 제대로 같이 공부해 보고자 한다.

* [새로 보는 프로그래밍 언어](http://www.acornpub.co.kr/book/programming-language)
 
     이 책은 Programming Language Pragmatics, 2nd edition의 번역본인데
     이후로 원서 개정판이 나와 원서 최신판은
     [Programming Language Pragmatics, 3rd edition](https://www.elsevier.com/books/programming-language-pragmatics/scott/978-0-12-374514-9)이다.
     이 책은 비교적 최신의 프로그래밍 언어 관련 지식을 폭넓지만 이론과도 연계하여 소개하고 있어 프로그래밍 언어들의 특징과 차이점 및 공통점을 파악하기 좋게 되어 있어서 3학년 프로그래밍언어 과목 교재로도 활용하는 책이다. 사실 이 수업의 선수과목에 해당하는 과목이 프로그밍언어 과목인데 안타깝게도 우리 학교에서 최근 몇년 개강되지 않아 선수과목에 해당하는 배경지식이 부족할 수 있으므로 수업 진행 중에 이 책을 전반적으로 틈틈이 스스로 읽어보는 것이 좋다.
     물론 수업에서도 이 책 내용의 일부 특히 *2장 프로그래밍 언어 구문* 부분과 관련된 내용을 학기 초반에 다룰 것이다.
     
 * [Programming in Haskell, 2nd edition](http://www.cs.nott.ac.uk/~pszgmh/pih.html)
 
     수업 프로그래밍 과제 등에 이용할 언어로 구성된 프로그래밍 교재이다. 정말 잘 쓰여진 책이며 두 파트로 나눠져 있는데 첫 파트는 처음 프로그래밍을 배우는 사람들을 대상으로 (책을 지은 교수님이 재직하시는 영국의 대학교 컴퓨터과학과 1학년 학생 대상으로) 하고 있어 하스켈의 기능을 엄선된 예제와 함께 찾아보며 스스로 학습하기에 좋다.
     이 강의의 주목적은 하스켈에 능숙하게 되는 것이 아니기 때문에 강의에 필요한 최소한만 설명하고 넘어가게 될 것이므로 나머지 의문나는 부분을 스스로 찾아보며 공부할 수 있는 참고서로 사용할 목적으로 선정한 부교재이다.
     학구적이면서도 간결한 영어 문장으로 쓰여져 있어서 읽어보면 영어공부 특히 기술적/학문적 글쓰기를 할 때 어떻게 문단을 전개해야 하는지도 공부가 되어서 꼭 원서도 구비해서 참고하며 공부하면 좋다.
     이 책의 예제중에 몇가지를 그대로 혹은 약간 변형해서 수업에서도 일부 활용할 예정이다.

## 수업에 사용할 SW
 * [IHaskell](https://github.com/gibiansky/IHaskell) - [Haskell](http://haskell.org) 프로그래밍 언어를 지원하나는 [Jupyter](http://jupyter.org) 커널
   - Docker for Toolbox를 이용한 IHaskell 설치 방법 [안내 영상](https://youtu.be/rvaXWrN6tJY)
       - 참고로 더 최신 버전 소프트웨어로 구성된 도커 이미지가 만들어진 관계로
         영상에 화면에 나오는 명령어 대신 아래와 같은 명령어를 사용하도록 한다.
         ```
         docker run -it -v "`pwd`":/home/jovyan/ihaskell/notebooks -p 80:8888 kyagrd/ihaskell
         ```
         위 명령어를 실행하는 디렉토리는 `/c/Users` 의 하위 디렉토리여야만 한다. 도커가 도는 가상머신 공유폴더가 `/c/Users`로 되어 있기 때문.
         예를 들어 c드라이브 바로 밑에 디렉토리를 만들어 거기에서 위 명령어를 실행시키면 가상머신의 공유폴더 설정을 바꾸지 않는 한 주피터 서버에서 그 디렉토리에 접근하지 못한다.
   - 최신 버전의 Mac OS X 및 Windows 10 Professional 에서 메모리 8GB이상을 갖춘 환경에서는
     Docker for Toolbox 대신 더 최신 버전의 도커 소프트웨어인 Docker for Mac이나 Docker for Windows를 사용해도 된다.
   - Linux를 사용하는 경우라면 설치가 더 간단하다. 배포판 docker 패키지로 docker 소프트웨어 설치 후 명령어를 실행하면 된다. 
 * [잔디 업무용 메신저](https://compiler.jandi.com/)
