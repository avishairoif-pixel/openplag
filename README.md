# OpenPlag Labs for Gemini CLI

[![M8ven Score](https://m8ven.ai/badge/mcp/avishairoif-pixel-openplag-j4tmm8?v=e75556d6c636b7cc92ea39325e740998)](https://m8ven.ai/mcp/avishairoif-pixel-openplag-j4tmm8?s=readme)

Free originality checks for academic papers, theses and essays, right from Gemini CLI. A document is compared with a local index of more than 180 million open-access records and the open web, in eight languages: English, Hebrew, Arabic, Russian, French, Spanish, German and Chinese. No account and no API key are needed.

## Install

```
gemini extensions install https://github.com/avishairoif-pixel/openplag
```

Then ask Gemini, for example: *"Check my paper thesis.pdf for originality with OpenPlag."* Gemini will ask for your permission before sending the document.

## What you get

- Verbatim overlap with published sources, and whether each shared passage is cited
- Paraphrase and translation candidates, listed separately and never counted in the score
- A link to the full report, valid for 24 hours

A similarity report is not a finding of plagiarism.

## Limits

Up to 10,000 words per check, one document at a time, a few checks a day. For longer documents and saved reports, open a free account at [openplaglabs.com](https://app.openplaglabs.com/?src=github).

## Other clients

The same server works in any MCP client that supports Streamable HTTP:

```
https://app.openplaglabs.com/mcp
```

In the Gemini app (where available), add it under Settings, Connected Apps, Add a custom app.

## Links

- Website: https://app.openplaglabs.com
- For AI agents: https://app.openplaglabs.com/llms.txt
- Terms of service: https://app.openplaglabs.com/terms

License: MIT
