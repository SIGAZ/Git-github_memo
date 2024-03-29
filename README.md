# Git-github_memo (깃 관련 메모)
## 깃 주요 용어 간략 정리

- 사용 컴퓨터 - Local repository
- 깃허브 - Remote repository

- Working directory: 작업할 파일이 있는 디렉토리
- Staging area: 커밋을 수행할 파일들이 올라가는 영역
- Git directory: git 프로젝트의 메타 데이터와 데이터 정보가 저장되는 디렉토리


## push step
working directory -> (git add) -> staging area -> (git commit) -> local directory -> (git push) -> remote repository


## pull step
remote repository -> (git fetch) -> local directory -> (git merge) -> staging area, working directory 


## 깃 초반 설정
- git config --global user.name (name)
- git config --global user.email (email adress)


## 깃 주요 사용 방법 정리
- repository, commit까지 하면 해당 폴더 내 .git 폴더에 저장된다.
- push 전까지는 전부 local에만 반영

- branch는 한 project에 여러 개발자들이 각각 다른 기능을 개발할 수 있다
- git에 project를 올리는 것이 대부분 master branch
- master branch는 배포가 가능한 수준의 안정화된 버전을 포함
- 또한 master branch는 언제든지 계속 안정화되어 있어야 된다.
- merge 전까지는 안정적으로 배포 가능

- 생성한 branch는 보통 개발/버그픽스로 나누어 개발한다 
- 개발 branch에서 작업을 마무리 한 뒤 master branch에서 merge를 한다. 
- branch가 서로 다른 상태에서 merge작업을 할때 error를 출력한다.  
- 소스코드에서 명시해주는데, "====="를 기준으로 윗쪽이 master branch, 아랫쪽이 sub branch
- 내용을 수정한 다음에 merge해주면 완료

## 깃허브 순서
1. 리포지토리 생성
2. 리포지토리에 프로그램 작성 및 추가
3. 커밋
4. 핫픽스 브랜치 생성 및 이동
5. 프로그램 수정
6. 커밋
7. 마스터 브랜치에 병합
8. 마스터 브랜치에 변경점 하나 추가
9. 커밋
10. 핫픽스 브랜치에 변경점 하나 추가
11. 커밋
12. 마스터와 핫픽스 브랜치 사이에 영향이 없음을 확인
13. 불필요한 프로젝트 파일을 관리 대상에서 제외하기
14. 충돌 해결하기
15. 기록 보기


## Readme에서 소스코드 작성
- 소스코드는 ESC 아래 키의 물결표에 있는 '를 3개 넣어 열고 닫으면 된다. 
- 3개를 넣은 뒤에 해당언어 키워드를 넣어 IDE 소드코드처럼 만들 수 있다.

``` C
#inlcude <stdio.h>

int main (void)
{
  printf("hello world")
  return 0;
}
```

## 링크는 ()로 사용할수 있으며, 하이퍼링크는 []로 사용할 수 있다.
- https://blog.naver.com/rnwjdgus7
- [SIGAZ BLOG](https://blog.naver.com/rnwjdgus7)


## 목록은 사칙연산중 덧셈,뺄셈,곱셈 기호를 통해 만들수 있다 
- 최대 3개까지 사용 가능하다
- 2개부터 탭을 넣어 구분을 해야된다. 

- 목록
  - 목록

## 구분선
- 구분선은 뺄셈 선을 길게 넣으면 자동으로 인식한다
-----------


## 인용구문
- 인용 구문은 '>(구문) - (사용자)'를 통해 만들 수 있다.
> "깃허브 사용은 프로그래머를 진화시키는 행동이다." - SIGAZ


## 테이블
- 테이블은 Shift + \(원화)인 | 를 통해 만들 수 있다
- 테이블 헤더에 "---|---" 를 넣어야 인식한다. 

테이블1|테이블2|테이블3
---|---|---
값1|값2|값3


## 볼드(굵게)체 
- 별 두개를 열고 닫아 사용할 수 있다. 
- **볼드체**


## 취소선
- 취소선은 물결표(~) 두개를 열고 닫아 사용할 수 있다.
- ~~저는 html로 프로그래밍 해요~~  html은 프로그래밍 언어가 아닙니다








## 레퍼런스 링크
https://gist.github.com/ihoneymon/652be052a0727ad59601
