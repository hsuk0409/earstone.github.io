---
layout: single
title: ""
permalink: /resume/
author_profile: true
sidebar:
  nav: "docs"
---

# 최 현 석 (Choi Hyeon-suk)
**Email:** hsuk0409@gmail.com

---

## Introduction
- Antigravity 기반의 에이전틱 워크플로우를 통해 복잡한 비즈니스 로직을 효율적으로 설계하고 구현합니다.
- 6년의 서버 개발 경험을 바탕으로 도메인 중심 설계(DDD)와 포트-어댑터 패턴을 실천합니다.
- 대 AI 시대를 맞아 단순 코딩을 넘어 에이전트와 질문하고 고민하며 함께 성장하는 개발 문화를 지향합니다.

---

## Featured Projects

### 1. 시니어 케어: 노인 낙상 관리 앱 (Android)
- **핵심 기술:** Kotlin, Accelerometer Sensor, Foreground Service, Broadcast Receiver, SMS Manager, Google Maps API
- **설명:** 고도화된 3단계 낙상 감지 알고리즘을 통한 자동 긴급 구조 서비스입니다.
- **상세 내용:** 
  - **3단계 센서 데이터 검증:** 자유낙하(3.5 m/s² 이하) -> 충격(55.0 m/s² 이상) -> 정지(1.5초간 움직임 없음)의 3단계 로직을 통해 일상적인 움직임과 실제 낙상을 정밀하게 구분하여 오탐율을 최소화했습니다.
  - **무중단 보호 시스템:** Foreground Service와 Wake-Lock을 활용하여 화면이 꺼진 상태에서도 끊김 없는 모니터링을 보장하며, BootReceiver를 통해 기기 재부팅 시에도 실시간 감지 서비스가 자동 실행되도록 구현했습니다.
  - **자동 긴급 구조 워크플로우:** 낙상 감지 시 자동으로 화면을 점등하고 30초 카운트다운을 시작합니다. 사용자 응답이 없을 경우 GPS 기반 실시간 위치 정보와 Google Maps 링크가 포함된 SOS 문자를 보호자에게 자동 발송합니다.
- **GitHub:** [https://github.com/hsuk0409/Elderly-Fall-Guard](https://github.com/hsuk0409/Elderly-Fall-Guard)

### 2. 위치 기반 음성 메모 앱 (진행중)
- **핵심 기술:** React Native, NestJS, PostgreSQL, Docker, Webhook
- **설명:** 사용자 위치를 기반으로 음성 메모를 저장하고 관리하는 지능형 리마인더 서비스입니다.
- **상세 내용:** 
  - 특정 장소에서 잊기 쉬운 할 일이나 기록을 음성으로 즉시 저장합니다.
  - 사용자가 해당 지점 반경 n미터 이내로 진입하면, 해당 위치와 관련된 모든 메모를 자동으로 한곳에 모아 사용자에게 인지시켜 줍니다.
  - 복잡한 일상 속에서 위치 기반 트리거를 통해 중요한 정보를 놓치지 않도록 돕는 것을 목표로 합니다.
- **GitHub:** [https://github.com/hsuk0409/voice-geo-memo](https://github.com/hsuk0409/voice-geo-memo)

---

## Work Experience

### **피에스에듀홀딩스** (2024.05 - 현재)
*서버 개발자 / 정규직*

- **공유기 포트포워딩 자동 설정 기술 개발 (2026.02)**
  - Go 언어의 UPnP 기술을 활용하여 유동 IP 환경에서 원격 포트포워딩 설정 자동화.
  - 전용 웹 서비스 제공을 통해 각 학원 지점에서 필요한 설정을 원클릭으로 처리할 수 있도록 구현.
- **학원 관리 프로그램 개발 및 서버 구축 (2025.03 - 2026.03)**
  - NestJS, Docker, MariaDB 기반 리눅스 환경 구축 및 관리.
  - Gemini(CLI)를 활용한 에이전틱 개발 프로세스 도입으로 생산성 향상.
  - 포트-어댑터 패턴 및 도메인 모델 중심 아키텍처 도입.

### **지오아이티** (2023.06 - 2024.02)
*백엔드 개발자 / 정규직*

- **웹소켓 기반 라이딩 앱 서버 개발 및 개선 (2023.09 - 2024.01)**
  - Node.js, Websocket, Cassandra 기반 고성능 통신 환경 구축.
  - InnoDB 레코드 잠금 트랜잭션 제어를 사용하여 즐겨찾기 중복 저장 동시성 이슈 해결.
  - 1,000줄 규모의 Stored Procedure를 JavaScript 코드로 리팩토링(500줄)하여 유지보수성 및 안정성 개선.

### **더커머스** (2021.09 - 2023.05)
*서버 개발자 / 정규직*

- **결제 구독권 시스템 개발 및 고도화 (2022.04 - 2022.10)**
  - Java, Spring Boot, MongoDB 기반 시스템 유지보수 및 기능 개선.
  - DTO 활용을 통한 주요 비즈니스 로직 캡슐화 및 테스트 코드 작성.
  - Spring Interceptor 및 Wrapper를 활용하여 요청 바디 스트림 재설정 문제 해결 및 결제 유효성 검증 최적화.
- **오픈마켓 연동 개발 (2021.09 - 2022.03)**
  - 롯데온, 카페24 등 다양한 오픈마켓 OpenAPI 연동(Python, Flask, AWS Lambda).

### **빌리지피플** (2020.03 - 2021.08)
*백엔드 개발자 / 정규직*

- **포인트 자동화 시스템 개발 (2020.11 - 2021.02)**
  - Spring Boot, JPA, Spring Quartz 기반 스케줄러 개발.
  - DDD 기반 적립/차감 로직 설계 및 만료 포인트 자동 회수 시스템 구축.
- **QueryDSL 도입 및 테스트 커버리지 확대**
  - 복잡한 쿼리를 QueryDSL로 전환하여 개발 생산성 및 타입 안정성 확보.
  - 170개 이상의 Junit 테스트 코드 및 Spring Rest Docs 기반 API 문서 자동화 구축.

---

## Technical Skills
- **Languages:** Java, Python, Node.js (JavaScript/TypeScript), Go, PHP
- **Frameworks:** Spring Boot, NestJS, Flask, ExpressJS, Vue.js
- **Infrastructure:** Docker, AWS (Lambda, API Gateway), MySQL, MariaDB, MongoDB, Redis, Linux
- **AI Tools:** Antigravity (Agentic Flow), Gemini, GitHub Copilot

---

## Education
- **단국대학교** (2016.03 - 2019.02) - 운동처방재활학과 학사 졸업
- **경민대학교** (2012.03 - 2016.02) - 레저스포츠과 전문학사 졸업

---

## Awards & Certificates
- **정보처리기사** (2019.08) - 한국산업인력공단
- **2급 생활스포츠지도사(보디빌딩)** (2018.07) - 국민체육진흥공단

---

## Links
- [Tistory Blog](https://earstone.tistory.com/)
- [GitHub](https://github.com/hsuk0409)
