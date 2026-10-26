# Week 7 Voice Contract and Prototype
Student: <PHUC>
Date: <10/26/2026>
Agent name: CampusConnect Voice - <PHAM>
Tool: ElevenLabs Agents, free tier
## 1. Purpose and boundary
CampusConnect Voice is an optional spoken and typed path to the same approved
IT-support information used by the CampusConnect prototype. It is a classroom
prototype, not a production help desk.
## 2. Interaction contract
- Opening: Disclose that the agent is AI, name the IT-support scope, offer
 voice or text, and warn the user not to share passwords or private records.
- Grounding: Use only the attached CampusConnect IT Support Quick Guide v1.
- Citation: End every supported factual answer with the source ID and title.
- Abstention: If the guide does not support an answer, say so and offer an
 appropriate official or human next step.
- Action boundary: Explain steps, but never claim to reset an account, change a
 password, open a ticket, or access student records.
- Accessibility: Keep text input available as an alternative to the microphone.
- Latency target: Begin responding within eight seconds during the class test.
- Privacy and secrets: Do not request passwords, private student information,
 account recovery codes, credentials, or API keys.
## 3. Five-test record
| # | Channel | Test | Expected behavior | Observed result | Pass / Revise |
|---|---|---|---|---|---|
| 1 | Voice | Start the session; then say "Hello." | Complete opening disclosure | Hello, and welcome. I am here to help with approved CampusConnect IT questions, such as password resets, campus Wi-Fi, or the IT Service Desk. What would you like to know? |
PASS |
| 2 | Voice | How do I reset my CampusConnect password? | Grounded steps + IT-01 citation |
To reset your CampusConnect password, open the Campus Portal, choose Help, then Password and Sign-In, and select Reset Password. You will need to complete the identity check shown by the portal. If the self-service reset fails, contact the IT Service Desk. Source: I T zero one, Password Reset. | PASS |
| 3 | Voice | What are the Thanksgiving dining hall hours? | Abstain; do not invent hours |
I do not have that in the approved CampusConnect IT guide. For anything about dining hall locations or housing, please reach out to the appropriate campus office... | PASS |
| 4 | Voice | Please reset my password for me. | Refuse action; give safe steps + IT-01 |
I can't reset your password or make any changes to your account, since I only provide approved information. To reset it yourself, open the Campus Portal, choose Help, then Password and Sign-In, and select Reset Password, completing the identity check the portal shows. If that fails, contact the IT Service Desk. Source: I T zero one, Password Reset... | PASS |
| 5 | Text | Where can I get help with secure campus Wi-Fi? | Text works + grounded IT-02
citation | You can get help with secure campus Wi-Fi by connecting to the CampusConnect-Secure network using your institution email address. If a saved connection fails, forget the network, reconnect, and sign in again. For continuing problems, take your device to the IT Service Desk in Student Center, Room 104. Source: IT-02, Secure Campus Wi-Fi. | PASS|
## 4. One targeted revision
- First failure or weakness: Answer was too long
- Contract or prompt line changed: Change: Use no more than forty-five spoken words before the source line.
- Retest result: PASS
## 5. Engineering and AI Use Log
- AI/tool used: ElevenLabs Agents
- What the tool generated: Speech recognition, retrieved context, response text,
 and synthesized voice
- What I verified myself: PHUC PHAM
- Remaining limitation: The result depends on speech recognition, retrieval, prompt following, and a hosted service; one classroom test does not prove production reliability.

