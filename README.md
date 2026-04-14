# 바이브 레디 (Vibe Ready)

> 바이브 코딩 시작 전, 아이디어 검증부터 PRD 완성까지 — Claude와 함께

---

## 왜 바이브 레디인가?

바이브 코딩은 빠르다. 아이디어를 말하면 AI가 코드를 만들어준다.  
하지만 **방향이 틀린 아이디어를 빠르게 만드는 것**은 의미가 없다.

많은 제작자들이 이런 경험을 한다.

- 며칠을 만들었는데 "이게 정말 필요한 건가?" 라는 의문이 든다
- 비슷한 서비스가 이미 있다는 걸 뒤늦게 발견한다
- 누구를 위한 서비스인지 모호해서 기능 결정을 못 한다
- PRD 없이 시작했다가 AI와의 대화가 산으로 간다

바이브 레디는 이 문제를 해결한다.  
**코딩을 시작하기 전에 제작자와 Claude가 함께** 아이디어를 검증하고,  
서비스를 구체화하고, PRD를 완성한다.

---

## 핵심 콘셉

**제작자와 Claude의 협업으로만 완성한다.**

실제 사용자 인터뷰도, 복잡한 시장 조사도 필요 없다.  
Claude가 시장 지식을 바탕으로 가상의 결과를 생성하고,  
제작자가 방향을 결정한다.

| 역할 | 책임 |
|---|---|
| **Claude** | 페르소나 생성, 가상 인터뷰 시뮬레이션, 경쟁사 분석, 문서 초안 작성 |
| **제작자** | 방향 결정, 내용 확정, 최종 판단 |

모든 선택 시점에서 Claude는 **최소 3가지 안을 제시하고 1가지를 추천**한다.  
제작자는 선택하거나, 수정을 요청하거나, 새로운 방향을 제안할 수 있다.

---

## 프로세스 개요

바이브 레디는 두 가지 프로세스를 제공한다.

```
간편 프로세스 ─── 아이디어가 구체적인 경우 (학습용, 빠른 프로토타입)
                  약 1~2시간

고급 프로세스 ─── 실제 출시를 목표로 하거나 아이디어가 불명확한 경우
                  약 4~8시간

                  1단계: 아이디어 검증    → 검증 결과 문서
                  2단계: 경쟁사 분석      → 경쟁사 분석표
                  3단계: 서비스 기획      → 서비스 기획서
                  4단계: 문서 완성        → PRD + 액션플랜
```

4단계가 끝나면 바이브 코딩을 바로 시작할 수 있다.

---

## 저장소 구조

```
vibe-ready/
│
├── README.md                           ← 이 파일 (프로젝트 소개)
├── CLAUDE.md                           ← Claude용 저장소 컨텍스트
├── master.md                           ← 전체 프로세스 마스터 문서
├── quick-process.md                    ← 간편 프로세스 (기존 app-build-process-prd)
│
├── guides/                             ← 단계별 가이드
│   ├── 01-idea-validation.md
│   ├── 02-competitive-analysis.md
│   ├── 03-service-planning.md
│   └── 04-document-completion.md
│
├── prompts/                            ← 단계별 프롬프트 모음
│   ├── 01-idea-validation-prompts.md
│   ├── 02-competitive-analysis-prompts.md
│   ├── 03-service-planning-prompts.md
│   └── 04-document-completion-prompts.md
│
└── templates/                          ← 보조 문서 템플릿
    ├── 01-validation-result.md
    ├── 02-competitive-analysis.md
    ├── 03-service-plan.md
    ├── 04-persona.md
    └── 05-virtual-interview.md
```

---

## 시작하는 법

### 1단계: 저장소 설정
1. 이 저장소를 Claude 프로젝트 지식에 연결한다

### 2단계: 프로젝트 초기화
2. Claude에게 다음과 같이 입력한다

```
바이브 레디 시작
```

3. Claude가 프로젝트 영문 키워드를 물어보면 답한다  
   예) `my-app`, `pet-care`, `todo-service`

4. Claude가 `[키워드]-claude.md` 파일을 생성해 준다

### 3단계: 프로젝트 지식 추가
5. 생성된 `[키워드]-claude.md` 파일을 Claude 프로젝트 지식에 문서로 추가한다

### 4단계: 바이브 레디 시작
6. `master.md`를 참고하여 프로세스를 선택하고 Claude와 대화를 시작한다

---

## 라이센스

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

이 저장소는 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 라이센스를 따릅니다.

- ✅ 개인 학습 및 비상업적 사용 — 허용
- ✅ 출처 표시 후 공유 — 허용
- ❌ 상업적 사용 — 금지
- ❌ 수정 후 다른 조건으로 배포 — 금지

Copyright (c) 2026 Taewon

*버전: 0.1 | 언어: 한국어 | 작성: 2026년 4월*