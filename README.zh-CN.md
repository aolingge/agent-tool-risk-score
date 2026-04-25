<p align="center">
  <img src="assets/readme-banner.svg" alt="Agent Tool Risk Score banner" width="100%">
</p>

<h1 align="center">Agent Tool Risk Score</h1>

<p align="center">给 Agent 工具清单中的文件、shell、网络、浏览器和密钥风险打分。</p>

<p align="center"><a href="README.md">English</a> · <a href="#quick-start">快速开始</a> · <a href="#checks">检查项</a> · <a href="#ci-usage">CI</a></p>

<p align="center">
  <img alt="Node.js" src="https://img.shields.io/badge/node-%3E%3D18-2563EB">
  <img alt="dependencies" src="https://img.shields.io/badge/dependencies-0-111827">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-16A34A">
</p>

<p align="center">
  <img src="assets/cli-preview.svg" alt="Agent Tool Risk Score CLI preview" width="88%">
</p>

## 为什么做这个

AI Agent 工具越来越多，但很多仓库缺少能在本地和 CI 里重复执行的小检查。这个工具保持零依赖、可镜像、可复制，适合学生、独立开发者和开源维护者使用。

## Quick Start

```bash
npx github:aolingge/agent-tool-risk-score --path tools.md
```

```bash
npx github:aolingge/agent-tool-risk-score --path tools.md --markdown > report.md
npx github:aolingge/agent-tool-risk-score --path tools.md --sarif > results.sarif
npx github:aolingge/agent-tool-risk-score --path tools.md --annotations
```

## Checks

| Check | What it looks for |
| --- | --- |
| files | Mentions file access. |
| shell | Mentions shell access. |
| network | Mentions network/browser access. |
| secrets | Mentions secret handling. |

## CI Usage

See [docs/github-actions.md](docs/github-actions.md) and [docs/quality-gates.md](docs/quality-gates.md).

## Mirrors

- GitHub: https://github.com/aolingge/agent-tool-risk-score
- Gitee: https://gitee.com/aolingge/agent-tool-risk-score

## Contributing

Good first PRs: add checks, add fixtures, improve docs, or add GitHub Actions examples.

## License

MIT
