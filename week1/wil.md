1. 개발 그냥 하면 되는거 아닌가?
: 좋은 코드를 짜는 것도 중요하지만 그 코드를 관리하는 것도 중요하다.
  - 코드의 수정을 관리해야 한다 (누가 언제 어떻게 수정했는지 알 수 있어야함)
  - 잔뜩 쌓인 파일들을 관리해야 한다.(-> git, git hub 사용)
  - 개발은 혼자 하는 일이 아니다 

2. Git 
:버전 관리 및 협업을 위해 사용하는 오픈소스 소프트웨어
  - 어떤 파일을 누가 언제 어떻게 수정됐는지를 추적하고 원하는 상태의 코드를 사용하기 위해 사용

3. 파일의 생명주기
   (1)untracked : 추적되고 있는 상태 (처음 파일을 만들었을 때)
   (2)tracked : 추적되지 않고 있는 상태
     -unmodified : 수정 x
     -modified : 수정 됨
     -staged 

4. Git의 영역
   (1)working Directory 
   (2)staging Area : git add를 통한 대기 장소
   (3)repository : git commit을통해 저장

5. Git으로 파일 관리하기
   (1)a. git init : 디렉토리에 Git 저장소를 만들기
   (2)a. git add : git으로 관리할 대상 등록하기
   (3)a. git commit : 파일 수정 후 로컬 저장소로 옮기기

6. Git에서 GitHub로
   locoal repo -> remote repo : git push
   remote repo -> working directory : git pull
