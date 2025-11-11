# International Wine Expo Website

## 웹사이트 소개
국제 와인 박람회를 주제로 한 웹사이트입니다.  
방문객은 박람회 일정, 프로그램, 위치 정보를 확인하고, 티켓을 사전 예약할 수 있으며, 부스 신청도 가능합니다.  

**주요 목적:**  
- 방문객에게 박람회 정보를 제공  
- 사전 예약 및 부스 신청 기능 제공 (UI 구현만)  

---

## 배포 링크
[GitHub Pages 링크](https://cms091.github.io/website/)  

---

## 기술 스택
- HTML / CSS / JavaScript 활용

---

## 구현 기능

| 기능 | 구현 여부 | 비고 |
|------|----------|------|
| 메인 페이지 (네비게이션, 일정, 프로그램, 위치, 갤러리) | 구현 | 디자인 기반 |
| 로그인 화면 | 구현 | 실제 서버X 로컬 스토리지로 UI만 구현 |
| 회원가입 화면 | 구현 | 실제 서버X 로컬 스토리지로 UI만 구현|
| 로그인 여부에 따른 페이지 접근 제한 | 구현 | UI/화면만 변경 |
| 와인 박람회 부스 신청 | 구현 | 폼 UI |
| 관람객 사전 예약 | 구현 | 폼 UI |
| 바이어 사전 예약 | 구현 | 폼 UI |

---

## 디자인 구상

### 피그마
- **데스크톱 버전**
![데스크톱 디자인](https://github.com/user-attachments/assets/7b312ff3-faff-4bbb-a0f0-33160b4624f3)

- **모바일 버전 (반응형)**
![모바일 디자인](https://github.com/user-attachments/assets/d35ef679-5cff-40bf-85d8-de80ecf8cdeb)

### 와이어프레임
![와이어프레임](https://github.com/user-attachments/assets/109ebd37-b595-4705-9c3c-65d3155150bf)

---

## 메인 페이지: 디자인 vs 구현

| 디자인 (Figma) | 구현 화면 |
|----------------|-----------|
|![디자인](https://github.com/user-attachments/assets/7b312ff3-faff-4bbb-a0f0-33160b4624f3) | ![구현](https://github.com/user-attachments/assets/0282ee3b-e7ec-4ec8-a154-df8af32ce6d4) |

> 주요 구현 사항: 반응형 레이아웃, 이미지/비디오 슬라이더, 폼 UI  

---

## 전체 페이지 구조
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

> 페이지 설명:  
- `index.html`: 메인 페이지  
- `join.html`: 회원가입 UI  
- `login.html`: 로그인 UI  
- `pre.html`: 관람객 사전 예약 폼  
- `pre1.html`: 부스 신청 폼  
- `pre2.html`: 바이어 사전 예약 폼
  
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/d5f2e41b-e06b-445a-9e01-4fc07e5e4c6f" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/fedc4cf7-ddf2-43e1-9a83-fe4fb645fcd4" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/a4f8d93d-bb7d-4719-8679-b5f3a7c4a9a4" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/25243f65-4532-430e-8dc7-b904ad092847" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/0b7651ac-883e-4e28-953a-6631b7ff5c2b" />
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/7227ad14-21c1-4820-b9c5-18747029f030" />

---

## 외부 리소스


|   이미지 |  템플릿  |  아이콘  | 
|---------|----------|---------|
| [Unsplash](https://unsplash.com/ko), [Pixabay](https://pixabay.com/ko/)  | [Bootstrap](https://getbootstrap.com/),[Miricanvas](https://www.miricanvas.com/templates)  | [Freepik](https://kr.freepik.com/icons)  |

---
