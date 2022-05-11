# 베이스 이미지
FROM node:alpine
# 해당 어플의 소스코드가 들어갈 디렉토리
WORKDIR /src
# 종속성 목록을 담고 있는 package.json 복사
COPY ./package*.json ./
# package.json에 명시된 종속성 다운
RUN npm install
# 모든 소스코드 WORKDIR 복사
COPY . .
# 컨테이너가 실행될 때 같이 실행할 명령어
CMD ["npm", "run", "start"]