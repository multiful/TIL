---
alias:
tags:
  - lecture-note
date: 2026-06-23
created: 2026-06-23 20:13
updated: 2026-06-23 20:13
---


> [!info] 강의 정보
> - **작성일:** 2026-06-23
> - **분야:** #AI_ML
> - **강의 출처:** [링크](https://file.notion.com/f/f/c69962b0-3951-485b-b10a-5bb29576bba8/7cc2d436-2fa6-4659-9b05-73c4654972b3/(0623)NLP4%EA%B8%B0_vibecoding.pdf?table=block&id=38744860-a4f4-803f-9372-d9cfb4965bea&spaceId=c69962b0-3951-485b-b10a-5bb29576bba8&expirationTimestamp=1782237600000&signature=Yfebob6Bbz6zx6UrW5uXBZcQpU6bgMyx9634hHoL0M8&downloadName=%280623%29NLP4%EA%B8%B0_vibecoding.pdf)
> - **관련 데일리:** [[2026-06-23 데일리 로그 & 회고]]

---

## 1. 핵심 내용 요약

> 한 줄 요약: NLPg는 실패했지만 그 흐름이 Copilot → ChatGPT → Cursor → Claude Code로 이어져 Vibe Coding 시대를 열었다.

### 핵심 개념
- NLPg: 자연어를 프로그래밍 언어처럼 컴파일하려 했던 시도 → 중의성·Ontology 문제로 실패
- Vibe Coding: 명확한 명령 대신 "느낌과 의도"로 AI와 대화하며 코드를 만드는 방식
- Agent-first Design: AI가 스스로 판단하고 수행, 개발자는 목표만 설정

---

## 2. 내용 정리

### 개념: NLPg (Natural-language Programming)
- **정의:** 자연어를 프로그래밍 언어로 1:1 대체하는 방식. 자연어 컴파일러를 만드는 것이 목표였음
- **특징:** SQL, Regex 같은 부분적 성과는 있었지만, 자연어의 중의성과 Ontology 구축 실패로 전면 도입은 좌절됨

### 개념: AI 개발 도구의 흐름
- **Github Copilot (2021):** 코드 자동완성 + 컨텍스트 기반 추천. AI가 개발에 관여 가능하다는 걸 처음 실증함
- **ChatGPT (2022):** 자연어로 코드 생성·수정하는 트렌드 확산. Agentic IDE의 기반이 됨
- **Cursor (2023):** AI를 IDE에 직접 내장. 프로젝트 전체 조작 가능. 단, 사람이 명령하면 수행하는 구조
- **Claude Code (2024):** Agent-first. AI가 스스로 무엇을 해야 할지 판단하고 전체 개발 루프를 자율화

### 개념: NLPg vs Vibe Coding 비교

| 구분 | NLPg | Vibe Coding |
|------|------|-------------|
| 입력 | 명확한 지시 | 느낌과 의도 |
| 역할 | 컴파일 가능한 자연어 | 의도에 맞는 코드 생성 |
| 실패 원인 | 문장 해석 오류 | 컨텍스트 부족 |
| 반복 방식 | 명령 수정 | 대화 기반 동작 |

### 개념: Vibe Coding 일반 프로세스
- **정의:** AI와 대화하면서 느낌 기반으로 코드를 완성해 나가는 개발 방식
- **특징:** 작업 지시 → 계획 → 수정 및 테스트 → PR 작성 → 검토/승인 순으로 진행

---

## 3. 중요 포인트

### 기억해야 할 내용
- NLPg 실패 원인은 기술 부족이 아니라 "자연어의 모호성"과 "Ontology 부재"였음
- Ontology는 딥러닝 이전엔 지식 모델, 현재는 데이터 의미 통합 모델로 쓰임

### 헷갈리는 내용
- Vibe Coding에서 "컨텍스트 부족"이 실패 원인인데 → 결국 프롬프트를 얼마나 잘 주느냐가 핵심
- Agent-first vs 기존 방식의 경계가 실제 사용에선 아직 흐릿하게 느껴짐

---

## 4. 프로젝트 연결

- **적용 아이디어:**
  - Claude Code나 Cursor 쓸 때 단순 명령보다 "의도와 배경"을 충분히 설명하면 더 잘 됨
  - PR 작성 시 AI에게 변경 이유 + 구현 방식 + 테스트 방법을 함께 정리시키면 활용도 높음

---

## 5. 개인 정리

- **새롭게 알게 된 점:**
  - NLPg가 실패한 게 단순 기술 문제가 아니라 언어 자체의 구조적 문제였다는 것
  - Vibe Coding은 NLPg의 재시도가 아니라 방향 자체가 다름 (컴파일 목표 x, 의도 파악 o)
- **추가 학습 필요:**
  - Ontology 개념 더 파보기 (지식 그래프, RDF 등)
  - Agent-first 설계 패턴 실제 사례 찾아보기
- **한 줄 총평:**
  > AI 개발 도구의 역사를 한 줄로 꿴 강의. NLPg → Vibe Coding으로 이어지는 맥락이 명확해졌다.