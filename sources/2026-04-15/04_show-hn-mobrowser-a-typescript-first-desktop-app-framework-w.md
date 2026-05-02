---
type: story
story_id: hn_47766955
episode_date: 2026-04-15
rank: 4
source: hacker_news
url: "https://teamdev.com/mobrowser/"
title: "Show HN MōBrowser, a TypeScript-first desktop app framework with typed IPC"
quality_score: 0.611
content_hash: "sha256:4f0cf50da62dad0c7176e204d0e1a22cfdc28dcff71f4439f50a614d0d155403"
concepts: [mobrowser, typed-ipc, protobuf, electron, tauri, jxbrowser, dotnetbrowser, chromium, node-js, webview]
companies: [teamdev]
people: []
extractor_model: claude-sonnet-4-6
extracted_at: "2026-05-02 03:16:26.278000"
tags: [story, source/hacker-news]
---

## Summary
MōBrowser is a new TypeScript-first desktop application framework built on TypeScript, Node.js, and Chromium, created by the team behind JxBrowser and DotNetBrowser. It aims to address pain points found in Electron (lack of type-safe IPC, no source code protection, weak modern web stack support) and Tauri (inconsistent WebViews across platforms, Rust/JS split stack). The framework features typed IPC via Protobuf code generation, consistent cross-platform rendering, built-in packaging and auto-updates, and source code protection. The author has 15 years of experience embedding web browsers into Java and .NET desktop applications and is seeking feedback from developers with production Electron or Tauri experience.

## Key claims
- MōBrowser is a desktop app framework built on TypeScript, Node.js, and Chromium.
- Typed IPC in MōBrowser is implemented using Protobuf code generation for RPC-style communication instead of string channels.
- Electron lacks type-safe IPC, source code protection, and strong support for the modern web stack according to the author.
- Tauri suffers from inconsistent WebView behavior across platforms and requires a Rust/JS split stack.
- MōBrowser includes built-in packaging, scaffolding, small delta auto-updates, and source code protection.
- The framework is developed by the team behind JxBrowser and DotNetBrowser, with 15 years of browser-embedding experience.
- MōBrowser targets web developers who want to ship desktop apps using a familiar web stack with fewer cross-platform surprises.

## Source
- **Origin:** hacker_news
- **URL:** <https://teamdev.com/mobrowser/>

## Related
[[concepts/mobrowser|mobrowser]] · [[concepts/typed-ipc|typed-ipc]] · [[concepts/protobuf|protobuf]] · [[concepts/electron|electron]] · [[concepts/tauri|tauri]] · [[concepts/jxbrowser|jxbrowser]] · [[concepts/dotnetbrowser|dotnetbrowser]] · [[concepts/chromium|chromium]] · [[concepts/node-js|node-js]] · [[concepts/typescript|typescript]] · [[concepts/views|views]] · [[concepts/delta|delta]] · [[companies/teamdev|TeamDev]] · [[episodes/2026-04-15|2026-04-15]]
