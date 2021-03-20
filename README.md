# Docker
- 기존 방식대로 그냥 프로그램을 설치할 때, 갖고 있는 서버, 패키지 버전, OS에 따라 설치 과정중 많은 에러들이 발생하고 설치 과정이 복잡함

### 기존 다운로드 방식
```
$ wget http://download.redis.io/releases/redis-6.0.4.tar.gz
$ tar xzf redis-6.0.4.tar.gz
$ cd redis-6.0.4
$ make
```
- wget이 없다면 에러가 발생
- 돌아가서 wget도 다운로드 받아야 함.

### 도커를 이용한 다운로드 방식
```
$ docker run -it redis
```
- 도커가 없어도 다운로드를 할 수는 있지만 프로그램 설치를 하는 도중, 예상치 못한 에러가 발생할 수도 있고 설치 과정이 복잡함.