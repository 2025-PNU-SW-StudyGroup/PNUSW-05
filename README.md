# 🚀 햄북 Stock 📈

> **PNU SW학습공동체 프로젝트** - 모의 주식 투자 플랫폼

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115.8-green.svg)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-18.2.0-blue.svg)](https://reactjs.org/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0+-orange.svg)](https://mysql.com/)
[![Redis](https://img.shields.io/badge/Redis-5.2.1-red.svg)](https://redis.io/)

## 📖 프로젝트 소개

**햄북 Stock**는 실제 주식 투자의 진입 장벽이 높아 실제 돈으로 선뜻 발을 딛기 어려운 사람들을 위해 개발된 모의 주식 투자 플랫폼입니다.

### 🎯 주요 특징
- 💰 **안전한 모의 투자**: 가상 머니로 위험 없이 주식 투자 체험
- 📊 **실시간 거래**: 실시간 매수/매도 및 가격 변동 시스템
- 📰 **뉴스 피드**: 매일경제 기사 크롤링 및 AI 요약
- 💬 **실시간 채팅**: 웹소켓 기반 익명 채팅방
- 🏆 **랭킹 시스템**: 수익률 기반 유저 랭킹 (명예의 전당)
- 🎨 **개인화**: 나만의 주식 상장 시스템

---

## 🛠 기술 스택

### Frontend
- **React 18.2.0** - 사용자 인터페이스
- **Axios** - HTTP 클라이언트
- **React Router DOM** - 라우팅
- **Recharts** - 차트 시각화
- **Swiper** - 슬라이더 컴포넌트

### Backend
- **FastAPI** - 고성능 웹 프레임워크
- **SQLAlchemy** - ORM
- **PyJWT** - JWT 인증
- **Redis** - 캐싱 및 세션 관리
- **OpenAI API** - 뉴스 요약
- **WebSocket** - 실시간 통신

### Database
- **MySQL** - 메인 데이터베이스
- **Redis** - 캐싱 및 세션 저장소

---

## 🚀 빠른 시작

### 1. 저장소 클론
```bash
git clone https://github.com/your-username/hambook-stocks.git
cd hambook-stocks
```

### 2. 백엔드 설정
```bash
# 가상환경 생성 및 활성화
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# 의존성 설치
pip install -r requirements.txt

# 환경 변수 설정
cp .env.example .env
# .env 파일에서 데이터베이스 설정 및 API 키 입력

# 서버 실행
uvicorn main:app --reload
```

### 3. 프론트엔드 설정
```bash
cd front-react
yarn install
yarn start
```

### 4. 데이터베이스 설정
```sql
-- MySQL 데이터베이스 생성
CREATE DATABASE hambook_stocks;
```

---

## 📁 프로젝트 구조

```
hambookstocks.v2/
├── app/                          # 백엔드 애플리케이션
│   ├── dependencies/             # 데이터베이스, JWT, Redis 설정
│   ├── models/                   # 데이터베이스 모델
│   ├── routers/                  # API 라우터
│   └── services/                 # 비즈니스 로직
├── front-react/                  # React 프론트엔드
│   ├── src/
│   │   ├── components/           # React 컴포넌트
│   │   ├── services/             # API 서비스
│   │   └── styles/               # CSS 스타일
│   └── public/                   # 정적 파일
├── front/                        # 기존 HTML/CSS/JS 프론트엔드
└── front2/                       # 대시보드 스타일 프론트엔드
```

---

## 🔧 주요 기능

### 📈 주식 거래 시스템
- 실시간 매수/매도 기능
- 가격 변동 알고리즘 (alpha = 0.1)
- 거래 내역 추적 및 관리

### 📰 뉴스 시스템
- 매일경제 기사 자동 크롤링
- OpenAI GPT를 활용한 기사 요약
- 실시간 뉴스 피드 제공

### 💬 채팅 시스템
- WebSocket 기반 실시간 채팅
- 로그인/비로그인 사용자 모두 참여 가능
- 익명 채팅 기능

### 👤 사용자 관리
- JWT 토큰 기반 인증
- Redis를 활용한 세션 관리
- 개인 주식 포트폴리오 관리

---

## 👥 팀원

| 이름 | 역할 | 담당 분야 |
|------|------|-----------|
| 하승원 | Frontend 개발 | React 기반 사용자 인터페이스 개발 |
| 김민찬 | Backend 개발 | FastAPI 기반 API 개발, 데이터베이스 설계 |
| 노현민 | 기획 | 프로젝트 기획 및 요구사항 분석 |
| 김다영 | 디자인 | UX/UI 디자인 및 사용자 경험 설계 |

---

## 📊 개발 진행 상황

### ✅ 완료된 기능
- [x] React 기반 웹 구조 세팅
- [x] JWT 토큰 처리 및 Redis 도입
- [x] MySQL 데이터베이스 전환
- [x] 회원가입, 로그인, 로그아웃 로직
- [x] 매일경제 기사 크롤링
- [x] OpenAI API를 활용한 뉴스 요약
- [x] 실시간 채팅 기능
- [x] 매수/매도 가격 변동 기능
- [x] MyPage 기능 구현
- [x] LOGO DESIGN 및 웹 컴포넌트 구조 디자인
- [x] 주식 거래 로직 및 게임 기능 설계
- [x] 사용자 맞춤형 기능 강화

### 🔄 진행 중인 기능

---

## 📞 문의

프로젝트에 대한 문의사항이 있으시면 이슈를 생성해 주세요.

---

**© 2025 햄북 Stock Team** | PNU SW학습공동체 프로젝트
