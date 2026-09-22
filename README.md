# Agent skills

Reusable skills for AI coding agents.

## Available skills

- [Sitecore component audit](skills/sitecore-component-audit/SKILL.md) — compare a local Sitecore component's expected fields with its rendering and datasource through Marketer MCP. The audit is read-only.

## Install

Install the Sitecore component audit skill for Codex in the current project:

```sh
npx skills add borislavpanov-web/agent-skills --skill sitecore-component-audit --agent codex
```

To use it across projects, add `--global`. In Codex, invoke it with `$sitecore-component-audit` and provide the component, exact Sitecore site, and page to audit.

The skill needs access to the component's local source code and a configured Marketer MCP connection with read-only access to the relevant Sitecore site. Installing the skill does not install or configure Marketer MCP.

The `npx skills add` command downloads skills from this GitHub repository; this repository is not an npm package. It will work once the repository is public and the files are pushed.
