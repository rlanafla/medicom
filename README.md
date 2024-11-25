# 메디콤
![logo (1)](https://github.com/user-attachments/assets/74c152e2-6fcb-41e8-97a8-796b0b2b2376)

#### 원인 모를 통증과 증상을 입력하면  의심되는 질병을 알려주고,
#### 어떤 진료과를 가야하는지와 근처에 있는 해당 진료과 병원까지 바로 찾아주는 시스템


## 배포 사이트
#### https://34.64.103.17/

### 관리자 로그인
#### 이메일 : admin@admin.com
#### 비밀번호 : 4444


## 기술 스택

### 백엔드
- SpringBoot
- Spring Data JPA
- Spring Security
- MySQL
- JWT
- Gemini API

### 프론트엔드
- React
- Nginx
- Axios
- MUI
- Firebase API
- Naver Map API

### 배포
- GCP
- Gitlab CI/CD

## ERD 및 와이어프레임
### ERD
![erd (1)](https://github.com/user-attachments/assets/71975e7a-f2b2-4d5c-8438-e6236059f9dc)

### 와이어 프레임
https://www.figma.com/design/GX6CyJdzJCfZVgUN4t9mZd/elice-project3?node-id=0-1&t=8cqv2TCWyLXtmpu7-0

## 기능

### 메인 기능
- 도로명주소API와 네이버 Geocoding API, ReverseGeocoding API를 통한 현재 위치 자동 설정, 검색 설정
- GEMINI API 연동을 통한 질의를 통해 사용자 질병 간단한 진단 및 진료과 소개 
- 해당 진료과가 존재하는 근처 병원(5km 반경) 검색 및 지도에 표시
- 유행중인 질병 확인
- 현재 위치 기반으로 주변 병원 일반 검색
- 진료과 기반 필터링
- 병원 예약
- 병원 방문 리뷰
- 병원 즐겨찾기 설정

### 유저
- 일반 회원가입 (가입 시 이메일 인증, 아이디 비밀번호 찾기, 비밀번호 기억하기)
- Oauth2를 사용한 소셜 로그인 기능(NAVER, GOOGLE)
- 로그인 시 Access Token, Refresh Token 발급
- Access Token 만료 시 Access Token, Refresh Token 모두 재발급
- 일반 유저, 의사, 관리자 총 3가지 Role
- 관리자는 유저 관리(삭제, 권한 관리) 가능
- 회원정보 수정 및 회원탈퇴
- 

### 게시판
- 공지사항을 통해 유저들에게 주요 사항 공지
- 게시글 조회수
- 게시글 추천
- 게시글 정렬(최신, 추천, 조회)
- 게시글 수정 및 삭제
- 댓글 및 대댓글

### 채팅
- 유저는 의사와 1:1 채팅을 통해 간편 원격 진단 및 진료과 소개
- 의사에게 소개받은 진료과를 통해 빠르게 근처의 해당 진료과 병원 검색
- 유저는 관리자와 1:1 채팅을 통해 문의 가능
- 의사는 진단 신청 대기중인 채팅방 확인 및 채팅 수락
- 관리자는 문의 대기중인 채팅방 확인 및 채팅 수락
- 고객센터 문의 채팅
