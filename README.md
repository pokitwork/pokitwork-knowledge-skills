# Pokitwork Knowledge Skills

Pokitwork 프로젝트의 공유 지식베이스. [Agent Skills (SKILL.md)](https://agentskills.io) 표준을 따르며, 모든 AI 코딩 에이전트에서 사용할 수 있다.

## Skills

| 스킬 | 설명 |
|------|------|
| `project-setup` | 프로젝트 초기 설정 (AGENTS.md 생성 + 에이전트별 설정) |
| `sveltekit-conventions` | SvelteKit 서버 레이어 아키텍처 (Active Record, Query Service, REST API) |
| `design-system` | 디자인 시스템 규칙 (shadcn 테마, 색상, 컴포넌트 배치) |
| `directory-structure` | 프로젝트 디렉토리 구조 + 라우트 맵 |
| `server-api` | 구현된 Query Service 및 REST API 엔드포인트 카탈로그 |

## 설치

### Claude Code

`.claude/skills/` 에 설치된다. ([문서](https://code.claude.com/docs/en/skills))

```bash
/skills install https://github.com/pokitwork/pokitwork-knowledge-skills
```

### Antigravity

`.antigravity/skills/` 에 설치된다. ([문서](https://antigravity.google/docs/skills))

```bash
/skills install https://github.com/pokitwork/pokitwork-knowledge-skills
```

### Cursor

`.cursor/skills/` 에 설치된다. ([문서](https://cursor.com/ko/docs/context/skills))

```bash
/skills install https://github.com/pokitwork/pokitwork-knowledge-skills
```

### OpenAI Codex

`.agents/skills/` 에 설치된다. ([문서](https://developers.openai.com/codex/skills))

```bash
$skill-installer install skills from https://github.com/pokitwork/pokitwork-knowledge-skills
```
