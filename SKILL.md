---
name: knowledge-base
description: 포킷워크(PokitWork) HR 도메인 지식베이스. 조직관리, 연차/휴가, 결재, 공지/알림, 근태의 엔티티 정의와 비즈니스 규칙. HR 관련 기능 구현 시 참고한다.
---

# PokitWork 도메인 지식베이스

HR SaaS 시스템의 비즈니스 요구사항을 서브도메인별로 관리한다.

## 서브도메인

### 조직관리 (Organization)

구성원(직원), 부서, 직책, 프로젝트를 관리한다.

- 구성원: 이름, 이메일, 사번, 소속부서, 직책, 입사일, 역할(admin/manager/user), 상태(재직/휴직/퇴직)
- 부서: 플랫 리스트, 리더 지정, 정렬
- 직책: 이름(고유), 정렬
- 프로젝트: PM + 수행인원, PM 이중결재 연동

상세: [references/organization.md](references/organization.md) | [스키마](references/organization-schema.md)

### 연차/휴가 (Leave)

연차 유형, 연차 정책(입사일/회계연도 기준), 부여형 휴가, 연차 신청, 휴직, 연차사용촉진을 관리한다.

- 연차 차감 유형: 연차(1일), 반차(0.5일), 반반차(0.25일)
- 계산 방식: 입사일 기준(A) / 회계연도 기준(B) — 회사 단위 설정
- 부여형 휴가: 포상휴가, 대체휴가 등 관리자 직접 부여
- 휴직: 육아/질병/가족돌봄/기타

상세: [references/leave.md](references/leave.md) | [스키마](references/leave-schema.md)

### 결재 (Approval)

결재선 규칙, 결재 요청, 결재 단계, 수신참조, 알림을 관리한다.

- 부서별 결재선 설정 (순차 승인)
- 프로젝트 PM 추가 결재
- 결재 요청 유형: 연차, 지출, 출장, 경조사, 교육
- 상태: 임시보관 → 대기 → 진행중 → 완료/반려
- 수신참조: 임원 + 경영지원팀 자동 추가

상세: [references/approval.md](references/approval.md) | [스키마](references/approval-schema.md)

### 공지/알림 (Notice)

공지사항, 카테고리, 개인 알림, 전체 알림을 관리한다.

- 공지사항: 관리자 작성, 카테고리 분류, 고정, 조회수
- 개인 알림: 결재 관련 등 1:1 알림
- 전체 알림: 공지 등록 시 전체 발송, 읽음 추적
- Inbox: 전체 | 결재 | 내 신청 | 알림 탭 통합

상세: [references/notice.md](references/notice.md) | [스키마](references/notice-schema.md)

### 근태관리 (Attendance)

유연근무제(시차출퇴근, 재택근로), 단축근로(육아기, 임신중)를 관리한다.

- 시차출퇴근: 코어타임 설정, 출퇴근 시간 조정
- 재택근로: 사전 신청, 시작/종료 보고
- 육아기 단축근로: 만 8세 이하, 주 15~35시간
- 임신 중 단축근로: 12주 이내/36주 이후, 1일 2시간 단축

상세: [references/attendance.md](references/attendance.md) | [스키마](references/attendance-schema.md)
