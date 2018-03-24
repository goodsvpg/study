## 1.Homebrew 로 설치하기 & 왜 Homebrew를 쓰는가

http://www.popit.kr/개발자를-위한-맥mac-정보-패키지관리자-homebrew/
https://swiftcoding.org/homebrew-installation

## 2.기본적인 사용법

https://chartio.com/resources/tutorials/how-to-start-postgresql-server-on-mac-os-x/

### role 생성
``` CREATE ROLE username WITH LOGIN PASSWORD 'quoted password' [OPTIONS] ```

_참고 : https://www.postgresql.org/docs/9.5/static/sql-createrole.html_
### 권한 추가
``` ALTER ROLE username CREATEDB; ``` 

_참고 : https://www.postgresql.org/docs/9.5/static/sql-alterrole.html_

### 데이터베이스 생성
``` psql postgres -U username ```
``` postgres=> CREATE DATABASE databasename; ```

### 유저에게 데이터베이스 접근 허용
``` GRANT ALL PRIVILEGES ON DATABASE databasename TO username; 
postgres=> \list -- lists all the databases in Postgres
postgres=> \connect databasename
postgres=> \dt -- list the tables in the currently connected database
```

출처 : https://www.codementor.io/engineerapart/getting-started-with-postgresql-on-mac-osx-are8jcopb

### PostgreSQL 에서 command line 으로 sql 실행하기
``` psql -U username -d myDataBase -a -f myInsertFile ```
출처 : http://i5on9i.blogspot.kr/2016/02/db-postgresql-command-line-sql.html
