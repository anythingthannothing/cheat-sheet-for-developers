## 특정 port 번호 죽이기(ex. localhost:3000)
### 1. sudo netstat -lpn |grep :3000 ➡ 3000번 포트를 사용 중인 프로세스 찾기
### 2. tcp6 0 0 :::3000 :::* LISTEN **4920**/node ➡ PID 4920에서 3000번 포트 사용 중
### 3. kill -9 4920 ➡ PID 4920을 kill하여 포트 3000번 해방 
<br>
