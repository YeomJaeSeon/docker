# 1. node 설치
FROM node:12
# 누군가 이미 linux환경에서 node를 설치한 이미지를 만들어놨음 그거사용하면 아래 처럼 할 필요없음

# FROM ubuntu:20.04
# RUN apt-get update
# RUN DEBIAN_FRONTEND=noninteractive apt-get install -y nodejs npm

# 2. 소스 복사
COPY . /usr/src/app

# 3. Nodejs 패키지 설치
WORKDIR /usr/src/app
RUN npm install

# 4. WEB 서버 실행 (Listen 포트 정의)
EXPOSE 3000
CMD node app.js