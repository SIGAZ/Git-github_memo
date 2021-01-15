# Git-github_memo
## 깃 관련 메모
### 깃 주요 용어 간략 정리

- 사용 컴퓨터 - Local repository
- 깃허브 - Remote repository

- Working directory: 작업할 파일이 있는 디렉토리
- Staging area: 커밋을 수행할 파일들이 올라가는 영역
- Git directory: git 프로젝트의 메타 데이터와 데이터 정보가 저장되는 디렉토리

### push step
- working directory 
- ↓ (git add)
- staging area
- ↓ (git commit)
- local directory
- ↓ (git push)
- remote repository

### pull step
- remote repository
- ↓ (git fetch)
- local directory
- ↓ (git merge)
- staging area, working directory 

### 깃 초반 설정
- git config --global user.name (name)
- git config --global user.email (email adress)

### 깃 주요 사용 방법 정리
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


### Readme에서 소스코드는 "'''(해당언어)" 키워드로 만들 수 있다.

'''(c)
#inlcude <stdio.h>

int main (void)
{
  printf("hello world")
  return 0;
}
'''

### 링크는 ()로 사용할수 있으며, 하이퍼링크는 []로 사용할 수 있다.
(https://blog.naver.com/rnwjdgus7)
[SIGAZ BLOG] (https://blog.naver.com/rnwjdgus7)

### 목록은 Shift + 8 인 별을 통해 만들수 있다 
- 별은 최대 3개까지 사용 가능하다

*목록
**목록
***목록
***목록 1)
***목록 2)

### 인용 구문은 '>(구문) - (사용자)'를 통해 만들 수 있다.
> "깃허브 사용은 프로그래머를 진화시키는 행동이다. - SIGAZ


### 테이블은 Shift + \(원화)인 | 를 통해 만들 수 있다

테이블1|테이블2|테이블3
값1|값2|값3
---|---|---

### 볼드(굵게)체는 별 두개를 열고 닫아 사용할 수 있다. 
**볼드체**

### 취소선은 물결표(~) 두개를 열고 닫아 사용할 수 있다.
~~저는 HTML로 프로그래밍 해요~~ HTML은 프로그래밍 언어가 아닙니다
