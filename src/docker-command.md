## 이미지 및 컨테이너 모두 삭제
### docker stop $(docker ps -a -q)
### docker rm $(docker ps -a -q)
### docker rmi -f $(docker images -q)

## 정지된 컨테이너, 실행 중인 컨테이너 이미지 외의 이미지, 볼륨, 네트워크 삭제
### docker system prune
<br>
