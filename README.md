도커 명령어
## local port 9999 -> docker port 8080 

뒤의 명령어들은 볼륨 설정

### TODO : docker-compose 작업하기 및 도커 포트도 8080 -> 9999 으로 바꾸기

[X]  cron 추가

[]  python version 바꾸기

[] TZ 바꾸기

```
docker run -p 9999:8080 --rm -v $PWD/logs:/logs -v $PWD/notebook:/notebook -e ZEPPELIN_LOG_DIR='/logs' -e ZEPPELIN_NOTEBOOK_DIR='/notebook' --name zeppelin apache/zeppelin:0.9.0
```