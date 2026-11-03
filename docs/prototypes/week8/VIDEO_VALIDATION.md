# Week 8 AI Presenter Prototype and Validation
Student: <Phuc Pham>
Date: <11/02/2026>
Branch: feature/week-8-avatar-prototype
HeyGen project: <CampusConnect: AI Presenter Introduction>
## Prototype hypothesis
A short AI presenter will help a new user understand the supported
IT topics, privacy boundary, and human fallback.
## Shared video
AI-generated presenter - not a live staff member.
This is a prerecorded introduction. It does not answer questions.
[Watch the CampusConnect presenter]
https://app.heygen.com/videos/campusconnect-ai-presenter-introduction-b0e789f5df12560db15686d98816f551
## Transcript
Hello. I am an AI-generated CampusConnect presenter, not a live staff member. You can use CampusConnect
for approved campus IT help.
Ask about password resets, secure campus Wi-Fi, or the IT Service Desk. Please do not share passwords,
recovery codes, student records, or other private information.
If the chatbot cannot support an answer from its approved guide, it will direct you to a human. This video is a
prerecorded introduction. You can read the same script in our GitHub project.
## Five checks
1. AI disclosure, IT topics, privacy, and fallback: <OBSERVED; PASS>
2. Full script and video duration: <SECONDS; OBSERVED; PASS>
3. Captions on and readable: <OBSERVED; PASS>
4. Muted video and GitHub transcript: <OBSERVED; PASS>
5. Share link works without HeyGen sign-in: <OBSERVED; PASS>
## Design decision
Decision: <KEEP / CHANGE / REMOVE the presenter idea>
Reason based on my checks: add. Adding script to video so every one can watch video, they don't have to listen to it. 
One improvement for later: <since topic relate to find resource for student, it work be better if could generate the AI watch around campus>
## Engineering and AI Use Log
AI tool used: HeyGen
What HeyGen generated: <an AI video that read from what I input.>
What I verified myself: <work fine>
Remaining limitation: <take very long time just for 30s video, if the script is long, I think it will take forever.>
