# Shell Command **NOTE**

### 기본적인 명령어
### 'pwd'
 "현재의 경로를 계층적 디렉터리 구조로 보여주는 명령어"
### 'cd'    
"디렉터리 이동 명령어
##### - arguments

"명령어 'cd'의 경로나 위치를 보기 위해 사용되는 것들" 
- '/' : 루트 표시
- '.' : 현재 디렉터리
- '.\.' : 현재보다 한 단계 상위의 디렉터리
- '~' : 현재 사용자의 홈 디렉터리
- '/[directoryname]' : 디렉터리 절대 경로
- './[directoryname]' : 디렉터리의 상대적 경로
- '.\./[directoryname]' : 한 단계 상위의 디렉터리의 상대적 경로

### 'ls'    
"파일과 디렉터리의 목록 출력 명령어"
##### - options
- '-l' : long format의 형태로 디테일한 정보를 출력
- '-lh' : '-l'과 같지만 사람이 더욱 이해하기 쉽게 출력 ex) 2286 --> 2.2KB
- 'ls [directoryname]' : 정해진 디렉터리 목록 출력
- 'ls -l [directoryname] [directoryname]' : 입력된 디렉터리를 long format의 형태로 출력
- 'ls -la .\.' : 한 단계 상위의 모든 디렉터리 출력
- [ls 추가 자료 및 long format 형태 사진](https://linuxcommand.org/lc3_lts0030.php)

### 'useful function'
- 자동완성 : 'tab' 키
- 이전 명령어 확인 : '↑' 방향키
- 화면 지우기 : 'clear' 명령어  

### 'manipulation'
"파일 및 디렉터리를 조작하는 명령어들"
"***Warning*** : *아래 명령어들은 파일과 디렉터리를 **삭제하거나 덮어쓸 수 있으므로** 중요한 데이터의 백업이 필요*"
##### 1. 'cp'
"파일과 디렉터리 복사"   
- 'cp -r' : 파일 전체를 현재의 폴더 안에 복사
- 'cp file1 file2' : file2가 있다면, file1을 file2에 덮어쓰기 / 없다면, file2를 만들어 복사
- 'cp file1 dir1' : file1을 dir1(디렉터리)안에 복사
- 'cp -R dir1 dir2' : dir1을 dir2에 복사
- [cp관련 추가 자료](Source:https://linuxcommand.org/lc3_lts0050.php)

##### 2. 'mv'
"파일과 디렉터리 이동 또는 이름 변경"    
- 'mv file1 file2' : file2가 없다면 file1의 이름을 file2로 변경 / 있다면, file1의 내용으로 변경
- 'mv file1 file2 dir1' : file1과 file2를 dir1으로 위치 변경 / dir1이 없으면 오류 발생
- 'mv file1 file2' : dir2가 없다면 dir1의 이름을 dir2로 변경 / 있다면, dir1의 내용이 dir2 내부로 이동
- [mv관련 추가 자료](https://linuxcommand.org/lc3_lts0050.php)

##### 3. 'rm'
"파일과 디렉터리를 영구적으로 되돌릴 수 없게 삭제"
- 'rm file1 file2' : file1과 file2를 영구 삭제
- 'rm -r dir1 dir2' : dir1과 dir2를 영구 삭제
- [rm관련 추가 자료](https://linuxcommand.org/lc3_lts0050.php)

##### 4. 'mkdir'
"새 디렉터리 생성"
- 'mkdir [directoryname]' : 디렉터리 생성

##### 5. 'wildcards'
"***rm과 함께 사용할 때에는 ls를 활용해 확인을 잘 하는 것이 좋음***"
- '*' : 모든 파일 이름
- g* : "g"로 시작하는 모든 파일
- 'b*.txt' : "b"로 시작하고 ".txt"로 끝나는 모든 파일
- "Data???" : 데이터 크기에 맞는 모든 파일 ex) 123 (O) / 1234 (X)
- [추가 wildcard 및 추가 응용](https://linuxcommand.org/lc3_lts0050.php)

### 'etc'
1. 'help [command]' : 명령어에 대한 설명 및 매뉴얼 확인
2. 'man [command]' : help와 동일하게 설명 및 매뉴얼 확인
3. 'exit' : 터미널 종료

