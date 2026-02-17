# Pokitwork Knowledge Base

포킷워크 도메인 지식베이스. HR/연차 관리 시스템의 비즈니스 요구사항을 단일 스킬로 관리한다.

## 구조

```
SKILL.md                          ← 전체 도메인 요약 (스킬 진입점)
references/
  organization.md                 ← 조직관리 (구성원, 부서, 직책, 프로젝트)
  organization-schema.md
  leave.md                        ← 연차/휴가관리 (유형, 정책, 부여형, 신청, 휴직, 사용촉진)
  leave-schema.md
  approval.md                     ← 결재관리 (결재선, 요청, 단계, 수신참조, 알림)
  approval-schema.md
  notice.md                       ← 공지/알림 (공지사항, 카테고리, Inbox)
  notice-schema.md
  attendance.md                   ← 근태관리 (유연근무, 단축근로)
  attendance-schema.md
```

## 스킬 갱신

도메인 요구사항이 변경되면 해당 references/ 파일을 수정하고 push한다.
팀원은 `npx skills add pokitwork/knowledge-base`로 최신 버전을 받는다.
