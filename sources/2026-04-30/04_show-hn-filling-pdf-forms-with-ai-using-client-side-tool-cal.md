---
type: story
story_id: hn_47947347
episode_date: 2026-04-30
rank: 4
source: hacker_news
url: "https://copilot.simplepdf.com/?share=a7d00ad073c75a75d493228e6ff7b11eb3f2d945b6175913e87898ec96ca8076&form=w9&lang=en"
title: Show HN Filling PDF forms with AI using client-side tool calling
quality_score: 0.663
content_hash: "sha256:e53cc63bc61424c720e5da8947f2c9b9bd8492e4e56eac9dbbee9a8f7719607b"
concepts: [simplepdf-copilot, client-side-tool-calling, tool-calling, ai-assistant, pdf-editor, simplepdf, commonforms, tanstack-start, ai-sdk, tailwind, css-modules, iframe-postmessage, lm-studio, deepseek-v4-flash]
companies: [simplepdf, vercel]
people: [joe-barrow]
extractor_model: gemini-2.5-flash-lite
extracted_at: "2026-04-30 10:17:28.597000"
tags: [story, source/hacker-news]
---

## Summary
The author has developed SimplePDF Copilot, an AI assistant that integrates with a client-side PDF editor to fill forms, answer questions, and manipulate documents. Unlike traditional "Chat with PDF" tools, Copilot performs these actions directly within the browser, ensuring that the PDF data never leaves the user's device, which is crucial for privacy-sensitive applications like healthcare. The system leverages client-side tool calling, where the LLM determines the action, but the execution occurs in the browser for speed and enhanced data control. The demo is open-source, though the core SimplePDF editor is not.

## Key claims
- SimplePDF Copilot is an AI assistant that can interact with a client-side PDF editor.
- The tool can fill fields, answer questions, focus on specific fields, add fields, and delete pages within a PDF.
- All PDF parsing, rendering, and field detection occur client-side, ensuring the PDF never leaves the browser.
- The AI assistant uses client-side tool calling, where the LLM initiates actions executed in the browser.
- This approach enhances speed and allows users to limit the data exposed to the LLM.
- The primary motivation for developing Copilot was to provide an AI experience for healthcare customers without compromising document privacy.
- The demo is open-source and available on GitHub.

## Source
- **Origin:** hacker_news
- **URL:** <https://copilot.simplepdf.com/?share=a7d00ad073c75a75d493228e6ff7b11eb3f2d945b6175913e87898ec96ca8076&form=w9&lang=en>

## Related
[[concepts/simplepdf-copilot|simplepdf-copilot]] · [[concepts/client-side-tool-calling|client-side-tool-calling]] · [[concepts/tool-calling|tool-calling]] · [[concepts/ai-assistant|ai-assistant]] · [[concepts/pdf-editor|pdf-editor]] · [[concepts/simplepdf|simplepdf]] · [[concepts/open-source|open-source]] · [[concepts/mcp-server|mcp-server]] · [[concepts/cloud|cloud]] · [[concepts/llms|llms]] · [[concepts/sdk|sdk]] · [[concepts/ocr|ocr]] · [[concepts/pii|pii]] · [[concepts/llm|llm]] · [[concepts/mcp|mcp]] · [[concepts/ai|ai]] · [[companies/simplepdf|SimplePDF]] · [[companies/vercel|Vercel]] · [[people/joe-barrow|Joe Barrow]] · [[episodes/2026-04-30|2026-04-30]]
