# git branch | branch를 확인하거나 만드는 명령어.
### $ git branch | 현재 저장소의 branch들을 확인.
### $ git branch apple | 현재 저장소에 apple branch를 만든다.

# git checkout [branch name] | 해당 branch로 이동.
### $ git checkout apple | apple branch로 이동.

# git log 명령중 branch와 관련된 것.
### $ git log --oneline
##### - commit에 관련된 정보를 한줄로 보여줌.
### $ git log --branches
##### - 각 branch들의 최신 commit들을 같이 나열해 줌.
### $ git log --graph
##### - 각 branch들의 계통을 그래프를 그려서 보여줌. (가지치기 모양)
### $ git log [br1]..[br2]
##### - br1에는 없고, br2에만 있는 commit을 보여줌.

# git merge [br1]
### $ git checkout master
### $ git merge o2
##### master branch로 checkout한 다음. o2 branch를 가져와서 현재 br인 master branch로 병합한다.
### $ git merge o2 --no-edit     |    --edit
##### - commit 메세지 창이 뜨지 않음.   |   commit 메세지 창이 뜸.

