# git 설치하기
### http://git-scm.com/ 에서 git download | 모두 기본값으로 설치.

# git 환경설정            | user.name, user.email 설정
### $ git config --global user.name "LEE"
### $ git config --global user.email "beeeeee@gmail.com"

# git에서 기본 편집기 변경하기
### $ git config --global core.editor "notepad++"

# git 초기화.
### $ git init 
##### - 현재 directory를 초기화.
### $ git init dir_name
##### - dir_name 하위 dir이 있으면 초기화, 없으면 만들고 초기화

# Staging.
### $ git add hello.txt

# Commit
### $ git commit -m "Message1"
##### - stage에 올라온 파일을 Message1이라는 메세지를 포함하여(-m) commit
# Staging & Commit 동시에 | $ commit -am
### $ git commit -am "message2"

# Status & log
##### - status는 현재 어느 branch에 있는지, stage, commit해야 하는 파일들 상태 보여주는 것.
##### - log는 commit한 버전에 관한 정보들을 나열 한다. commit한 사람, commit message들을 
### $ git status
##### - branch, 파일 수정상태, Staging, Commit여부 등 
### $ git diff
##### - 방금수정한 파일과, 저장소에 있는 최신 파일의 차이를 보여줌.
### $ git log --stat
##### - commit에 관련된 file까지 함께 나열.




