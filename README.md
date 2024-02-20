

시스템 환경 변수:

HOME: 사용자의 홈 디렉토리
LANG: 사용자의 로케일 설정 (e.g. "ko_KR.UTF-8")
TERM: 사용자 터미널 유형
USER: 현재 로그인한 사용자 
SHELL: 현재 사용하는 셸
PATH: 외부 명령어를 검색하는 경로 목록
PWD: 현재 작업 디렉토리 경로
OLDPWD: 이전 작업 디렉토리 경로
EDITOR: 기본 텍스트 편집기
HISTSIZE: 명령어 히스토리 크기
MAIL: 메일 스풀 파일 경로
PS1: 프롬프트 문자열
PS2: 두 번째 프롬프트 문자열(멀티라인 명령어를 사용할 때 출력하는)
HISTFILE: 명령어 히스토리 파일

단축키 
Shift + PgUp: 지나간 이전 화면을 보여준다.
Shift + PgDn: 지나간 이후 화면을 보여준다.
Ctrl + L : 화면 지우기 (clear)

시스템에 직접 로그인하는 방법: 로컬에서 콘솔을 이용해서 로그인
시스템에 간접 로그인하는 방법: 원격에서 터미널을 이용해서 로그인 
- putty.exe, ssh.exe

CentOS 7을 설치하고 부팅이 되면 6개의 가상 콘솔이 열려있다.
각 가상콘솔을 이동하는 단축키 형식: Alt + 펑션키(F1  ~ F6)
Alt + F1: 첫 번째 가상콘솔  /dev/tty1
Alt + F2: 두 번째 가상콘솔  /dev/tty2
Alt + F3: 세 번째 가상콘솔  /dev/tty3
Alt + F4: 네 번째 가상콘솔  /dev/tty4
Alt + F5: 다섯 번째 가상콘솔  /dev/tty5
Alt + F6: 여섯 번째 가상콘솔  /dev/tty6

명령행 편집 기능
bash에서 지원되는 명령행 편집 기능입니다. 
저도 자주 사용하는 기능인데 잘 활용하면 명령어를 빠르게 사용할 수 있는 장점이 있습니다.
단축키 설명
Ctrl + a 명령행의 처음으로 이동
Ctrl + e 명령행의 끝으로 이동
Ctrl + w 명령행 왼쪽 단어 삭제
Ctrl + u 명령행 전체 삭제
Ctrl + k 명령행 오른쪽 전체 삭제
Ctrl + r 명령행 히스토리 검색
Ctrl + d 한 글자 삭제


명령어의 종류
  . alias 명령어
    - 메모리에 저장되어 있다.
  . 내부 명령어
    - 셸 내부에 저장되어 있다.
    - /bin/bash
  . 외부 명령어
    - 실행 디렉터리에 저장되어 있다.
    - /bin, /usr/bin, /sbin, /usr/sbin

명령어 우선순위 
  . alias 명령어(메모리) > 내부 명령어(/bin/bash) > 외부 명령어(/bin, /usr/bin, /sbin, /usr/sbin)


파일 및 디렉토리 명령어
  . help: 내부 명령어에 대한 도움말을 확인하는 명령어
  . man: 외부 명령어에 대한 도움말을 확인하는 명령어
  . pwd: 현재 작업 디렉토리의 경로를 표시하는 명령어
  . tree: 디렉터리를 tree 형식으로 출력하는 명령어
  . cd: 작업 디렉토리를 변경하는 명령어
  . ls: 디렉토리의 파일을 확인하는 명령어
  . mkdir: 디렉터리를 생성하는 명령어
  . rmdir: 디렉터리를 삭제하는 명령어
  . rm: 파일을 삭제하는 명령어
  . cp: 파일을 복사하는 명령어
  . mv: 파일의 이동, 파일의 이름을 변경하는 명령어
  . ln: 심볼릭 링크나 하드 링크를 생성하는 명령어
  . echo: 메시지와 변수의 저장된 값을 출력하는 명령어
  . stat: 파일 또는 파일 시스템 상태를 표시하는 명령어
  . cat: 파일의 내용을 출력하는 명령어
  . less/more: 파일의 내용을 출력하는 명령어 (페이지 단위)
  . head: 파일의 처음 부분을 출력하는 명령어
  . tail: 파일의 끝부분을 출력하는 명령어
  . touch: 빈 파일을 생성하거나 파일의 최근 수정 시간을 변경하는 명령어
  . grep: 파일에서 특정 패턴을 검색하는 명령어
  . find: 파일을 검색하는 명령어
  . chmod: 파일의 허가권을 변경하는 명령어
  . chown: 파일의 소유권을 변경하는 명령어
  . chgrp: 파일의 그룹을 변경하는 명령어

패키지 관리
  . yum: RedHat 계열 배포판(RHEL7, CentOS7)에서 사용하는 패키지 관리 도구
  . dnf: edHat 계열 배포판(RHEL8,9 Rocky Linux8,9)에서 사용하는 패키지 관리 도구
  . apt-get: Debian 계열 배포판(Debian, Unbuntu)에서 사용하는 패키지 관리 도구
  . apt: Debian 계열 배포판(Debian, Unbuntu)에서 사용하는 패키지 관리 도구


텍스트 편집기
  . nano: 입문자용 편집기
  . vi: 시니어급 편집기
  . emacs: 리처드 스톨만 선생님께서 만든 편집기



명령어의 도움말
  . 외부 명령어 --help, man 외부 명령어 
    - e.g.) ls --help, man ls
  . help 내부 명령어, man 내부 명령어
    - e.g.) help cd, man cd

명령어 앞에 # 이 들어가면 주석으로 처리한다.
C, Java 프로그래밍에서  // 
Python 프로그래밍에서 #
셸에서는 #


단축키 
Shift + PgUp: 지나간 이전 화면을 보여준다.
Shift + PgDn: 지나간 이후 화면을 보여준다.

o 리눅스 디렉터리 구조

절대 경로: 최상위 디렉티리(/) 부터 시작하는 경로
상대 경로: 현재 디렉터리부터 시작하는 경로

/etc/hosts 일 경우
현재 디렉터리 위치: /root
절대 경로: /etc/hosts
상대 경로: ../etc/hosts

현재 디렉터리: .
상위 디렉터리: ..

yum: 패키지를 설치하는 명령어
사용법: yum 옵션 명령어 패키지명
-y: 옵션
install: 설치 명령어
tree: 패키지명

tree: 디렉터리를 tree 형식으로 출력하는 명령어
# yum -y install tree
# tree -L 1 /
/
├── bin -> usr/bin : 명령어 디렉터리
├── boot : 부팅 관련 디렉터리
├── dev  : 장치 디렉터리
├── etc  : 환경 설정 디렉터리
├── home : 일반 사용자의 홈디렉터리가 위치하는 디렉터리
├── lib -> usr/lib : 32bit 라이브러리 디렉터리
├── lib64 -> usr/lib64 : 64bit 라이브러리 디렉터리
├── media : USB/DVD/외장HDD 마운트 디렉터리
├── mnt : USB/DVD/외장HDD 마운트 디렉터리 
├── opt : 추가 SW 디렉터리
├── proc: 가상 파일시스템(메모리) 디렉터리
├── root : 관리자의 홈 디렉터리
├── run : 부팅 후에 프로세스의 런타임 테이터를 저장하는 디렉터리
├── sbin -> usr/sbin : 관리자용 명령어
├── srv : 사이트에서 생성되는 데이터를 저장하는 디렉터리
├── sys : 2.6 커널에서 사용되는 가상 파일 시스템 디렉터리
├── tmp : 임시 디렉터리
├── usr : 일반 애플리케이션이 위치하는 디렉터리
└── var : 시스템의 로그, 스풀링 같이 가변적으로 변경되는 데이터가 위치하는 디렉터리

19 directories, 0 files


# yum -y install mc

  . help: 내부 명령어에 대한 도움말을 확인하는 명령어

# help 
# help help
# help pwd
# help cd

pwd(Print Working Directory): 현재 디렉터리의 위치를 출력하는 명령어
내부 명령어, 외부 명령어가 동시에 있는 명령어
내부 명령어가 우선순위를 먼저 갖기 때문에 pwd를 실행하면 내부 명령어 pwd가 실행된다.
# pwd
/root

  . pwd: 현재 작업 디렉토리의 경로를 표시하는 명령어

  . tree: 디렉터리를 tree 형식으로 출력하는 명령어

  . cd: 작업 디렉토리를 변경하는 명령어

  . ls: 디렉토리의 파일을 확인하는 명령어
    기본 ls 는 .으로 시작하는 모든파일들을 출력하지 않는다.   
    ls -a 모든 파일 출력
    ls -la 모든파일을 자세히 출력
       -F 파일의 종류에 따라 문자가 붙는다.

    파일의 종류                    -F옵션시 보여지는 문자
    -: 일반파일이면서 실행파일       *
   d: 디렉터리                       /
   l: 심볼릭링크(바로가기)           @
   b: 블럭장치(하드디스크)
   c: 문자장치(터미널)
   p: 파이프                         |(shift+\)
   s: 소켓                            =
   ?: 권한이 없어 파일 형식을 알 수 없는 경우

  -i inode 번호(파일마다 가지고 있는 고유 번호)

  . mkdir: 디렉터리를 생성하는 명령어

    내부명령어 umask와 관련이 있다.
   #umask
   0022
- rw- r-- r-- 6 4 4
- rwx rwx rwx 7 7 7
- rw- rw- rw- 6 6 6
- r-x --x rw- 5 1 6
- r=4 w=2 x=1
- r=읽기 w=쓰기 x=실행
8진수
rw-
0 000
1 001
2 010
3 011
4 100
5 101
6 110
7 111
  dirA 디렉터리에 파일의 목록을 출력한다.
# ls -l dirA = #ll A
합계 0

  -d 검색대상이 디렉터리일 때 디렉터리 자체의 설정된 권한등... 자세히 출력한다.

# ls -ld dirA
drwxr-xr-x. 2 root root 6  2월 19 20:19 dirA

ls의 기본 옵션은 정렬해서 출력한다.(숫자,대문자,소문자 순서로 출력)

# ls -lr 거꾸로 정렬

-m : 허가권(퍼미션)을 직접 설정해서 디렉터리를 생성한다.  umask 의 설정된 값과 상관없이 디렉터리를 생성한다.
# mkdir -m 000 test1; ll -d test1
d---------. 2 root root 6  2월 19 20:31 test1

700의 권한으로 test2 디렉터리를 생성한다.
# mkdir -m 700 test2; ll -d test2
drwx------. 2 root root 6  2월 19 20:33 test2

현재 디렉터리에 test3 디렉터리 안에 test4 디렉터리를 생성한다.
test3 디렉터리가 현재 디렉터리에 존재하면 생성되고 없으면 에러가 발생한다.
# mkdir test3/test4
# mkdir test3/test4 테스트 3 하위에 4 디렉터리를 만든다.
-p 옵션 : 부모/자식 디렉터리를 동시에 생성하는 옵션. -p옵션은 뒷 쪽에써도 상관X
-v: 디렉터리 생성을 출력하는 옵션
# mkdir -v test4

SELinux: 보안강화 리눅스 옵션(보안과 관련된 기능을 제공하는 리눅스 커널안에 들어있음.)
# ls -dZ test4
drwxr-xr-x. root root unconfined_u:object_r:admin_home_t:s0 test4

  . rmdir: 디렉터리를 삭제하는 명령어

  . rm: 파일을 삭제하는 명령어

# rm -rfv(rf:하위에 파일이 있어도 묻지 않고 지우는데 v:옵션으로 내역을 보여줌) test1
removed directory: `test1/test3'
removed directory: `test1'

rm 명령어는 파일을 삭제하는데 옵션이 하나도 없으면 그냥 삭제한다.
그래서 위험하므로 우선순위가 빠른 alias 명령어로 rm 을 설정한 것이다.
rm 을 사용하면 rm -i 가 실행된다.
# alias rm
alias rm='rm -i'

# rm 0.txt
rm: remove 일반 빈 파일 `0.txt'?  <-- 엔터(삭제하지 않는다.), y(삭제한다.)
# \rm 0.txt  <-- rm 이 아니기 때문에 그냥 지운다. 

/bin/rm 0.txt, /usr/bin/rm 0.txt 동일하다.
=bin디렉터리 안에 있는 rm 명령어를 사용해서 0.txt를 지운다
(이 때 arias에 셋팅된 rm -i는 작동하지 않는다(명령어 이름이 달라서))

# rm -f * 디렉터리 안을 전부 지운다.

  . cp: 파일을 복사하는 명령어
 
  복사 /소스1 /소스2 /소스3 을 . 현재 디렉토리에
# cp /etc/hosts /etc/group /etc/passwd . 
cp: overwrite `./group'? y
cp: overwrite `./passwd'? y

etc/hosts 파일을 현재 디렉터리에 hosts1.txt 파일로 복사한다.
# cp /etc/hosts hosts1.txt
# cp /etc/hosts .
# alias cp
alias cp='cp -i'
# cp /etc/hosts /etc/group /etc/passwd .
cp: overwrite `./hosts'? y

# cp -f /etc/shadow group
cp: overwrite `group'?  <-- 엔터 (복사가 안된다.)

# \cp /etc/shadow group    <-- cp 가 아니기 때문에 그냥 복사한다. /bin/cp /etc/shadow group, /usr/bin/cp /etc/shadow group 동일하다.

# cp /etc/redhat-release  <-- 에러가 발생한다. 복사할 곳을 지정하지 않았기 때문이다.

/etc 디렉터리를 현재 디렉터리에 ETCBACKUP 으로 복사한다.
에러가 발생되는 것은 디렉터리를 복사할 때는 반드시 옵션을 주어야 한다.
# cp /etc ETCBACKUP  <-- 에러(옵션을 안줬기 때문에)

# cp -a /etc ETCBACKUP  <-- 정상적으로 복사


  . mv: 파일의 이동, 파일의 이름을 변경하는 명령어
2개의 기능이 있다. (이동, 이름 변경)
Usage: mv [OPTION]... [-T] SOURCE DEST
  or:  mv [OPTION]... SOURCE... DIRECTORY
  or:  mv [OPTION]... -t DIRECTORY SOURCE...
Rename SOURCE to DEST, or move SOURCE(s) to DIRECTORY.

# cat > a.txt 
^d  <-- Ctrl + D

a.txt 파일을 b.txt 파일로 이름을 변경한다.
# mv a.txt b.txt

# mkdir backup

현재 디렉터리에 있는 b.txt 파일을 backup 디렉터리에 이동한다.
# mv b.txt backup

/backup/b.txt 파일을 현재 디렉터리로 이동시킨다.
# mv backup/b.txt .

>>> 아래 명령어들과 모두 동일하다. <<<
mv backup/b.txt ./b.txt
mv backup/b.txt b.txt
mv backup/b.txt /root
mv backup/b.txt /root/b.txt
mv backup/b.txt $HOME
mv backup/b.txt $HOME/b.txt

# mkdir backup

현재 디렉터리에 있는 b.txt 파일을 backup 디렉터리에 이동한다.
# mv b.txt backup

  . ln: 심볼릭 링크나 하드 링크를 생성하는 명령어
  
Usage: ln [OPTION]... [-T] TARGET LINK_NAME   (1st form)
  or:  ln [OPTION]... TARGET                  (2nd form)
  or:  ln [OPTION]... TARGET... DIRECTORY     (3rd form)
  or:  ln [OPTION]... -t DIRECTORY TARGET...  (4th form)

lrwxrwxrwx. 1 root root  8  2월 20 21:13 hello2.py -> hello.py
심볼릭 링크의 권한과 크기는 의미가 없다 (원본의 권한과 크기를 따르기 때문에)

-s : 심볼릭 링크 파일을 생성하는 옵션
-s 옵션이 없으면 하드링크를 생성한다.

현재 디렉터리에 존재하는 hello.py 파일을 hello2.py 파일로 심볼릭 링크를 생성한다.
# mkdir dirA; ln -s dirA DIRA
# ls -l
합계 0
lrwxrwxrwx. 1 root root 4  2월 20 21:20 DIRA -> dirA
drwxr-xr-x. 2 root root 6  2월 20 21:19 dirA

# cd DIRA
# pwd -P
# pwd -L
# pwd
# cd -
심볼릭 링크는 파티션을 넘어갈 수 있다.
다시말해서 다른 파티션에 있는 파일을 심볼릭 링크로 생성할 수 없다.
참고로 하드링크는 파티션을 넘어갈 수 없다.

0byte 크기의 파일 /boot/a.txt 를 생성한다.
# touch /boot/a.txt


/boot/a.txt 파일을 /root/a.txt 파일로 심볼릭 링크 파일을 생성한다.
# ln -s /boot/a.txt   

>>> 아래 명령어는 모두 동일하다. <<<
# ln -s /boot/a.txt a.txt
# ln -s /boot/a.txt .
# ln -s /boot/a.txt /root
# ln -s /boot/a.txt /root/a.txt
# ln -s /boot/a.txt $HOME
# ln -s /boot/a.txt $HOME/a.txt

# ll a.txt
lrwxrwxrwx. 1 root root 11  2월 20 21:29 a.txt -> /boot/a.txt
#ln -s hello.py hello2.py
두 파일의 내용이 동일하다.
# cat hello.py
# cat hello2.py

심볼릭링크는 디렉터리도 링크를 생성할 수 있다.
# mkdir dirA; ln -s dirA DIRA
# ls -l
합계 0
lrwxrwxrwx. 1 root root 4  2월 20 21:20 DIRA -> dirA
drwxr-xr-x. 2 root root 6  2월 20 21:19 dirA

  . echo: 메시지와 변수의 저장된 값을 출력하는 명령어

  . stat: 파일 또는 파일 시스템 상태를 표시하는 명령어

  . cat: 파일의 내용을 출력하는 명령어

  . less/more: 파일의 내용을 출력하는 명령어 (페이지 단위)
# less /etc/passwd /키로 원하는 단어를 검색하고 해당 부분으로 이동가능
# more /etc/passwd 입력이 제한되어 있어 검색기능이X 
둘다 q키로 끔

  . head: 파일의 처음 부분의 내용을 출력하는 명령어
    ls --help | head
# head passwd
# head -3 /etc/passwd
# head /etc/passwd -3  <-- 에러
# head -n 3 /etc/passwd
# head /etc/passwd -n 3

  . tail: 파일의 끝부분의 내용을 출력하는 명령어
# tail passwd
# tail -3 /etc/passwd
# tail /etc/passwd -3  <-- 에러
# tail -n 3 /etc/passwd
# tail /etc/passwd -n 3


  . touch: 빈 파일을 생성하거나 파일의 최근 수정 시간을 변경하는 명령어

  . grep: 파일에서 특정 패턴을 검색하는 명령어

  . find: 파일을 검색하는 명령어
   -type <파일형식>
  
    -: 일반파일이면서 실행파일   *          찾다 / -[1하위 디렉토리에서만] -디렉토리타입 -상세정보
   d: 디렉터리                       /              # find -maxdepth 1 -type d  -ls
   l: 심볼릭링크(바로가기)        @             # find -maxdepth 1 -type l  -ls
   b: 블럭장치(하드디스크)                       # find /dev -type b -ls
   c: 문자장치(터미널)                            # find /dev -type c -ls
   p: 파이프                         |(shift+\)    # find / -type p -ls
   s: 소켓                            =              # find /dev -type s -ls

  . chmod: 파일의 허가권을 변경하는 명령어

  . chown: 파일의 소유권을 변경하는 명령어

  . chgrp: 파일의 그룹을 변경하는 명령어

  . whish 명령어: 명령어의 위치,유무를 알려준다.

단축키
Ctrl + S : 터미널 잠금
Ctrl + Q : 터미널 잠금 해제
Ctrl + C : 취소

실습> nano 편집기 사용하기
RedHat 계열: yum, dnf 를 이용해서 애플리케이션을 설치한다.
Debian 계열: apt-get, apt 를 이용해서 애플리케이션을 설치한다.

vi 편집기 사용이 어려운 분들은 nono 편집기를 사용한다.
# yum -y install nano
# nano test.txt

  GNU nano 2.3.1               File: test.txt                            Modified

이 파일은 nano 편집기를 사용해서 저장합니다.


^G Get Help  ^O WriteOut  ^R Read File ^Y Prev Page ^K Cut Text  ^C Cur Pos
^X Exit      ^J Justify   ^W Where Is  ^V Next Page ^U UnCut Text^T To Spell

Ctrl + O를 입력하면 아래쪽에 메뉴가 바뀌고 이 상태에서 엔터를 치면 저장된다.

File Name to Write: test.txt
^G Get Help         M-D DOS Format      M-A Append          M-B Backup File
^C Cancel           M-M Mac Format      M-P Prepend

Ctrl + X를 입력하면 종료한다.

저장하지 않고 Ctrl + X 를 누르면 아래처럼 3개의 메뉴가 나온다.
Yes
No    ^C Cancel
 

실습> vi 편집기
디렉터리 위치: /usr/bin/vi

vi > i > 입력 ... > ESC > :q!
# vi 
안녕하세요.

ESC > :q!


# vi hello.py

i > 아래 코드를 입력한다.

print("Hello Linux!")

ESC > :wq


# cat hello.py
print("Hello Linux!")

# python hello.py
Hello Linux!
# ls -l hello.py
-rw-r--r--. 1 root root 22  2월 20 20:53 hello.py


# chmod 755 hello.py
# ls -l hello.py
-rwxr-xr-x. 1 root root 22  2월 20 20:53 hello.py

vi hello.py > i > 입력 > ESC > :wq
# vi hello.py
#!/usr/bin/python

print("Hello Linux!")

# hello.py
-bash: hello.py: command not found

# echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/root/bin

# ./hello.py
Hello Linux!


실습> 웹서버를 설치하고 심볼릭 링크 파일을 생성하기

웹서버 패키지명: httpd

httpd 패키지를 설치한다.
# yum -y install httpd

방화벽을 모두 중지한다.
웹서버로 접근하는 클라이언트의 요청(Request)을 받아들이기 위해서 중지한다.
# systemctl stop firewalld

웹서버(httpd)를 실행한다. 
# systemctl start httpd  <-- systemctl start httpd.service

# cd /var/www/html

:wq 단축키: ZZ
:q! 단축키: ZQ

i > 입력 > ESC > ZZ(:wq) 단축키
# vi test.html
홍길동 웹서버에 오신 것을 환영합니다.


# ll
합계 4
-rw-r--r--. 1 root root 54  2월 20 21:42 test.html
# cat test.html
홍길동 웹서버에 오신 것을 환영합니다.

http://192.168.100.3/
환영 메세지가 출력된다.

http://192.168.100.3/test.html
홍길동 웹서버에 오신 것을 환영합니다.

현재 디렉터리에 test.html 파일을 현재 디렉터리에 index.html 파일로 심볼릭 링크를 생성한다.
# ln -s test.html index.html
# ll
합계 4
lrwxrwxrwx. 1 root root  9  2월 20 21:45 index.html -> test.html
-rw-r--r--. 1 root root 54  2월 20 21:42 test.html
[root@localhost html]# cat index.html
홍길동 웹서버에 오신 것을 환영합니다.

http://192.168.100.3/
홍길동 웹서버에 오신 것을 환영합니다.

vi > i > 수정 > ESC > :wq or ZZ 
# vi test.html
<center>홍길동 웹서버에 오신 것을 환영합니다.</center>

# cat index.html
<center>홍길동 웹서버에 오신 것을 환영합니다.</center>
