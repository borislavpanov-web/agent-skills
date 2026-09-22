---
name: sitecore-component-audit
description: Read-only comparison of a local Sitecore component's expected fields with its rendered instance and datasource in Sitecore through Marketer MCP. Use when asked to audit component field mappings or missing content.
---

# Sitecore component audit

1. Locate the requested component in the local codebase. Read its TSX and directly relevant types or helpers. List every field it expects, including rendering parameters when relevant, with its local type, whether it is required, and a file and line citation. Distinguish fields read directly from fields used by child components.
2. Establish the exact Sitecore site and page before making a Sitecore query. Use identifiers already supplied or confirmed in the conversation; if either is ambiguous, ask the user to identify it. Do not guess from a similar page or site.
3. Use Marketer MCP read-only tools to locate the component's rendering on that page and its linked datasource. Record the page, rendering, and datasource identifiers or URLs. If multiple instances match, identify each one or ask which instance to audit.
4. Compare local field names and types with datasource fields and their current values. For each text field, show the actual source content and the text visible in the rendered component, including headings or text over images. Note formatting, truncation, or transformation when the two differ. Account for Sitecore field wrappers, empty values, and fields inherited or supplied through rendering parameters. Cite the local code location, the datasource field, and the rendered page location for each comparison. Label any type compatibility judgment as an inference when the Sitecore field type is not directly exposed.
5. Report mismatched names or types, source versus rendered text differences, missing fields, empty required values, and any values that cannot be verified. Keep missing, empty, and inaccessible distinct. If the rendering or datasource cannot be found, report the search scope and what remains unverified.

This audit is read-only. Do not edit code, Sitecore content, configuration, or generated files. Do not run builds or tests.
