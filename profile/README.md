# TestDino

TestDino is the test intelligence platform for Playwright. It explains what your suite is doing across every CI run, and exposes every operation to AI agents over the Model Context Protocol or the REST API.

A Playwright report explains a single run. TestDino keeps all of them: it groups failures by root cause, detects flaky tests across runs, tracks code coverage, and returns answers where you already work, in your pull request, in Slack, and in your IDE.

## Get started

```bash
npm install @testdino/playwright
```

Add the reporter to `playwright.config.ts` and set `TESTDINO_TOKEN` in CI. Results stream to the dashboard as each test completes, with no separate upload step.

Full setup: [docs.testdino.com/getting-started](https://docs.testdino.com/getting-started)

## What it does

| Capability | Detail |
|:---|:---|
| Real-time streaming | Results, traces, screenshots, and videos appear during the run |
| Failure classification | Every failure is sorted into Actual Bug, UI Change, Unstable Test, or Miscellaneous |
| Flaky test detection | Flakes identified across runs, branches, and pipelines |
| Error grouping | Similar failures collapsed by error message and root cause |
| CI checks | Block merges until tests meet your quality gates |
| Code coverage | Track which code your tests cover and spot gaps across runs |
| Test management | Manual test cases, runs, and releases alongside automated results |
| MCP server | Claude, Cursor, and Copilot query test data and act on it directly |

## For AI agents

TestDino is agent-callable end to end. An agent connected over MCP can check suite health, find flaky tests, debug a failing test case, write manual test cases, and create releases in one call. The same operations are available over REST, authenticated with the same `td_pat_` personal access token.

| Interface | Use it for |
|:---|:---|
| [MCP server](https://docs.testdino.com/mcp/overview) | Interactive debugging and test-data questions from an IDE or chat agent |
| [REST API](https://docs.testdino.com/api-reference/overview) | Scripted and bulk access |
| [OpenAPI spec](https://docs.testdino.com/openapi.json) | Machine-readable contract |

## CI providers

GitHub Actions, GitLab CI, CircleCI, Azure DevOps, and Jenkins. See [CI setup](https://docs.testdino.com/guides/ci-setup-overview).

## Links

- [Documentation](https://docs.testdino.com)
- [Changelog](https://changelog.testdino.com)
- [Product](https://app.testdino.com)

## Community

[LinkedIn](https://www.linkedin.com/company/testdino) · [X](https://x.com/testdinohq) · [YouTube](https://www.youtube.com/@testdinohq) · support@testdino.com
