![image](https://user-images.githubusercontent.com/85022962/224867989-8abcc9f9-9b70-4bbd-a1df-c8c8692c4fe1.png)

# 최신버전 
# FROM node:latest

# alpine은 리눅스 파일 최소 단위
FROM node:alpine3.17

WORKDIR /app

COPY package.json package-lock.json./

# ci시 package-lock.json 파일 버전 갖고옴 안정성 맞춰줌
RUN npm ci 

# 자주 변경되는 것 마지막 -> 도커는 레이어 시스템으로 변경 안되는 건 캐시 -> 변경되는 것만 업데이트 작업
COPY index.js .

ENTRYPOINT [ "node" , "index.js" ]
