# git 설치하기
### http://git-scm.com/ 에서 git download | 모두 기본값으로 설치.

# git 환경설정            | user.name, user.email 설정
### $ git config --global user.name "LEE"
### $ git config --global user.email "beeeeee@gmail.com"

# git에서 기본 편집기 변경하기
### $ git config --global core.editor "notepad++"

# git initialization.
### $ git init 
##### - 현재 directory를 초기화.
### $ git init dir_name
##### - dir_name 하위 dir이 있으면 초기화, 없으면 만들고 초기화

# Staging & Commit
### $ git add hello.txt
##### - Staging.
### $ git commit -m "Message1"
##### - Commit | stage에 올라온 파일을 Message1이라는 메세지를 포함하여(-m) commit
### $ git commit -am "message2"
##### - Staging & Commit 동시에 | 한번이라도 staging을 했던 파일만 가능
### $ git commit --amend 
##### - 가장 최근의 commit message를 수정. - vim에서 수정하고, 저장.

# Status & log
##### - status는 현재 어느 branch에 있는지, stage, commit해야 하는 파일들 상태 보여주는 것.
##### - log는 commit한 버전에 관한 정보들을 나열 한다. commit한 사람, commit message들을 
### $ git status
##### - branch, 파일 수정상태, Staging, Commit여부 등 
### $ git diff
##### - 방금수정한 파일과, 저장소에 있는 최신 파일의 차이를 보여줌.
### $ git log --stat
##### - commit에 관련된 file까지 함께 나열.
### $ git log --oneline
##### - commit에 관련된 정보를 한줄로 보여줌.
### $ git log --branches
##### - 각 branch들의 최신 commit들을 같이 나열해 줌.
### $ git log --graph
##### - 각 branch들의 계통을 그래프를 그려서 보여줌. (가지치기 모양)


# .gitignore | 버전관리에서 제외.
##### 버전관리 중인 directory안에 vim으로 .gitignore 파일을 만들어 그 안에 제외할 내용적기.
##### mynote.txt
##### temp/
##### .swp
##### -위와 같이 3줄을 .gitignore 파일 안에 작성하면 mynote.txt, temp directoy, 확장자가 swp인 파일을 관리에서 제외한다.

# git checkout | 수정된 파일 되돌리기
### $ git checkout -- hello.txt
##### checkout쓰고 -- 쓰고 공백한칸, 파일이름. | 작업트리에서 수정내용이 원래 파일로 돌아감.

# git reset | 커밋 되돌리기 (이후 내용은 삭제)
### $ git reset HEAD hello2.txt | staging된 hello2.txt파일을 unstaging.
##### - -file- 을 쓰지않으면, 모든 file을 unstaging.
### $ git reset HEAD^
##### - commit까지 했어도 가장 마지막에 한 commit을 취소하고, unstaging한다.
### $ git reset --soft HEAD^
##### - 최근 commit을 하기 전 상태로 작업 트리를 되돌린다.
### $ git reset --mixed HEAD^ | $ git reset
##### - 최근 커밋과 스테이징을 하기전 상태로 작업트리를 되돌림 | $ git reset 과 같다.
### $ git reset --hard HEAD^
##### - 최근 커밋과 스테이징, 파일 수정 하기 전 상태로 되돌림. - 이 작업은 되돌릴 수 없다.
### $ git reset --hard [복사한 커밋 해시]
##### - 해당 커밋 이후의 내용은 삭제하고, 해당 커밋으로 이동.

# git revert | 커밋 삭제하지 않고 되돌리기
### $ git revert [복사한 커밋 해시]
##### - 편집기가 자동으로 열리면서 commit메세지를 입력할 수 있도록 해준다.
###### 이건 잘 이해가 안됨.


  
