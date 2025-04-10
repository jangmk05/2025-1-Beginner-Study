## git log

- commit 기록을 최신 순으로 확인

- --oneline 옵션을 사용하면 각 커밋을 한 줄에 요약

## commit Id

- commit의 식별을 위해 사용하는 40자 길이의 16진수

- 중복 확률은 2의 80제곱 분의 1

- SHA-1 해시 함수를 사용

## HEAD

-  HEAD는 현재 작업중인 위치를 가리킨다.

- 현재 작업중인 브랜치의 가장 최근 commit

- 다음 commit의 base가 되는 commit

- 새로운 commit이 생기면 HEAD도 변경

## git status

- 세 가지 상태에 따라 파일을 분류하여 확인

# commit --amend
:마지막 commit의 내용에 변경이 있을 때 사용

- 완전히 새로운 커밋으로 대체(commit id가 바뀜)

- vim으로 진입하여 커밋 메시지를 수정하게 됨

1) '-m' option으로 vim 진입 없이 commit 메시지수정하기
: $ git commit --ammend -m "커밋 메시지"

2) '--no-edit' option으로 commit 메시지 수정없이 커밋 수정
: $ git commit --amend --no-edit

- commit --amend 주의 사항
: 다른 사람이 작업 기반으로 삼고 있는 commit은 amend하면 안된다.

# reset
: 커밋을 제거하는 데 사용

- 3가지 옵션 존재(soft, mixed, hard)

- 돌아갈 커밋의 id를 사용
ex. $ git reset --soft a1s2d3f

## reset --soft
: 커밋만 취소하고 변경 사항이 staging area로 돌아감

## reset --mixed
: 커밋을 취소하고 변경사항이 working directory로 돌아감

## reset --hard
: 커밋을 취소하고 변경사항을 모두 제거해 이전 커밋으로 돌아감

# revert
: 커밋을 제거하지 않고 되돌림

-되돌리기 위한 새로운 commit이 생성

- --edit 옵션이 디폴트

# revert --no-edit
: 편집기 진입 없이 바로 revert 가능

- $ git revert --no-edit "<commit id>"

# revert --no-commit
: 직접 커밋하지 않고, revert 내용을 staging area에 올림

# reset vs revert

- reset은 커밋을 삭제하므로 위험

- 커밋을 공유하는 다른 브랜치에도 영향을 줄 수 있음

- 커밋을 삭제하기보다 생성하여 되돌리는 revert가 안전
