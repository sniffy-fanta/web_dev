# Hacking Practice

모의해킹 스터디를 하며 실습한 웹 개발 프로젝트입니다.

<br>

## Web Site

웹 모의해킹 스터디에서 처음으로 웹 개발을 하며 다양한 보안 테스트와 기능 구현을 직접 실습한 사이트입니다.

<br>

### 주요 업데이트 이력

Git 커밋 이력이 정상적으로 남지 않은 부분이 있습니다. (Git 연습 과정 중 기록 누락)

<br>

### DB/환경 설정

- **사용 환경**: Apache, PHP, MySQL

| 테이블명   | 주요 컬럼                                 |
|------------|------------------------------------------|
| users      | idx(PK), userid, userpw, name, address   |
| board      | idx(PK), title, content, author, post_date, file, views, likes |
| post_likes | idx(PK), post_id, user_id                |

- DB 이름: `mydb`
- DB 백업 파일: `fanta_backup.sql` (새 DB 사용하셔도되고 백업 파일 사용하셔도 됩니다.)

<br>

### 실행/이용 가이드

1. **코드 다운로드**
    ```bash
    git clone https://github.com/sniffy-fanta/web_dev.git
    cd web_dev
    ```

2. **웹 서버(루트 경로)로 파일 복사**
    ```bash
    sudo cp -r * 웹 서버 루트 경로
    예시) sudo cp --r * /var/www/html
    ```

3. **웹서버 구동 후 접속**
- 해당 파일들은 웹 서버 설정에서 지정한 IP 및 PORT를 주소란에 치시고 들어가시면 됩니다.
- 예시) `http://localhost:80/pages/login.php`

<br>

### 테스트 계정

- messi / 123456
- ronaldo / 123456

<br>

### 개인적인 파일 및 특이사항

- **keylogger.js** : 키로깅(쿠키·키 입력 탈취) 스크립트
- **keylogger.php** : 공격자 입장에서 테스트할 수 있는 PHP 파일
- **keylogger.log** : 키로거 로그 파일
- **cookie.php** : 세션 쿠키 탈취 파일
- **cookie.log** : 탈취된 쿠키 기록 파일

<br>

### 기타 안내

- 각 파일/폴더는 실습 및 보안 테스트 용도로 제작되었습니다.
- 실제 운영 환경에서는 모든 취약점 관련 파일 삭제, 권한 설정 강화 등이 반드시 필요합니다.


  
