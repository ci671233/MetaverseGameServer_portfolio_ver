
# 메타버스 게임 서버

> **Unity 기반 3D 메타버스 게임과 연동되는 서버**  
> 실시간 로그인 관리, 사용자 간 상호작용, 에셋 관리, 룸 기능을 제공하며, GIN 프레임워크 기반으로 구축됨

---

## 로젝트 개요
- 메타버스 게임 서버 백엔드 구현
- GIN(Golang) 기반 RESTful API 구성
- 유니티 프론트엔드와 실시간 연동
- MongoDB / MySQL 혼합 사용
- 컨테이너 환경에서 여러 서버를 Docker Swarm으로 관리
- 요구사항 기반 설계와 컨테이너 계층 빌드로 최적화된 환경 제공

---

## 요구사항 정의서

| 요구사항 고유번호 | 명칭 | 분류 | 응락 수준 | 세부 내용 |
|------------------|------|------|-----------|-----------|
| TER-001 | Login Server | 테스트 | 필수 | - 사용자 접속 정보 관리 기능<br>- 입력된 사용자 정보 토대로 일치 여부 확인 기능 |
| TER-002 | Map Server | 테스트 | 필수 | - 맵 업로드<br>- 맵 삭제, 조회 기능 |
| TER-003 | Asset Server | 테스트 | 필수 | - 에셋 다운로드 및 조회<br>- 에셋 업로드<br>- 에셋 메타데이터 관리 |
| TER-004 | Game Server | 테스트 | 필수 | - 다중 사용자 로그인 확인<br>- 사용자 간 채팅 및 실시간 정보 업데이트 기능 |  

---

## 🛠️ 기술 스택

- **Frontend**: Unity 3D
- **Backend**: Golang (GIN Framework)
- **Database**: MongoDB, MySQL
- **Infra**: Docker, Docker Swarm

---

## 시스템 구조도

### • 메타버스 게임 서버 구성도  
<img width="600" alt="architecture" src="https://github.com/user-attachments/assets/d0dd79b8-6f3a-47e8-be18-909cea1efb96" />

### • DB 스키마  
<img width="530" alt="db-schema" src="https://github.com/user-attachments/assets/171783a3-fd93-4875-9d24-908b0f31ad80" />

### • 운영 모델 전략  
<img width="551" alt="operation" src="https://github.com/user-attachments/assets/b3695224-5459-49ed-ab84-b70b41adff96" />

---

## 결과물

### • UI 화면

**Login**  
<img width="514" alt="login-ui" src="https://github.com/user-attachments/assets/b67c25f7-fa52-4e8a-b9fb-fd91c56a50a9" />

**Map**  
<img width="547" alt="map-ui" src="https://github.com/user-attachments/assets/7096e25e-40df-4a26-a006-560e789fc41a" />

**Player**  
<img width="583" alt="player-ui" src="https://github.com/user-attachments/assets/74e23cc6-a8ec-4a7b-96fd-21818bfb3af0" />

---

### • Server 실행 화면

**Login Server**  
<img width="468" alt="login-server" src="https://github.com/user-attachments/assets/8fa0f2c6-21b4-403b-80b7-a29e44963ab3" />

**Map Server**  
<img width="739" alt="map-server" src="https://github.com/user-attachments/assets/cd0ff056-767c-4a0d-9c9e-4caf66fac26c" />

**Asset Server**  
<img width="739" alt="asset-server-1" src="https://github.com/user-attachments/assets/5d7274ba-7d4c-4093-ba57-168b8c6fba4e" />
<img width="739" alt="asset-server-2" src="https://github.com/user-attachments/assets/4802994e-80cb-4807-a868-de131e57cdf8" />

**Docker 환경**  
<img width="686" alt="docker" src="https://github.com/user-attachments/assets/92a59c91-819e-4164-9c3b-f561e8cb1550" />

---

## 마무리

- 본 프로젝트는 팀 프로젝트로 진행되었으며 웹 서버 기반 메타버스 게임 입니다.
- 프론트 팀 3명, 백엔드 팀 2명으로 구성되었습니다.
- 저는 Asset Server 개발과 Docker 배포를 담당하였습니다.


