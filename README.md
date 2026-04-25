<p align="center">
  <img src="assets/readme-banner.svg" alt="Agent Tool Risk Score banner" width="100%">
</p>

<h1 align="center">Agent Tool Risk Score</h1>

<p align="center">Score file, shell, network, browser, and secret risks in AI-agent tool lists.</p>

<p align="center"><a href="README.zh-CN.md">中文</a> · <a href="#quick-start">Quick Start</a> · <a href="#checks">Checks</a> · <a href="#ci-usage">CI</a></p>

<p align="center">
  <img alt="Node.js" src="https://img.shields.io/badge/node-%3E%3D18-2563EB">
  <img alt="dependencies" src="https://img.shields.io/badge/dependencies-0-111827">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-16A34A">
</p>

<p align="center">
  <img src="assets/cli-preview.svg" alt="Agent Tool Risk Score CLI preview" width="88%">
</p>

## Why This Exists

AI-agent workflows keep growing, but many repositories still miss tiny local checks that are easy to repeat in CI. This tool stays zero-dependency, mirror-friendly, and easy to fork.

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
