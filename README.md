# Socket_Mini_Project
## 시현 영상
![ezgif com-video-to-gif-chat](https://github.com/jayoung977/Socket_Mini_Project/assets/61008837/7a15b0d6-23a4-4e8b-9204-752d83adcb00)


## :star: 서비스 소개  
- **채팅 + 게시판 + 로그인 가능한 익명 채팅 서비스**


## :open_file_folder: 주요 기능
- **Socket.IO를 사용한 채팅 애플리케이션.**
- **Session을 이용하여 로그인 기능 구현**
- **REST API를 이용한 게시판 기능 구현**

## :globe_with_meridians: AWS 배포링크
http://3.106.52.247:8001/

## :white_check_mark:프로젝트 구동 방법 
```
git clone https://github.com/jayoung977/Socket_Mini_Project.git
cd server
node app.js
```
```
cd client
sudo vi /etc/nginx/sites-available/Socket_Mini_Project.conf
```
```
#편집기 입력
server { 
        listen 80; 
        location / { 
                root /home/ubuntu/Socket_Mini_Project/client/build; 
                index index.html index.htm; 
                try_files $uri /index.html; 
        } 
}
```

```
sudo ln -s /etc/nginx/sites-available/Socket_Mini_Project.conf /etc/nginx/sites-enabled/Socket_Mini_Project.conf
sudo systemctl stop nginx
sudo systemctl start nginx 
sudo systemctl status nginx 
```

## :sparkles: 개인 미니채팅프로젝트 2등 수상
[포스코X코딩온 개인 미니채팅프로젝트 2등.pdf](https://drive.google.com/uc?id=140lhHDWKyMpPotn94wMMRlUY9jaOmeq8)

