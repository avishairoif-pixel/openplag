# OpenPlag Labs: originality checks

Use the `openplag` MCP tools when the user asks to check a paper, thesis, essay or other academic text for plagiarism, overlap with published work, citation problems or originality. Texts in English, Hebrew, Arabic, Russian, French, Spanish, German and Chinese are supported.

## How to use the tools

1. **Ask first.** Before calling `check_document`, tell the user that the document will be sent to OpenPlag Labs, an external service, checked, and deleted when the check ends. Call the tool only after the user agrees, and set `user_confirmed` to true.
2. **One document per request.** Never send several documents at once, and never split a long document into parts. The limit is 10,000 words per check.
3. **Wait patiently.** A check takes 10 to 20 minutes. Call `get_check` with the token you received, no more often than the `poll_after_seconds` value in the answer.
4. **Respect refusals.** If a call is refused, follow its message. If `retry` is false, do not retry, and pass `tell_user` on to the user.
5. **Report honestly.** Give the user the summary and the link to the full report (valid for 24 hours), and always pass on the disclaimer that comes with the result.

## How to explain the result

- The main score is **verbatim overlap**: identical or lightly changed passages shared with other sources. The report shows whether each shared passage is cited.
- **Paraphrase and translation candidates** are listed separately and are never counted in the score.
- A similarity report is **not a finding of plagiarism**. Quoted and properly cited passages are normal in academic work.
- The writing indicator is a probability, not evidence.

Users who need longer documents (up to 60,000 words), reports kept for 30 days or a history of checks can open a free account at https://app.openplaglabs.com/?src=gemini

Terms of service: https://app.openplaglabs.com/terms
