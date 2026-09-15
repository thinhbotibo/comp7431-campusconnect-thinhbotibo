# Verification

## Planned commands
- Run: python app.py
- Test: pytest

## Required evidence for the later prototype
- [ ] 5 expected questions pass
- [ ] 2 confusing questions get a safe fallback
- [ ] Source and owner display correctly
- [ ] No private data is required

## Concrete fallback test cases

1. Conflicting guidance: When two approved sources provide different deadlines, the system must display both sources and owners, identify the conflict, avoid selecting one as correct, and offer a human handoff.

2. Unsupported question: When no approved source answers a question, the system must state that it cannot verify the answer, avoid inventing information, and direct the student to an appropriate human office.

## Week 1 evidence
- [ ] Every Markdown file opens in VS Code
- [ ] sample_pages.md says the content is synthetic
- [ ] No password, token, API key, or student record appears

## Rule
Fix the app, not the test, unless the expected result is wrong.

