### Command Line Interface
+ Git, Github 사용시 필요
+ 파일,폴더,프로그램을 생성/수정/실행시키기 위해 사용함
+ 용어 
> directory : 폴더로 이해하면 편함
> root directory(/) : 최상위 폴더, **/** 로 표현함
> home directory(~) : CLI를 시작했을 때 처음 위치
> working directory : 현재 작업하고 있는 폴더
+ CLI(Command Line Interface) 사용법
    - Windows : Git bash 이용
    - Mac : Terminal 이용
+ 시작 화면 예시
~~~~
Du@Du_PC MINGW64 ~ (master)
$
~~~~
+ 명령어별 예시
    + pwd : print working directory
~~~~
Du@Du_PC MINGW64 ~ (master)
$ pwd
/c/Users/Du
~~~~
    + clear : CLI 화면에서 command를 지움
~~~~
Du@Du_PC MINGW64 ~ (master)
$ pwd
/c/Users/Du

Du@Du_PC MINGW64 ~ (master)
$ clear
~~~~
~~~~
Du@Du_PC MINGW64 ~ (master)
$
~~~~
    + ls : 현재 directiory에 포함된 file, folder 리스트업
        + ls -a : 숨겨진 file,folder까지..
        + ls -al : 숨겨진 file, folder의 detail 까지
    + cd : directory 변경
    ~~~~
    cd directory 주소
     >> 입력한 주소로 directory 변경
    cd
     >> home directory로 변경
    ~~~~
    + cd.. : 한단계 위 directory로 이동
    + mkdir : 현재 directory 하위에 directory 생성
    + touch : 현재 directory에 빈파일 생성
    + cp : 지정한 파일을 지정된 directory로 복사
    ~~~~
    cp test_file test_directory_path
     >> test_file을 test_directory_path로 복사
    ~~~~
    + cp -r : directory의 모든 파일을 지정된 directory로 복사
    ~~~~
    cp -r test_directory_path test2
     >> test_directory_path에 있는 모든 파일을 test2로 복사
    ~~~~
    + rm : 파일 완전 삭제 (삭제시 복구 불가)
    ~~~~
    rm test_file
     >> test_file 완전 삭제
    ~~~~
    + rm -r : 폴더 삭제 (삭제시 복구 불가)
    ~~~~
    rm r test2
     >> test2 directory 완전 삭제
    ~~~~
    + mv :
      
        1) file을 지정한 directory로 이동

        2) file명 바꾸기
    ~~~~
    mv test_file test_directory
     >> test_file을 test_directory로 이동
    mv test_file test_file2
     >> test_file 파일명을 test_file2로 변경
    ~~~~
    + echo : command 뒤에 입력한 내용 print
    ~~~~
    Du@Du_PC MINGW64 ~ (master)
    $ echo HelloWorld
    HelloWorld
    ~~~~
    + date : 현재 날짜 print
    ~~~~
    Du@Du_PC MINGW64 ~ (master)
    $ date
    2018년 06월 16일 토 오후 10:07:42
    ~~~~
    + exit : Git bash 끝내기

### Introduction to Git
+ Git??
    + 강력한 Version Control 시스템 (로컬)
    + 오픈소스
    + CLI 사용
    + 프로젝트를 콜라보레이션 할 때 특히 유용함
+ Download Git
+ install Git
+ install Git bash
+ Configure Username and Email
~~~~
Du@Du_PC MINGW64 ~ (master)
$ git config --global user.name "Duhyun"

Du@Du_PC MINGW64 ~ (master)
$ git config --global user.email "wisky006@gmail.com"
~~~~
~~~~
Du@Du_PC MINGW64 ~ (master)
$ git config --list
 >>> 설정 확인 필요시
~~~~

### Introduction to GitHub
+ GitHub??
    + 웹기반 호스팅 서비스
    + Git을 이용한 소프트웨어 개발 프로젝트에 사용함
    + push / pull을 이용해서 로컬 작업을 서버에 올리고 내릴 수 있음
    + 로컬 작업에 대한 **백업 기능** 제공
    + 다른 사람과 프로젝트를 **공유**할 수 있음
 
 
### Creating a Github Repository
+ GitHub 들어가서 만들면 됩니당...

### Basic Git Commands
+ $git init
+ $git add test.md
+ $git commit -m "second commit test"
+ $git remote rm origin 
+ $git remote add origin https://github.com/username/aaa.git
+ $git push -u origin master
    + $git checkout -b branchname
    + $git branch
    + $git checkout branchname
### Basic Markdown
- Heading(제목) : ###, ##, # 등 (총 여섯개)

~~~~
    #이 적을 수록 크기가 커진다
~~~~

- Unordered List : * 또는 -, +
~~~~
* 내용
- 내용
+ 내용
~~~~
- Italic : *텍스트*
~~~~
*텍스트*
~~~~
- Bold : **텍스트**
~~~~
**텍스트**
~~~~
- 인용 : >
> 이게 인용
- 코드 블럭 : ~~~~
- 수평선
-----
~~~~
----
~~~~
- 링크
  
[링크명](https://www.naver.com)
~~~~
[링크명](링크주소)
~~~~
- 참조 링크
  
[링크명][참조명]
[참조명]:https://www.naver.com
~~~~
[링크명][참조명]
[참조명]:링크주소
~~~~
- 이미지 링크
~~~~
~[링크명](이미지링크)
~~~~
### Installing R Packages
### Installing Rtools