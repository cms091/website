# Website 소개
국제와인박람회를 주제로 한 웹사이트. 

박람회 일정 제공 및 관련 정보 제공, 티켓 판매 등 고객들을 위한 정보 및 사전예약 서비스 제공이 주가 되는 사이트입니다. 

# 배포 링크
https://cms091.github.io/website/

# 구현 기능 
- 네비게이션, 일정, 프로그램, 위치, 갤러리 등등으로 구성된 메인 페이지 구현
- 로그인 , 회원가입 화면 구현(데이터 연동 기능X, 화면만)
- 로그인 여부에 따라서 접속 가능한 페이지 분리 및 일부 화면 변동
- 와인박람회 부스 신청, 관람객 사전예매, 바이어 사전예매 할 수 있는 폼 서브 페이지 구현


# 디자인 구상
## `피그마`
### 데스크톱 버전(기본)
<img width="1025" height="751" alt="image" src="https://github.com/user-attachments/assets/7b312ff3-faff-4bbb-a0f0-33160b4624f3" />

### 모바일 버전(반응형)
<img width="308" height="650" alt="image" src="https://github.com/user-attachments/assets/d35ef679-5cff-40bf-85d8-de80ecf8cdeb" />

## `와이어프레임`
![와이어프레임](https://github.com/user-attachments/assets/109ebd37-b595-4705-9c3c-65d3155150bf)


## 메인 페이지 🎨 디자인 vs 구현 비교

| 디자인 (Figma) | 구현 화면       |
|-----------------|----------------|
|<img width="400" height="250" alt="image" src="https://github.com/user-attachments/assets/7b312ff3-faff-4bbb-a0f0-33160b4624f3" /> |<img width="400" height="250" alt="image" src="https://github.com/user-attachments/assets/0282ee3b-e7ec-4ec8-a154-df8af32ce6d4" /> |
|<img width="150" height="300" alt="image" src="https://github.com/user-attachments/assets/d35ef679-5cff-40bf-85d8-de80ecf8cdeb" />          |      <img width="150" height="300" alt="image" src="https://github.com/user-attachments/assets/b4bbd307-b697-4a63-a568-f5cc956779e9" /> |


# 전체 페이지 구조 및 화면
```
📦website(root)
 ┣ 📂css(스타일)
 ┃ ┣ 📜index.css
 ┃ ┣ 📜join.css
 ┃ ┣ 📜login.css
 ┃ ┣ 📜pre.css
 ┃ ┗ 📜pre2.css
 ┣ 📂icon(아이콘)
 ┃ ┣ 📜cancel_close_delete_exit_logout_remove_x_icon_123217.png
 ┃ ┣ 📜Check.svg
 ┃ ┣ 📜check_3991408.png
 ┃ ┣ 📜msection01_visual_obj.svg
 ┃ ┣ 📜stop_545666.png
 ┃ ┣ 📜unCheck.svg
 ┃ ┗ 📜wine_4698216.png
 ┣ 📂img(이미지)
 ┃ ┣ 📜agreement-2548138_1280.jpg
 ┃ ┣ 📜albert-vincent-wu-Day9Xhsx6gA-unsplash.jpg
 ┃ ┣ 📜australia-3857041_1280.jpg
 ┃ ┣ 📜javier-balseiro-jDU4yYk5Kgs-unsplash.jpg
 ┃ ┣ 📜mathilde-langevin-IZB7W07TvxQ-unsplash.jpg
 ┃ ┣ 📜picnic-1853380_1280.jpg
 ┃ ┣ 📜popup.png
 ┃ ┣ 📜two-types-of-wine-2466267_1280.jpg
 ┃ ┣ 📜Untitled-1.png
 ┃ ┣ 📜viktoriya-lissachenko-OZujH2Cv_As-unsplash.png
 ┃ ┗ 📜wine-2773374_1280.jpg
 ┣ 📂spon(로고)
 ┃ ┣ 📜basketball-logo-4659385_640.png
 ┃ ┣ 📜coffee-307147_640.png
 ┃ ┣ 📜farm-7098017_640.png
 ┃ ┣ 📜logo-2067396_1280.png
 ┃ ┣ 📜public-domain-vectors-6vXuamI0WRY-unsplash.png
 ┃ ┣ 📜public-domain-vectors-dFUC0agUgKM-unsplash.png
 ┃ ┣ 📜round-icons-u1tMOgFxoqI-unsplash.png
 ┃ ┗ 📜round-icons-zunivDntgTM-unsplash.png
 ┣ 📂video(비디오)
 ┃ ┣ 📜3136626-hd_1920_1080_30fps.mp4
 ┃ ┣ 📜3189297-hd_1080_1920_25fps.mp4
 ┃ ┣ 📜3197862-hd_1920_1080_25fps.mp4
 ┃ ┣ 📜4667126-uhd_2160_4096_25fps.mp4
 ┃ ┣ 📜4694345-sd_338_640_25fps.mp4
 ┃ ┗ 📜81170-575216182_small.mp4
 ┣ 📜index.html(홈)
 ┣ 📜join.html(회원가입)
 ┣ 📜login.html(로그인)
 ┣ 📜pre.html(관람객 사전예약)
 ┣ 📜pre1.html(업자 부스 신청)
 ┗ 📜pre2.html(바이어 사전예약)
```
<img width="639" height="671" alt="image" src="https://github.com/user-attachments/assets/d5f2e41b-e06b-445a-9e01-4fc07e5e4c6f" />
<img width="500" height="219" alt="image" src="https://github.com/user-attachments/assets/fedc4cf7-ddf2-43e1-9a83-fe4fb645fcd4" />
<img width="497" height="270" alt="image" src="https://github.com/user-attachments/assets/a4f8d93d-bb7d-4719-8679-b5f3a7c4a9a4" />
<img width="500" height="778" alt="image" src="https://github.com/user-attachments/assets/25243f65-4532-430e-8dc7-b904ad092847" />
<img width="496" height="570" alt="image" src="https://github.com/user-attachments/assets/0b7651ac-883e-4e28-953a-6631b7ff5c2b" />
<img width="499" height="665" alt="image" src="https://github.com/user-attachments/assets/7227ad14-21c1-4820-b9c5-18747029f030" />


# 사용한 외부 링크 및 사이트
- https://unsplash.com/ko (이미지)
- https://pixabay.com/ko/ (이미지)
- https://getbootstrap.com/ (html/css 템플릿)
- https://www.miricanvas.com/templates (html/ 이미지 템플릿)
- https://kr.freepik.com/icons (아이콘)
