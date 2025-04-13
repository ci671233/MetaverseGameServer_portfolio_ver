# 메타버스 게임 서버
> **Unity 기반 3D 메타버스 게임과 연동되는 서버**  
> 실시간 로그인 관리, 사용자 간 상호작용, 에셋 관리, 룸 기능을 제공하며, GIN 프레임워크 기반으로 구축됨

## 📝 프로젝트 개요
- 메타버스 게임 서버 백엔드 구현
- GIN(Golang) 기반 RESTful API 구성
- 유니티 프론트엔드와 실시간 연동
- MongoDB / MySQL 혼합 사용
- 컨테이너 환경에서 여러 서버를 Docker Swarm으로 관리
- 요구사항 기반 설계와 컨테이너 계층 빌드로 최적화된 환경 제공

## 요구사항 정의서
| 요구사항 고유번호 | 명칭 | 분류 | 응락 수준 | 세부 내용 |
|------------------|------|------|-----------|-----------|
| TER-001 | Login Server | 테스트 | 필수 | - 사용자 접속 정보 관리 기능<br>- 입력된 사용자 정보 토대로 일치 여부 확인 기능 |
| TER-002 | Map Server | 테스트 | 필수 | - 맵 업로드<br>- 맵 삭제, 조회 기능 |
| TER-003 | Asset Server | 테스트 | 필수 | - 에셋 다운로드 및 조회<br>- 에셋 업로드<br>- 에셋 메타데이터 관리 |
| TER-004 | Game Server | 테스트 | 필수 | - 다중 사용자 로그인 확인<br>- 사용자 간 채팅 및 실시간 정보 업데이트 기능 |  

## 기술 스택
- **Frontend**: Unity 3D
- **Backend**: Golang (GIN Framework)
- **Database**: MongoDB, MySQL
- **Infra**: Docker, Docker Swarm

## 시스템 구조도
- 메타버스 게임 서버
  <img width="600" alt="image" src="https://github.com/user-attachments/assets/d0dd79b8-6f3a-47e8-be18-909cea1efb96" />

- DB 스키마
  <img width="530" alt="image" src="https://github.com/user-attachments/assets/171783a3-fd93-4875-9d24-908b0f31ad80" />

- 운영 모델 전략
  <img width="551" alt="image" src="https://github.com/user-attachments/assets/b3695224-5459-49ed-ab84-b70b41adff96" />

## 결과물
- UI
  - Login
    <img width="514" alt="image" src="https://github.com/user-attachments/assets/b67c25f7-fa52-4e8a-b9fb-fd91c56a50a9" />
  
  - Map
    <img width="547" alt="image" src="https://github.com/user-attachments/assets/7096e25e-40df-4a26-a006-560e789fc41a" />
  
  - Player
    <img width="583" alt="image" src="https://github.com/user-attachments/assets/74e23cc6-a8ec-4a7b-96fd-21818bfb3af0" />

- Server
  - Login
    <img width="468" alt="image" src="https://github.com/user-attachments/assets/8fa0f2c6-21b4-403b-80b7-a29e44963ab3" />
  - Map
    <img width="739" alt="image" src="https://github.com/user-attachments/assets/cd0ff056-767c-4a0d-9c9e-4caf66fac26c" />
  - Asset
    <img width="739" alt="image" src="https://github.com/user-attachments/assets/5d7274ba-7d4c-4093-ba57-168b8c6fba4e" />
    <img width="739" alt="image" src="https://github.com/user-attachments/assets/4802994e-80cb-4807-a868-de131e57cdf8" />
  - Docker
    <img width="686" alt="image" src="https://github.com/user-attachments/assets/92a59c91-819e-4164-9c3b-f561e8cb1550" />

