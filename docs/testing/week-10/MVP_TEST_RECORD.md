# Week 10 MVP Test, CI, and Freeze
Student: <Phuc Pham>
Date: <11/16/2026>
Branch: release/week-10-rc1
Local URL: http://127.0.0.1:7860
Environment: <CHROME>
## 1. Six-test MVP record
| # | Quality area | Action and expected result | Observed evidence | Result |
|---|---|---|---|---|
| 1 | Supported retrieval | Ask: "How do I reset my CampusConnect password?" The answer uses
the approved password-reset passage.
| <Open the Campus Portal, choose Help, then Password and Sign-In, and select Reset Password.
Complete the identity check shown by the portal. If the self-service reset fails, contact the IT Service Desk.> | <PASS> |
| 2 | Citation support | Open the displayed source from Test 1. At least one important answer
claim is directly supported by the source passage. 
| Source: IT-01, Password Reset · CampusConnect IT Support Quick Guide v1 (synthetic classroom data) | <PASS> |
| 3 | Unsupported query | Ask: "What are the Thanksgiving dining hall hours?" The system
states its IT-support limit and does not invent hours, a source, phone number, or office. |
I do not have enough approved evidence to answer that. | <PASS> |
| 4 | Voice and text fallback | Use the supported answer. If voice works, its meaning matches
the visible grounded answer. If voice is unavailable, the text, source, and a clear Continue
in text or retry path remain. |THE VOICE WORK | PASS |
| 5 | Video accessibility | Mute the tab and skip the video. AI disclosure and transcript
remain visible, and the chatbot is reachable by keyboard. | AI DISCLOSURE AND TRANSCRIPT IS AVAIABLE | PASS |
| 6 | Latency and recovery | Time one supported question. Class target: grounded text in 5
seconds or less. If slower, the question is preserved and progress, retry, or text fallback is
clear. | FASTER THAN 5 SECOND FOR BOTH VOICE AND TEXT | PASS |
## 2. Lighthouse and manual accessibility evidence
Performance score: 96
Accessibility score: <100>
One important Lighthouse finding or "none listed": <NONE LISTED>
Keyboard plus muted-video result: <NO SEE>
## 3. Defect decision and retest
Highest-severity finding: <NONE>
Severity: <MINOR>
Smallest repair made: <No repair required">
Focused retest result: <GOOD>
## 4. Release gate
Release decision: <go>
Decision reason: <SCORE IS GOOD>
GitHub Actions run: <[(https://campus-it-answer-nook.lovable.app/)](https://github.com/thinhbotibo/comp7431-campusconnect-thinhbotibo/actions/runs/43991740689)>
Release tag if GO: v0.9.0-rc1
## 5. Engineering and AI Use Log
What I tested myself: <TEST ALL WHAT I NEED THE AI SUPPORT TO DO>
What remained human-reviewed rather than automated: <TRY WITH DIFFERENCE CONCEPT OF SAME QUESTION >
Known limitation carried into Week 11 Red Teaming: <STILL SMALL PROJECT, NO MUCH TO TELL>
