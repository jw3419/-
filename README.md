## 1. Intro

![](https://user-images.githubusercontent.com/68436925/108617755-35998980-745c-11eb-9c1d-4832f3438f6a.png)

<br>

> **프로젝트 명 :** Smart Airport Web Application

> **프로젝트 형태 :** 졸업생 프로젝트

<br>

## 2. Team Member
--- 

## Role 🧑🏼‍💻

<details>
<summary>이재원 [Team Leader]</summary>

- #### Position: `알고리즘 개발`

- #### Stack: `Python`

#### [데이터 분석]

- 데이터 정의 및 전처리
- 데이터 차원 축소
- 

#### [서버 & 배포]

- API 개발
  - 게시판과 댓글 생성, 읽기, 수정, 삭제
  - 페스티벌 참석자 명단 생성, 읽기, 삭제
  - 페스티벌 카테고리 렌더링
  - Google Oauth
- AWS EC2 상의 공동 작업 공간 : Jupyter Notebook 환경 구축
- Nginx 프록시 서버 환경 설정
- Docker를 사용하여 EC2에 배포
- 프록시 서버와 도커 컨테이너 연결

<br></br>

</details>

<details>
<summary>박정환 [Team Member]</summary>

- #### Position: `Front-End`

- #### Stack: `React`, `React-Hooks`, `Redux`, `Redux-saga`, `TypeScript`, `Styled-components`

#### [공통 작업]

- 레퍼런스 조사
- Design
  - 와이어-프레임
  - 플로우차트
  - DB 스키마
  - API

#### [클라이언트]
- Fessport CI
- Deployment
  - HTTPS 환경 배포 (AWS S3 & Route53 & Cloudfront)
- Navigation bar 
  - 반응형 디자인 및 슬라이드 버튼 구현
- 로그인, 회원가입
  - Modal 창을 통해 구현
  - React-spring - 모달 애니메이션
- 동행 페이지
  - 페스티벌 별 게시판 필터링
  - Companion (동행)
  - 코멘트 기능
  - 반응형 디자인 
- 사고 팔기 페이지 
  - 페스티벌 별 게시판 필터링
  - 코멘트  기능
  - 반응형 디자인 
- 리뷰 페이지
  - 키보드 이벤트 - 모달창내에 이미지 선택
  - 반응형 디자인 
- 포스팅 페이지
  - 페스티벌 별 카테고리 선택 작성
- Redux-saga Business logic 
  - 게시판 saga
  - 코멘트 saga
  - Sign in & out & up saga
  - 동행 saga

</details>

<details>
<summary>이종혁 [Team Member]</summary>

- #### Position: `Front-End`

- #### Stack: `React`, `React-Hooks`, `Redux`, `Redux-saga`, `TypeScript`, `Styled-components`

#### [공통 작업]

- 레퍼런스 조사
- 설계
  - 와이어 프레임
  - 플로우 차트
  - DB 스키마
  - API

#### [클라이언트]

- 프론트엔드 사이드 개발 환경 구축
  - Typescript & React
  - ESLint & Prettier
- Redux-saga 비즈니스 로직 구축
  - category, userInfo, image upload 등…
  - map, festival, artist, wish and like 등…
- Main Page
  - 반응형 메인 지도 설계 및 구현
  - 포스터 모달 구현
- Festival and Artist List Page
  - 리스트 비즈니스 로직 및 출력
  - 카테고리 및 필터링, 검색 기능 구현
  - 반응형 웹 디자인
- Festival and Artist Detail Page
  - 디테일 정보 비즈니스 로직 및 출력
  - 'like' & 'visit' 버튼 기능
  - 콘텐츠 슬라이더, 비디오 플레이 모달, 타 DB 테이블 연결
- Fessport Page
  - 이미지 업로드 및 회원정보 수정
  - 'Collector visit' 스탬프 구현
  - 'Badge challenge' 구현
- Wish List Page
  - 페스티벌 & 아티스트 ‘like’ 리스트 출력


</details>

<details>
<summary>강희석 [Team Member]</summary>

- #### Position: `Back-End`

- #### Stack: `Node.js`, `Express`, `TypeScript`, `MongoDB`, `Mongoose`, `Nginx`, `Docker`

#### [공통 작업]

- 레퍼런스 조사
- 디자인
  - wire-frame
  - flow-chart
  - DB Schema
  - API
  - DB models using mongoDB and mongoose

#### [서버]

- 메인 MAP 나라 별 페스티별 API
- 페스티벌 및 아티스트 리스트, 상세 페이지
- 페스티벌 및 아티스트 좋아요 및 취소 기능
- 페스티벌 방문 API
- 사용자 뱃지 획득 기능 API
- 회원가입 / 로그인 / 로그아웃 / Kakao Oauth 기능
- 마이페이지
  - 사용자 정보 요청(토큰) 페이지 및 수정 API
  - 내가 쓴 글 기능

</details>

--- 

## 3. Project

### 🎈 Smart Airport가 무엇인가요?

Smart Airport는 공항 내의 시설을 추천해주는 서비스입니다.

인공지능을 통해 사용자가 선택한 시설과 유사한 시설들을 추천하여,<br>
인천공항내에 다양한 시설들을 폭 넓게 이용할 수 있도록 도움을 주는 웹 어플리케이션입니다.<br>

<br>

### 🎈 Flow Chart
**1. 비행기 편명 입력:** <br>
탑승마감 시간까지 남은 시간을 계산하고, 게이트 위치정보를 수집한다.
![그림1](https://user-images.githubusercontent.com/68436925/108619546-ec9c0200-7468-11eb-931f-50147f41202a.png)

<br>

**2. 이용 시설 입력:** <br>
자신이 이용할 시설을 입력한다.
![그림2](https://user-images.githubusercontent.com/68436925/108620533-19074c80-7470-11eb-8c8f-9c31fd08eb21.png)

<br>

**3. 추천 시설 안내:** <br>
추천한 시설의 경로를 안내한다.
![그림3](https://user-images.githubusercontent.com/68436925/108620643-d42fe580-7470-11eb-8097-8e016f7ddd2a.png)

<br>

**4. 탑승 알림:** <br>
비행기 탑승 마감 시간이 임박하면, 사용자에게 알림을 보낸다.
![그림4](https://user-images.githubusercontent.com/68436925/108620569-494eeb00-7470-11eb-9761-f89b6111dc6b.png)


### 🎈 Smart Airport는 이렇게 만들어졌습니다!


