## 1. cat
- 파일 내용 간단하게 출력하거나 두 개 이상의 파일을 연결해서 출력할 때 사용
  ```
  $ cat [옵션] [파일명]
  ```
  - 출력 예시
   + 파일 내용 출력 
    ```
    $ cat file1
     first file
    ```
   + 파일 내용 연속 출력 
    ```
    $ cat file1file2 file3
     first file
     second file
     third file
    ```
  - 생성 예시
   + 기존 파일 지우고 저장 
    ```
    $ cat > file1 (내용 입력 후 ctrl+d 눌러 저장)
     first file
    ```
   + 기존 파일 내용 뒤에 연속해서 기록
    ```
    $ cat >> file1 (내용 입력 후 ctrl+d 눌러 저장)
     first file 
     second file
    ```
  - 병합 예시
   + 여러 파일을 병합하여 하나의 파일로 생성
    ```
    $ cat file1 file2 > file3
    ```

## 2. find
- 특정 파일이나 디렉토리 검색
  ```
  $ fine [검색 경로] -name [파일명]
  ```
- 옵션 
   + -exec : 명령어 실행
   + -type : 디렉토리나 파일만 지정하여 검색
- 예시
   + 확장자명 검색
    ```
    $ find -./ -name '*.txt'
    ```
  +  확장자가 txt인 파일만 찾아 삭제
    ```
    $ find -./ -name '*.txt' -exec rm {} \;
    ```
  +  확장자가 txt인 파일만 찾아 내용 수정
    ```
    $ find -./ -name '*.txt' -exec rm {} \;
    ```
## 3. chmod
- 권한 변경
  ```
  $ chmod [option] [mode] [file]
  ```
- 예시
 +  현재 경로에 있는 .txt 파일 실행 권한 부여 
    ```
    $ chmod +x ./*.txt
    ```
  +  파일 소유한 그룹과 그 외 사용자 모든 구 ㅓㄴ한 제거 
    ```
    $ chmod ro-rwx file1
    ```