# mysql
## tips
- 상황 : query를 날렸는데 table lock 걸림 
- 해결 방법 : 문제가 되지 않는 프로세스라면 죽인다... 
```
show processlist;
kill <id>
```
