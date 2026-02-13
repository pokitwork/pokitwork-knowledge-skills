# Pokitwork Knowledge Skills

Pokitwork 프로젝트의 공유 지식베이스. [Agent Skills (SKILL.md)](https://github.com/anthropics/agent-skills) 표준을 따르며, Claude, Gemini CLI, OpenAI Codex 등 모든 AI 코딩 에이전트에서 사용할 수 있다.

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

```bash
/skills install https://github.com/dev-goraebap/pokitwork-knowledge-skills
```

### Gemini CLI

```bash
gemini skill install https://github.com/dev-goraebap/pokitwork-knowledge-skills
```

### OpenAI Codex

```bash
# .agents/skills/ 에 클론
git clone https://github.com/dev-goraebap/pokitwork-knowledge-skills .agents/skills/pokitwork
```
