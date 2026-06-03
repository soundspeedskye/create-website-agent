# create-website-agent

`create-website-agent` is an agent instruction document set for generating an initial client-side website from scratch.

This repository is not a generated website. It contains the rules and workflow that an agent follows when creating a new website.

## What It Generates

- React + TypeScript + Vite
- Tailwind CSS
- React Router
- FSD-based structure
- Client-only demo app
- localStorage demo data
- sessionStorage login state
- Mock account authentication

## How To Use

1. Place this document set where your agent can read it.
2. Use `agent.md` as the starting instruction.
3. Let the agent read `rules/index.md` and `workflow/index.md` first.
4. Follow the numbered workflow order.
5. Read detailed rule files only when needed.

This is intended for init-stage website creation, not for merging into an existing production project.

## Limitations

Generated apps do not include real backend authentication, database persistence, OAuth/JWT, real file storage, email sending, or production-level security.

## License

MIT License. Copyright (c) 2026 soundspeedskye

---

# create-website-agent 한국어

`create-website-agent`는 초기 상태의 클라이언트 웹사이트를 생성하기 위한 에이전트 지시문 문서 모음입니다.

이 저장소는 생성된 웹사이트가 아니라, 에이전트가 새 웹사이트를 만들 때 따라야 할 규칙과 워크플로를 담고 있습니다.

## 생성 대상

- React + TypeScript + Vite
- Tailwind CSS
- React Router
- FSD 기반 구조
- 서버 없는 클라이언트 데모 앱
- localStorage 데모 데이터
- sessionStorage 로그인 상태
- mock 계정 기반 인증

## 사용 방법

1. 에이전트가 읽을 수 있는 위치에 이 문서 모음을 둡니다.
2. `agent.md`를 시작 지시문으로 사용합니다.
3. `rules/index.md`와 `workflow/index.md`를 먼저 읽게 합니다.
4. `workflow/index.md`의 번호 순서대로 진행하게 합니다.
5. 세부 기준이 필요할 때만 개별 rule 문서를 읽게 합니다.

이 문서는 기존 운영 프로젝트에 병합하기 위한 것이 아니라, init 상태에서 새 웹사이트를 초기 제작하기 위한 용도입니다.

## 제한사항

생성된 앱은 실제 서버 인증, DB, OAuth/JWT, 실제 파일 저장, 실제 메일 전송, 운영 수준의 보안을 포함하지 않습니다.

## 라이선스

MIT License. Copyright (c) 2026 soundspeedskye

---

# create-website-agent 简体中文

`create-website-agent` 是一组用于生成初始客户端网站的 Agent 指令文档。

这个仓库本身不是生成后的网站，而是用于指导 Agent 创建新网站的规则和工作流文档。

## 目标输出

- React + TypeScript + Vite
- Tailwind CSS
- React Router
- 基于 FSD 的结构
- 无服务器客户端演示应用
- 基于 localStorage 的演示数据
- 基于 sessionStorage 的登录状态
- 基于 mock 账号的认证流程

## 使用方法

1. 将该文档集放在 Agent 可以读取的位置。
2. 使用 `agent.md` 作为起始指令。
3. 让 Agent 先读取 `rules/index.md` 和 `workflow/index.md`。
4. 按照 `workflow/index.md` 的编号顺序执行。
5. 仅在需要详细标准时读取具体 rule 文档。

该文档集适用于 init 阶段的新网站初始制作，不适用于直接合并到已有生产项目。

## 限制

生成的应用不包含真实服务器认证、数据库、OAuth/JWT、真实文件存储、真实邮件发送或生产级安全保证。

## License

MIT License. Copyright (c) 2026 soundspeedskye
