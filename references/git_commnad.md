# Git Setting

## 1. 기본 설정하기

- 사용자 설정
 ```
  $ git config --global user.name [user_name]
  ```

- 메일 설정

  ```
  $ git config --global user.mail [user_mail]
  ```

- config 확인

  ```
  $ git config --list
  ```

## 2. 로컬저장소 만들기

- 저장소 만들기
 ```
  $ mkdir [project_name]
  ```

- 저장소 들어가기
 ```
  $ CD [project_name]
  ```

- 로컬 저장소 생성
 ```
  $ git init [project_name]
  ```

- 저장소 내려받기
 ```
  $ git clone [id@원격저장소_URL]
  ```

## 3. File 상태 확인

- File 현재 상태 
 ```
  $ git status
  ```

## 3. Branch

- 조회하기
 ```
  $ git branch -v
  ```

- Branch 생성
 ```
  $ git branch [branch_name]
  ```

- Branch 변경
 ```
  $ git checkout [branch_name]
  ```

- Branch 생성 및 변경
 ```
  $ git checkout -b [branch_name]
  ```

- Branch 확인
 ```
  $ git branch
  ```

## 4. Commit

- 파일 변경 완료
 ```
  $ git commit -m "[commit_msg]"
  ```

## 5. 조회하기

 ```
  $ git log
  ```

## 6. 원격저장소

- 원격저장소 확인
 ```
  $ git remote -v
  $ git remote show origin
  ```

## 6. Merge

- 원격저장소 확인
 ```
  $ git checkout master
  $ git diff origin master
  $ git merge issue
  $ git branch -d issue
  ```

## 7. Pull ( Fetch+Merge )

 ```
  $ git pull
  ```

## 8. Push

 ```
  $ git push origin issue
  $ git request-pull origin issue
  $ git checkout master
  $ git fetch
  $ git merge
  ```

## 9. Pull Request 보내기

 ```
  $ git request-pull origin/master issue
  ```
