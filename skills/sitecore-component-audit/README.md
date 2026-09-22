# Sitecore component audit

This skill compares the fields expected by a local Sitecore component with its rendering and datasource through Marketer MCP. It reports missing content and differences between source and rendered text. The audit is read-only.

## Install

Install it for Codex in the current project:

```sh
npx skills add borislavpanov-web/agent-skills --skill sitecore-component-audit --agent codex
```

Add `--global` to use it across projects. In Codex, invoke it with `$sitecore-component-audit` and provide the component, exact Sitecore site, and page to audit.

## Requirements

The skill needs access to the component's local source code and a configured Marketer MCP connection with read-only access to the relevant Sitecore site. Installing the skill does not install or configure Marketer MCP.
