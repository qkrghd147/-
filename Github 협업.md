## 주요 코드!
* **git init**  git 저장소를 초기화
* **git add .**  폴더에 변경된 모든파일 staging area에 올리기
* **git commit –m “커밋에 대한 설명”** 유사시에 돌아갈 수 있는 저장소의 체크포인트 생성
* **git remote add origin http://원격 저장소 주소** git 원격저장소(remote repository)연결
## branch 관련 코드
* **git branch 브랜치 명** 새로운 브랜치를 생성
* **git checkout 브랜치 명** 해당 브랜치로 이동
* **git push origin 브랜치** 원격 저장소의 특정 브랜치에 프로젝트 저장
* **git pull origin 브랜치** 원격 저장소의 특정 브랜치에서 변경사항 pull 해오기
* **git clone http:// 원격 저장소 주소.** git 원격 저장소에 있는 파일 전체 복사
* **git status git** 저장소의 상태를 확인

## github 협업순서

1. github에서 repository 생성
2. 팀원을 collaborator로 추가
3. 초기 프로젝트를 push
4. 팀원들의 로컬에 프로젝트 pull (push 된 것을 local로 pull 해옴, git clone을 사용하여도 무방!)
5. 팀원 각자의 브랜치를 생성하여 작업
6. 브랜치에 작업 한 내용을 push
7. Master와 merge 하기 전 pull request
8. pull request 확인 후 Master와 merge

## fork를 이용한 협업 

1. 작업 하고 싶은 repository fork 해오기
2. 자신의 로컬에서 작업
3. 변경사항을 자신의 브랜치에 push
4. 원본 레포지토리 소유자에게 pull request 요청
5. 소유자가 pull request를 승인하여 merge하면 자동으로 collaborator 추가
