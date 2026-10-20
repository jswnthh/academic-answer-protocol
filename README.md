# Academic Answer Generation Protocol (AGP)

Reusable, versioned instructions for generating examination answers using AI assistants. **Version 1.0**.

## Student quick start

1. Open an AI assistant that can read public web links.
2. Paste the **raw URL** for [`AGP.md`](AGP.md), followed by your question and marks.
3. For subject-specific marking, also provide the raw link to the relevant file in `subjects/`.
4. If the assistant cannot read a URL, copy and paste the Markdown file's contents instead.

**Prompt to copy:**

> Read and follow the complete answer-generation instructions at `https://raw.githubusercontent.com/USERNAME/REPOSITORY/main/AGP.md`. Also read the subject rubric at `https://raw.githubusercontent.com/USERNAME/REPOSITORY/main/subjects/operating-systems.md`. If either link cannot be accessed, tell me before answering. Subject: Operating Systems. Question: What is CPU scheduling? Marks: 2.

Replace `USERNAME/REPOSITORY` with your GitHub repository path, and change the subject file and question as needed.

## Files

| File | Purpose |
|---|---|
| `AGP.md` | Self-contained master instructions and fallback mark-wise rules |
| `rules/mark-wise.md` | Educator-facing explanation of 2/5/10-mark formats |
| `subjects/operating-systems.md` | Source-based OS CIA I rubric and key constraints |
| `subjects/business-mathematics-statistics.md` | Source-based BMS CIA I question-specific marking guidance |
| `STUDENT-GUIDE.md` | Copyable student prompts and troubleshooting |

## Updating rules
Edit files on GitHub and commit. The `main` raw URL will serve the latest committed version, but **AI conversations do not automatically refresh their previous context**. Students should start a new chat or explicitly request that the assistant re-fetch the rules. For reproducible assessment, link to a specific commit instead of `main`.

## Limitations
A link is not a guaranteed enforcement mechanism. Some AI products cannot retrieve raw URLs, and assistants can misinterpret instructions or make factual errors. Check textbook references, calculations and exam requirements. Do not treat this repository as an official institution policy unless formally approved.

## Source provenance
Derived from two uploaded CIA I rubric/answer-key documents (Operating Systems and Business Mathematics and Statistics). This repository generalizes their formatting rules and retains subject-specific assessment criteria. It does not reproduce complete official question papers or supply missing datasets.
