# CampusConnect Requirements Specification v1
Status: Draft — Week 3
Student: Phuc Hoang Pham
Branch: docs/week-3-requirements-ai
## 1. Problem statement
Students who need IT Support information need a reliable way to find the correct
next step because the current experience may be scattered, difficult to search, or
hard to verify as current.
## 2. Evidence carried forward from Week 2
- E-01: The academic advisor receives questions that involve multiple campus offices and uses saved bookmarks to search for answers.
- E-02: When campus webpages provide conflicting information, the advisor checks with colleagues before responding to students.
- A-01: We assume that advisors have difficulty identifying which campus source is the most current and authoritative; this still needs validation through advisor interviews or observation.
## 3. One user journey inside the MVP
A student asks one typed IT Support question. CampusConnect searches only approved
IT Support material, returns a short answer with a visible source, or says the
available sources do not support an answer.
## 4. Four requirements
- FR-01 — The system shall accept one typed IT Support question.
- GR-01 — Every factual answer shall identify the approved source used.
- SF-01 — If approved sources are insufficient, the system shall not invent an
answer and shall provide a helpful IT Support next step.
- NFR-01 — A keyboard user shall be able to submit a question and read the result.
## 5. MVP boundary
IN: one typed question, approved IT Support material, one grounded answer, visible
source, safe failure, and helpful next step.
OUT: password resets, ticket creation, personal student records, voice, automatic
actions, and answers from unapproved material.
## 6. AI critique and human decision
- ChatGPT suggestion:
    1. GR-01 — Source grounding.
    2. A visible approved-source citation does not establish how the system handles conflicting approved sources.
    3. EVIDENCE: E-02 identifies conflicting campus information; citing one source alone would not resolve that conflict.
    4. RECOMMENDATION: Add “When approved sources conflict on the requested next step, disclose the conflict and use SF-01”; test with two approved sources giving incompatible instructions.
- Claude suggestion:
    1. **Section 2 / FR-01 / GR-01 / SF-01 (evidence-to-requirement trace)**
    2. The evidence is about an academic advisor handling multi-office questions, not students asking IT Support questions (EVIDENCE: E-01, E-02); the claim that "advisors have difficulty identifying the most current source" is already an ASSUMPTION (A-01), yet no requirement says how "approved" or "current" is decided, so GR-01 and SF-01 rest on an undefined term, and the link from advisor evidence to student IT Support needs is an unvalidated ASSUMPTION.
    3. Without a testable definition of "approved source," GR-01 and SF-01 cannot be pass/fail tested, and the whole MVP boundary (IN/OUT) depends on a list that does not yet exist, so Week 4 cannot fairly compare the local and hosted paths.
    4. Add one line to Section 5 or GR-01: "Approved sources = [a named list of IT Support pages/documents chosen by the human team, each with a last-  reviewed date]," and mark the advisor-to-student link as ASSUMPTION until validated; test: ask one question answered by a listed source (expect answer plus that source) and one not covered by it (expect abstention plus next step).
- My decision: Accepted / Revised / Rejected
- My reason: <EXPLAIN USING WEEK 2 EVIDENCE, SCOPE, OR TESTABILITY>
