# Docker CLI
## 1. Auth
### docker login ➡ 도커 허브에 로그인(ID & PW)
### docker logout ➡ 도커 허브 계정 로그아웃
### docker push {userId/imageName:tag} ➡ 도커 허브에 이미지 푸쉬
### docker pull {userId/imageName:tag} ➡ 도커 허브에서 이미지 풀

<br>

## 2. Image
### docker build . ➡ 현재 폴더의 Dockerfile을 기반으로 이미지 빌드
#### -t ➡ 이미지 이름과 tag를 설정
### docker images ➡ 로컬에 저장된 모든 이미지 목록 표시
### docker rmi {image} ➡ ID 또는 이름으로 이미지 삭제

<br>

## 3. Container
### docker run {imageName:tag} ➡ 이미지를 기반으로 컨테이너 실행
#### --name {containerName} ➡ 컨테이너의 이름을 직접 지정
#### -it ➡ 인터렉티브 tty 모드로 진입
#### --rm ➡ 컨테이너 중지 시 자동으로 삭제
#### -d ➡ detached 모드로 시작
### docker ps ➡ 실행 중인 컨테이너 리스트 표시
#### -a ➡ 중지된 컨테이너까지 표시

<br>

## 이미지 및 컨테이너 모두 삭제
### docker stop $(docker ps -a -q)
### docker rm $(docker ps -a -q)
### docker rmi -f $(docker images -q)

## 정지된 컨테이너, 실행 중인 컨테이너 이미지 외의 이미지, 볼륨, 네트워크 삭제
### docker system prune

<br>
