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

- **AI 에이전트 협업 전략가**: 단순한 코드 생성을 넘어 에이전트에게 비즈니스 맥락(Context)을 설계하고, 아키텍처적 의사결정을 주도하며 함께 최적의 솔루션을 도출하는 '에이전틱 워크플로우'를 지향합니다.
- **실전적 AI 활용과 검증**: 6년의 백엔드 개발 경험을 토대로 AI의 결과물을 비판적으로 수용하며, 도메인 중심 설계(DDD)와 포트-어댑터 패턴 준수를 통해 지속 가능한 코드 품질을 유지합니다.
- **성장하는 개발 문화**: 대 AI 시대를 맞아 에이전트와 질문하고 고민하며, 기술적 복잡도를 함께 해결해 나가는 동료 지향적 개발 문화를 실천하고 있습니다.

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

_서버 개발자 / 정규직_

- **인프라 아키텍처 개선 및 데브옵스 환경 구축 (2025.11 - 2026.04)**
  - DB 서버 과부하 이슈의 근본 원인 파악 및 쿼리 최적화를 위해 PMM(Percona Monitoring and Management) 기반의 실시간 DB 성능 모니터링 시스템 구축.
  - 기존 로컬 서버 내 이미지 직접 저장 및 DB 바이너리 저장 방식에서 Cloud Object Storage와 CDN 서비스를 활용한 인프라로 전환하여 리소스 제공 효율 및 서버 확장성 확보.
  - Docker 및 GitHub Actions를 활용한 컨테이너 기반 CI/CD 파이프라인을 구축하여 환경 일관성 보장 및 배포 자동화로 개발 생산성 향상.
  - NestJS 환경에 Winston 및 New Relic을 연동하여 중앙 집중형 로깅 및 실시간 모니터링 시스템 구축.
- **학원 관리 프로그램 개발 및 에이전틱 프로세스 고도화 (2025.03 - 현재)**
  - NestJS, Docker, MariaDB 기반 리눅스 환경 구축 및 관리.
  - **에이전틱 워크플로우 도입**: Antigravity 및 Gemini 에이전트를 개발 전 과정에 도입하여 생산성 향상.
  - **고민과 실천**: 에이전트가 단기적인 구현에 매몰되지 않도록 'Session Implementation Plan'을 통해 장기적인 설계 방향성을 제시하고, 생성된 코드의 아키텍처 정합성을 상시 검증하여 기술 부채를 최소화.
  - **지식 자산화**: 에이전트와의 설계 고민 과정을 기록하고 최적의 프롬프트/맥락 관리 기법을 수립하여 협업 효율 극대화.
  - 포트-어댑터 패턴 및 도메인 모델 중심 아키텍처 도입.

### **지오아이티** (2023.06 - 2024.02)

_백엔드 개발자 / 정규직_

- **웹소켓 기반 라이딩 앱 서버 개발 및 개선 (2023.09 - 2024.01)**
  - Node.js, Websocket, Cassandra 기반 고성능 통신 환경 구축.
  - InnoDB 레코드 잠금 트랜잭션 제어를 사용하여 즐겨찾기 중복 저장 동시성 이슈 해결.
  - 1,000줄 규모의 Stored Procedure를 JavaScript 코드로 리팩토링(500줄)하여 유지보수성 및 안정성 개선.

### **더커머스** (2021.09 - 2023.05)

_서버 개발자 / 정규직_

- **결제 구독권 시스템 개발 및 고도화 (2022.04 - 2022.10)**
  - Java, Spring Boot, MongoDB 기반 시스템 유지보수 및 기능 개선.
  - DTO 활용을 통한 주요 비즈니스 로직 캡슐화 및 테스트 코드 작성.
  - Spring Interceptor 및 Wrapper를 활용하여 요청 바디 스트림 재설정 문제 해결 및 결제 유효성 검증 최적화.
- **오픈마켓 연동 개발 (2021.09 - 2022.03)**
  - 롯데온, 카페24 등 다양한 오픈마켓 OpenAPI 연동(Python, Flask, AWS Lambda).

### **빌리지피플** (2020.03 - 2021.08)

_백엔드 개발자 / 정규직_

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
- **AI & Collaborative Engineering:**
  - **Tools:** Antigravity (Agentic Flow), Gemini, GitHub Copilot
  - **Practices:** Agentic Workflow Design, Strategic Context Management, AI-Driven Architecture Refactoring, Verification & Validation

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
