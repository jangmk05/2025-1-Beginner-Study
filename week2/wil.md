## Git으로 파일 관리하기

-git init : git 저장소를 새로 초기화하는 명령어 이다.

-git add <파일명> : git에서 파일을 스테이지에 추가하는 명령어

-git commit : 스테이지에 올려놓은파일을 실제로 기록

-git push origin main : 원격저장호인 origin에서 브랜치인 main으로 푸시한다.

## Fork

:다른 사용자의 Repository를 자신의 계정으로 복사하여 독립적으로 수정하고 관리

## Star

:관심 있는 Repository나 프로젝트에 star를 달아 북마크처럼 관리

## Issue

:Repository에서 작업 계획, 토론 및 추적을 위해 활용

## Branch

:기존 브랜치에서 분리되어 생성되는 별도의 작업 공간

-> Fork와 달리 같은 Repository에 생성됨

-> type/<issue 번호>-<간략한 설명>
ex. "docs/1-readme"

## Pull Request

:분기된 Branch를 다시 병합하기 위한 절차, 새로운 변경을 제안하거나 병합시 발생하는 충돌을 해결, Merge에 앞서 코드 리뷰

## Merge

(1)Merge commit
: 기본적인 병합 방식, 두 브랜치의 변경 사항을 하나의 새로운 커밋으로 병합

(2)Squash and Merge
: 여러개의 커밋을 하나의 커밋으로 압축(squash)하여 병합

(3)Rebase and Merge
: 원본 브랜치 위에 변경 사항을 재정렬한 후, 병합하는 방식이다.
병합할 브랜치를 원본 브랜치의 끝으로 붙여넣어 선형적인 히스토리를 만듦, 모두 새로운 커밋으로 변경

## 실습 
<https://github.com/jangmk05/2025-1-Beginner-Study/pull/1>