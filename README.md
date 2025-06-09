1단계] 요구사항 정의서
🔹기능 정리
식당 목록 페이지

식당 상세 페이지

주소, 운영시간, 설명, 대표 사진

리뷰 목록, 리뷰 작성 버튼

지도 표시 (네이버 지도)

예약 버튼 (네이버 예약 링크 연결)

리뷰 작성 페이지

작성자, 평점, 내용, 날짜 입력

로그인/회원가입 페이지

간단한 localStorage 인증 가능

공통 UI

헤더, 검색창, 카테고리 필터 등

🔹비기능 요구사항
HTML + JS로 UI

Spring Boot로 서버 (회원정보, 리뷰 DB)

  GitHub 저장소 연동 및 커밋 관리

  네이버 지도 API 사용

  네이버 예약 링크 연결

[2단계] 시스템 설계 (화면 + DB + 기술 스택)
🔹화면 구성도
home.html – 검색 & 카테고리

restaurantlist.html – 식당 리스트

restaurantdetail.html – 식당 정보 + 리뷰 + 지도 + 예약

reviewwrite.html – 리뷰 작성

review.html – 작성된 리뷰 보기

login.html, signup.html – 인증 기능

🔹기술 스택
영역	기술
프론트	HTML, CSS, JavaScript (기초 Vanilla JS)
백엔드	Spring Boot (Java), MySQL or H2
배포	GitHub Pages + Render or EC2
버전관리	GitHub, 커밋 단위 명확히
지도	네이버 지도 API
예약	외부 네이버 예약 링크 연결

ERD 예시
User(id, username, password)
Restaurant(id, name, location, description, category)
Review(id, user_id, restaurant_id, rate, content, date)

