# mysql
## tips
- 상황 : query를 날렸는데 table lock 걸림 
- 해결 방법 : 문제가 되지 않는 프로세스라면 죽인다... 
```
show processlist;
kill <id>
```
- 유사 기능이라도 목적이 다르다면 테이블을 분리해야 각 목적에 따른 요구사항 수용시 독립적으로 수정 가능 하다.
  - 게시판 같은 경우 a게시판 b게시판 등등으로 나뉠때 그 목적이 다르다면 테이블을 달리한다. 간혹 분류 같으로 테이블을 구분하는 형태를 취하는 경우가 있는데 개발할때 수정없이 분류값만 바꾸면서 되서 편하나 추후 각각의 목적에 따른 별개의 요구사항 발생시 서로 관련없는 변경 사항이 들어갈 수 있다.

- [explain](http://www.dontorz.com/bbs/?mode=view&bbsid=study&ctg_cd=sql&bltn_seq=176)

- [show syntax](https://dev.mysql.com/doc/refman/8.0/en/show.html)
