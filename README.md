# ✨ 알고리즘 스터디 GitHub 사용 가이드
## 🚨 메인 브랜치에는 직접 푸쉬하지 않기!
1. 주마다 새로운 브랜치를 만들어서(1인당 1개) 문제 풀이 진행
2. 주차별 과제를 모두 해결한 후, 메인 브랜치로 Pull Request(PR) 보내기
3. 다른 스터디원이 코드를 확인 후 리뷰 작성 및 PR 승인
4. 문제를 다 풀지 못했더라도 진행한 부분까지 공유해 주세요!
## 📌 GitHub 기본 사용법 (VS Code 기준)
### 1️⃣ 레포지토리 클론받기

1. VS Code에서 `F1` → `Git: Clone` 입력
![image](https://github.com/user-attachments/assets/12201539-681b-4b3b-aada-d9609e7c01d0)
2. Clone from GitHub -> 이 레포지토리 선택  
3. 저장할 디렉토리 선택  
4. 클론 완료!  
### 2️⃣ 브랜치 만들기
## ⚡ 브랜치 만들기 전 최신 코드 받아오기
VS Code 터미널 상에서 아래 명령어 입력
![image](https://github.com/user-attachments/assets/8e554533-3bcf-41a5-b7b3-5b5f7d747314)
```bash
git checkout main
git pull origin main
```
새로운 브랜치 생성(main 브랜치 위치에서 생성해주세요!)
![image](https://github.com/user-attachments/assets/b79e133d-7a51-41a8-987b-86561550c66d)
```bash
git checkout -b 자신이름_week00
```
## ✅ 브랜치 네이밍 규칙:
자신이름_week00 
```bash
git checkout -b hyunwoo_week01
```
### 코드파일 작성하기


1. VS code 내에서 클론받은 레포지토리 폴더에 위치해있는지 확인
![스크린샷 2025-02-24 18-48-22](https://github.com/user-attachments/assets/43161ec1-2566-470a-8906-c8b915b74cd1)
2. 그렇지 않다면 좌상단 `File` -> `New Window` -> 새창이 열리면 `Open folder` 클릭 후 클론받은 레포 이름의 폴더열기
   혹은 터미널 상에서 `cd 레포지토리 저장경로` 입력
![image](https://github.com/user-attachments/assets/3f99c212-cb13-4f54-bb58-72d6e61e0784)
4. 본인 이름의 폴더 생성하기(최초 1회만)

VS코드 상에서 생성하거나 
![image](https://github.com/user-attachments/assets/5597c5ad-a835-483b-aaf4-64a2c0eb3c82)

스터디 레포지토리 위치에서 `mkdir 폴더명`으로 새 폴더 생성
![image](https://github.com/user-attachments/assets/2a6c0b12-cadb-4269-8c17-40fce0f2ba27)

5. 본인 이름 폴더 내에서 `'week00' 폴더` 생성 후 코드 작성

### 3️⃣ 코드파일 커밋 후 푸쉬하기
## 💻 VS Code에서 커밋 & 푸쉬

1. 현재 브랜치 위치 확인(자신의 브랜치에 위치했는지)

![image](https://github.com/user-attachments/assets/1e3156bf-a1c5-4de1-822a-bb8651129360)

2. 그렇지 않다면 브랜치 전환

![image](https://github.com/user-attachments/assets/81b77146-0baf-46c0-819d-73fb954afa5f)

3. 변경 사항이 있거나, 새로 추가된 파일은 Changes에 자동으로 뜨게 됨

VS Code `소스 컨트롤` → `+` 버튼 클릭하여 변경 사항 추가

![image](https://github.com/user-attachments/assets/ae55ed45-2477-4a21-b236-4fbf74d9f978)  
4. 커밋 메시지 작성 후 `Commit` 버튼 클릭

커밋 메시지 양식: `백준 0000번 문제풀이`

![image](https://github.com/user-attachments/assets/4a629248-a485-4f7f-8758-d524bc8f032a)  
5. 브랜치 확인 후 `Publish branch` or `Sync Changes` 버튼 클릭  

## 🖥️ 터미널에서 커밋 & 푸쉬

1. 현재 브랜치 확인
```bash
git status  
```
2. 브랜치 이동 (필요시)
```bash
git checkout 이동할 브랜치
```

3. 변경된 파일 추가
git add 파일명  
예시:
```bash
git add 1001.cpp  
```
4. 커밋 메시지 작성
git commit -m "커밋 메시지"
``` bash
git commit -m "백준 1001번 - A+B 풀이"
```
5. 원격 브랜치에 푸쉬
git push origin 브랜치명
``` bash
git push origin 이름_week00  
```
6. 깃허브에서 푸쉬된 내용 확인!

### 4️⃣ Pull Request(PR) 보내기
## 🔥 PR 머지 순서 (메인 -> 개인 브랜치 -> 메인)


1. Github에서 `New pull request` 클릭 -> 메인 브랜치에서 자신의 브랜치로 PR 생성
![image](https://github.com/user-attachments/assets/0b44c3c0-0fc3-4bbb-ac0e-c19c41cb5c99)

2. base 브랜치를 자신의 브랜치, compare 브랜치를 `main` 브랜치로 설정 -> `Create pull request`
(만약 There isn't anything to compare이 뜬다면 5번부터 수행!)

![image](https://github.com/user-attachments/assets/547965f3-89ba-4c23-81f5-9813494113f9)

4. title 입력 후(양식: 머지 전 충돌 테스트) Assignees로 본인 할당   
![image](https://github.com/user-attachments/assets/a4cdb86f-f5e9-4bcd-bb5b-2f3262363648)

4. `Create pull request` 클릭 후 해당 PR은 본인이 수락 `Merge pull request` -> `Confirm merge`

![image](https://github.com/user-attachments/assets/b2f74c2a-866c-4a1b-a166-3cd4e5af0499)

5. GitHub에서 자신의 브랜치에서 메인 브랜치로 PR 생성

6. base 브랜치를 `main`으로, compare 브랜치를 자신의 브랜치로 설정 -> `Create pull request`

![image](https://github.com/user-attachments/assets/db6bc126-71ef-481c-9dcf-724ec284677c)


7. title 입력 후(양식: 이름 week00) `Asigeens`로 본인 제외한 다른 사람들 전부 체크!
8. `Create pull request` 클릭
10. 다른 스터디원이 검토 후 `main` 브랜치로 머지 `Merge pull request` -> `Confirm merge`
11. 코드에서 좋았던 부분, 개선 가능할 부분에 대하여 코멘트 달아주기!
![image](https://github.com/user-attachments/assets/b5d19f81-d7d6-447d-bbea-d740bf3bbbd8)

📚 추가 참고 사항
작업은 각각 자신의 폴더에서만 진행하기에 머지 시 conflict(충돌)이 발생할일은 거의 없지만 발생 시 스터디 진행자에게 연락해 주세요!
각 단계를 진행하는 중, 이해가 안되는 부분이나, 잘 안되는 부분이 있으면 스터디 진행자에게 연락해 주세요!
