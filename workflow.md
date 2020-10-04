# Github Workflow - TEAM 이준혁

Team 이준혁의 Github workflow 에 대한 설명을 하는 md파일입니다.

***작업방법***
1. 이 workflow.md파일이 있는 팀 레포지토리를 Fork해서 만들어지는 개인 repository에서 작업합니다. **fork를 끝내면 fork된 repository를 clone합니다.**

2. 저번 시간에 작성했던 workflow 전략에 대한 설명을 각 branch 당 한사람씩 작성합니다. **작업은 5개의 브랜치 중 master 브랜치에서 하시면 됩니다.**(hotfix, features, develop, master, release). 이때, 각 branch에 대한 설명을 이 workflow.md파일에다 작성해야하며, vim 에디터를 이용해서 작성해야합니다.

각 branch를 설명할 팀원은 다음과 같습니다.
> ### branch 설명담당
> * master - 
> * develop -
> * features -
> * hotfix -
> * release -

3. 작업이 끝나면 Fork한 repository에 작업을 병합시킨 후, Fork한 repository의 원본 repository로 pull request를 진행합니다.

*주의 : pull request된 작업물을 원본에 merge 시키는 작업은 팀장만 가능합니다.*

* 같은 시간대에 여러사람이 작업 후 원본 repository에 pull request 하여 작업을 업데이트 하게 되면, commit후 pull request 시에 오류가 발생할 수 있습니다.

* 따라서, pull request 시에 오류가 발생하게 된다면, **git remote add upstream "원본 repository 주소"** 명령어를 이용하여 원본 repository를 upstream으로 설정한 후, **git pull upstream master** 명령어를 사용해서 원본 repository의 변경사항을 fork한 repository로 가져온 후, 자신이 작업한 변경사항을 수기로 재입력, 재commit하여 pull request하거나 rebase를 진행하여 pull request 하면 됩니다.

commit 충돌 시 rebase를 이용하여 충돌을 해결하는 방법 : <https://lhy.kr/git-workflow>

pull request 하는 방법 : <https://engineering-skcc.github.io/github%20pages/github-pages-fork-1/>

fork repository와 원본 repository에 충돌이 발생했을 때 해결하는 방법 : <https://engineering-skcc.github.io/github%20pages/github-pages-fork-2/>



## Master branch

작성자 : 

## Develop branch

작성자 : 

## Features branch

작성자 : 

## Hotfix branch

작성자 : 

## Release branch

작성자 : 

