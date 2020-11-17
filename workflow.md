# Github Workflow - TEAM 이준혁
SWDEV-1

Team 이준혁의 Github workflow 에 대한 설명을 하는 md파일입니다.

***작업방법***
1. 이 workflow.md파일이 있는 팀 레포지토리를 Fork해서 만들어지는 개인 repository에서 작업합니다. **fork를 끝내면 fork된 repository를 clone합니다.**

2. 저번 시간에 작성했던 workflow 전략에 대한 설명을 각 branch 당 한사람씩 작성합니다. **작업은 5개의 브랜치 중 master 브랜치에서 하시면 됩니다.**(hotfix, features, develop, master, release). 이때, 각 branch에 대한 설명을 이 workflow.md파일에다 작성해야하며, vim 에디터를 이용해서 작성해야합니다.

각 branch를 설명할 팀원은 다음과 같습니다.
> ### branch 설명담당
> * master - 이준혁
> * develop - 박종윤
> * features - 남현기
> * hotfix - 최종인
> * release - 이의형

3. 작업이 끝나면 Fork한 repository에 작업을 병합시킨 후, Fork한 repository의 원본 repository로 pull request를 진행합니다.

*주의 : pull request된 작업물을 원본에 merge 시키는 작업은 팀장만 가능합니다.*

* 같은 시간대에 여러사람이 작업 후 원본 repository에 pull request 하여 작업을 업데이트 하게 되면, commit후 pull request 시에 오류가 발생할 수 있습니다.

* 따라서, pull request 시에 오류가 발생하게 된다면, **git remote add upstream "원본 repository 주소"** 명령어를 이용하여 원본 repository를 upstream으로 설정한 후, **git pull upstream master** 명령어를 사용해서 원본 repository의 변경사항을 fork한 repository로 가져온 후, 자신이 작업한 변경사항을 수기로 재입력, 재commit하여 pull request하거나 rebase를 진행하여 pull request 하면 됩니다.

commit 충돌 시 rebase를 이용하여 충돌을 해결하는 방법 : <https://lhy.kr/git-workflow>

pull request 하는 방법 : <https://engineering-skcc.github.io/github%20pages/github-pages-fork-1/>

fork repository와 원본 repository에 충돌이 발생했을 때 해결하는 방법 : <https://engineering-skcc.github.io/github%20pages/github-pages-fork-2/>



## Master branch

작성자 : 이준혁

develop에서 개발이 완료된 기능들을 중간정리 및 관리를 하는 branch. 다시말해 develop의 작업물을 중간저장하는 branch로 볼 수 있다.
master branch에서 프로그램을 배포하기 전, 배포 전략에 대한 전략수립을 한다. 완성된 전략에 따라서 release branch에서 배포를 진행한다.


## Develop branch

작성자 : 박종윤

주요 기능을 개발하고 features branch에서 개발된 모든 feature들을 병합하고 관리하는 branch입니다.   
상시로 버그를 수정한 커밋들이 추가되며 새로운 기능 추가 작업이 있는 경우 feature branch를 생성하여 작업합니다.   
평소에는 develop branch를 기반으로 개발을 진행하게 됩니다.

## Features branch

작성자 : 남현기

Feature Branch는 Deveplop에서 파생되어 추가적인 feature을 개발할 때 사용하는 Branch이다.

추가 Feature가 개발이 완료되면 **Feature에 존재하는 모든 commit들은 Develop Branch에 rebase된다.**

## Hotfix branch

작성자 : 

## Release branch

작성자 : 이의형

Develop branch를 거쳐 master branch 에 있는 release 준비가 완료된 작업물을 버전 태깅을 거쳐 최종적으로 결과물 release를 진행하는 branch.
