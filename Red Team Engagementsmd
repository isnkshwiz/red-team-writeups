# red-team-writeups
Write-ups and notes for my Red Teaming journey

Red Team Engagements – TryHackMe Write-up

 Date: July 12, 2025  
 Module: Red Team Engagements  
 Room: https://tryhackme.com/room/redteamengagements

📌 Objectives
  Learn the steps and procedures of a red team engagement, including planning, frameworks, and documentation.

| Task № | Title                         |
| ------ | ----------------------------- |
| 1      | Introduction                  |
| 2      | Defining Scope and Objectives |
| 3      | Rules of Engagement           |
| 4      | Campaign Planning             |
| 5      | Engagement Documentation      |
| 6      | Concept of Operations         |
| 7      | Resource Plan                 |
| 8      | Operations Plan               |
| 9      | Mission Plan                  |
| 10     | Conclusion                    |

Task 1: Introduction — Summary
🔑 Key Points:
A successful Red Team engagement requires well-coordinated planning and communication among all involved parties.

This module focuses on:
Components of a Red Team engagement
Planning and documenting a Red Team campaign

🧪 Types of Engagements:
Tabletop Exercises – discussion-based simulation of attack scenarios
Adversary Emulation – mimicking real-world threat actors (e.g., APTs)
Physical Assessment – testing physical security (e.g., building access)

🎯 Learning Objectives:
Understand the components and structure of a Red Team engagement
Learn to plan engagements based on objectives, available resources, and TTPs
Learn how to write documentation that aligns with client goals

ℹ️ Notes:
No prerequisites are required to complete this room



Task 2: Defining Scope and Objectives — Summary
🎯 Key Concepts
🔹 Client Objectives
The foundation of any engagement; must be clearly defined and mutually understood.
Set early during planning and guide all further documentation, operations, and tactics.
Without clear objectives, the engagement will likely be unstructured and ineffective.

🔹 Types of Engagements
Internal/Network Penetration Test
Broader, less specific, uses standard TTPs
Focused Adversary Emulation
Simulates a specific APT group (e.g., APT38 for financial targets)
Tailored tactics based on threat intelligence

🎯 The type of engagement depends heavily on client-defined objectives.

🔹 Scope Definition
The scope defines what is allowed and what is off-limits.
Scope should always be set by the client, though red teams may raise concerns if limitations affect the realism or success of the test.

📌 Scope Examples:
❌ No exfiltration of data
❌ Production servers are off-limits
✅ 10.0.0.8/20 is in scope
❌ 10.0.3.8/18 is out of scope
❌ No system downtime allowed
❌ No exfiltration of PII

🧠 Red Team Perspective
Understand the implications of the objectives and scope, not just the literal text.
Be dynamic: engagement planning often begins just from the initial objectives and scope.
Think ahead: how would your team realistically execute an engagement within those boundaries?

🔑 Takeaway
Client Objectives = Strategic Direction
Scope = Tactical Boundaries
Both must be well-defined to enable a successful, safe, and realistic engagement.

Task 2 (Part 2) — Example Analysis (English)
🎯 Client: Global Enterprises
🔹 Objectives:
Identify system misconfigurations & network weaknesses
Focus on external-facing systems
Assess EDR (Endpoint Detection and Response) effectiveness
Evaluate SIEM, detection, and response capabilities
Test segmentation between DMZ and internal servers
Allow white cards under conditions
Simulate data exposure & exfiltration with fake data

🔹 Scope:
❌ No system downtime
❌ DDoS/DoS strictly forbidden
❌ No real malware (ransomware, etc.)
❌ No PII exfiltration – use dummy data
✅ 10.0.4.0/22 is in scope
❌ 10.0.12.0/22 is out of scope
❌ *.bethechange.xyz – prohibited
✅ *.globalenterprises.thm – allowed
⚠️ DMZ and critical systems will be monitored closely

❓ Questions:
Q1: What CIDR range is permitted to be attacked?
✅ 10.0.4.0/22
Q2: Is the use of white cards permitted?
✅ Yes, depending on downtime and duration
Q3: Are you permitted to access *.bethechange.xyz?
❌ No



Task 3: Rules of Engagement — Summary (English)
🔑 Key Concepts:
Rules of Engagement (RoE) is the first official and legally binding document in a Red Team engagement.

It formalizes:
Client objectives
Scope
Engagement expectations
Serves as a contract between the client and the red team.
May be accompanied by external legal agreements, like NDAs.

🧾 Why RoE matters:
Sets clear, legal expectations
Prevents miscommunication
Protects both parties during the engagement

🧱 Common RoE Sections:
| Section Name                               | Description                                         |
| ------------------------------------------ | --------------------------------------------------- |
| **Executive Summary**                      | High-level overview and authorization context       |
| **Purpose**                                | Why the RoE exists                                  |
| **References**                             | Standards/frameworks used (e.g., ISO, HIPAA)        |
| **Scope**                                  | What is allowed or restricted                       |
| **Definitions**                            | Clarifies technical/legal terms                     |
| **Rules of Engagement & Support**          | Obligations, expectations, technical behavior       |
| **Provisions**                             | Exceptions or additional notes                      |
| **Requirements, Restrictions & Authority** | Defines red team’s responsibilities and permissions |
| **Ground Rules**                           | What red team can/cannot do                         |
| **Resolution/Points of Contact**           | List of essential contacts and escalation paths     |
| **Authorization**                          | Formal statement of legal approval                  |
| **Approval**                               | Final signatures from both parties                  |
| **Appendix**                               | Additional supporting details                       |

🧠 Notes:
RoE is just the starting point — future planning documents will expand on it.
Treat RoE as a legal contract, not a tactical plan.

Answers:
Q1: How many explicit restrictions are specified?
🅰️ 3 explicit restrictions
Use of white cards is strictly prohibited
Any form of DDoS or DoS is prohibited
Attacks against any system within 192.168.1.0/24 is prohibited

Q2: What is the first access type mentioned in the document?
🅰️ Phishing
(Under "Access Types" section)

Q3: Is the red team permitted to attack 192.168.1.0/24? (Y/N)
🅰️ No (N)
(That range is explicitly prohibited)



Task 4: Campaign Planning — Summary 
🔑 Key Concepts:
Campaign planning shifts from business-level planning (objectives, RoE) to technical execution planning.
It defines how and what the red team will do during the engagement.
Every red team may use a different structure, but this room uses a 4-part planning system adapted from military ops.

📦 4 Types of Campaign Plans:
| Plan Type            | Purpose                              | Includes                                      |
| -------------------- | ------------------------------------ | --------------------------------------------- |
| **Engagement Plan**  | High-level technical overview        | CONOPS, resources, personnel, timeline        |
| **Operations Plan**  | Detailed breakdown of the engagement | Operator roles, known intel, responsibilities |
| **Mission Plan**     | Execution plan with specifics        | Commands, timing, assigned operator           |
| **Remediation Plan** | What happens *after* the campaign    | Reports, debriefs, remediation guidance       |

🧠 Notes:
These documents ensure clear communication, precision, and legal & technical traceability.
The Mission Plan is the most hands-on, while the Engagement Plan is strategic.



Task 5: Engagement Documentation — Summary
🔑 Key Concepts:
Engagement documentation is the formalization of the ideas outlined in campaign planning.
Not every plan requires an official document — some can be informal (e.g., email confirmation).
This task explains the technical components of each of the four core plans:
Engagement Plan
Operations Plan
Mission Plan
Remediation Plan

📄 Engagement Plan Components:
| Component         | Purpose                                                                                                         |
| ----------------- | --------------------------------------------------------------------------------------------------------------- |
| **CONOPS**        | High-level, non-technical summary of how the red team will meet the client’s objectives and approach the target |
| **Resource Plan** | Lists **timelines** and all needed **resources** (people, hardware, cloud tools, etc.)                          |

⚙️ Operations Plan Components:
| Component                  | Purpose                                                                                          |
| -------------------------- | ------------------------------------------------------------------------------------------------ |
| **Personnel**              | Defines required team members and skillsets                                                      |
| **Stopping Conditions**    | Conditions that would trigger stopping the engagement (e.g., system failure, detected intrusion) |
| **RoE** *(optional)*       | May restate or reference the original Rules of Engagement                                        |
| **Technical Requirements** | What knowledge/tools the team needs to successfully complete the engagement                      |

🧨 Mission Plan Components:
| Component                          | Purpose                                                             |
| ---------------------------------- | ------------------------------------------------------------------- |
| **Command Playbooks** *(optional)* | Specific commands, tools, and usage logic — helpful for large teams |
| **Execution Times**                | Schedule or timing for executing actions                            |
| **Responsibilities/Roles**         | Assigns who does what, and when                                     |

🛠️ Remediation Plan (optional) Components:
| Component                    | Purpose                                                                           |
| ---------------------------- | --------------------------------------------------------------------------------- |
| **Report**                   | Full summary of what happened and what was discovered                             |
| **Remediation/Consultation** | How the client should fix the issues — either in report or in a follow-up meeting |



Task 6: Concept of Operations (CONOPS) — Summary
🔑 Key Concepts 
CONOPS is a high-level overview of the red team engagement.
Serves as a bridge between business/client understanding and red team's operational planning.
Should be semi-technical — understandable to non-technical readers, but still detailed.
Used as a reference point for all further planning (Operations Plan, Mission Plan, etc.)

📄 Standard CONOPS Components:
Client name
Service provider
Timeframe
General objectives/phases
Additional training goals (e.g., exfiltration)
High-level tools/techniques
Emulated threat group (if applicable)

Answers:
Q1: How long will the engagement last?
🅰️ One month

Q2: How long is the red cell expected to maintain persistence?
🅰️ Three weeks

Q3: What is the primary tool used within the engagement?
🅰️ Cobalt Strike



Task 7: Resource Plan — Summary (English)
🔑 Key Concepts:
The Resource Plan is part of the Engagement Plan, focused on logistics and requirements.
It extends the CONOPS with exact dates, roles, and resource needs.
Unlike CONOPS, it is not a narrative — written as bullet points or structured lists.

📋 Key Sections of a Resource Plan:
🏷️ Header Info:
Author (who wrote the plan)
Customer name
Dates of engagement activities

📅 Engagement Dates:
Engagement Start/End
Reconnaissance
Initial Compromise
Post-Exploitation / Persistence
Other key dates

📘 Knowledge Required (Optional):
For Recon
For Compromise
For Post-Exploitation

📦 Resources Required:
Personnel (number of red team members, roles)
Hardware (laptops, tools, physical devices)
Cloud (infrastructure needed)
Miscellaneous (VPNs, accounts, etc.)

🧠 Note:
The plan should be clear, specific, and to the point.
Include only what is necessary — not too detailed, not too vague.

✅ Answers:
When will the engagement end? (MM/DD/YYYY)
11/14/2021
📌 Found in: ENGAGEMENT DATES: 10/12/21 - 11/12/21
What is the budget the red team has for AWS cloud cost?
$1000
📌 From: “Red Cell is requesting a budget of $1000 for AWS cloud costs”
Are there any miscellaneous requirements for the engagement? (Y/N)
N (No)
📌 From: “Miscellaneous: n/a”



Task 8: Operations Plan — Summary 
🔑 Key Concepts:
The Operations Plan gives detailed instructions on how the engagement will be executed.
It expands the CONOPS and may optionally include or reference the Rules of Engagement (RoE).
Written in bullet format like the Resource Plan.

📋 Key Sections of an Operations Plan:
| Section                              | Purpose                                                          |
| ------------------------------------ | ---------------------------------------------------------------- |
| **Header**                           | Includes authors and basic info                                  |
| **Personnel Writing**                | Who created the document                                         |
| **Dates**                            | Engagement timeline                                              |
| **Customer**                         | Client name                                                      |
| **Halting/Stopping Conditions**      | When/why red team should stop the campaign                       |
| **Assigned Personnel**               | Who’s responsible for which tasks                                |
| **Planned TTPs/Attacks**             | Specific techniques and actions to be used                       |
| **Communications Plan**              | How the red team will communicate internally and with the client |
| **Rules of Engagement** *(optional)* | If not already included in a separate RoE document               |

Communications Plan – Examples:
vectr.io — Structured, visual engagement tracking
Email — Formal communication, status updates
Slack — Real-time, team chat coordination

✅ Answers:
What phishing method will be employed during the initial access phase?
Spearphishing via mshta and typosquatted domains
📌 Found in the Planned TTPs and Attacks section.
What site will be utilized for communication between the client and red cell?
vectr.io
📌 Stated clearly in the Communications Plan: “the red cell will utilize vectr.io to communicate…”
If there is a system outage, the red cell will continue with the engagement. (T/F)
False
📌 From Halting/Stopping Conditions: “In the event of a system outage all engagement operations will cease”



Task 9: Mission Plan — Summary
🔑 Key Idea:
The Mission Plan is an internal red team document that outlines the exact actions for operators to perform. It is based on the previous plans (like CONOPS and Operations Plan) but written from the operator’s perspective.
Unlike the Operations Plan (business/client-facing), the Mission Plan is tactical and focused on step-by-step red team execution.

📋 Minimum Components:
| Component                     | Purpose                                                                  |
| ----------------------------- | ------------------------------------------------------------------------ |
| **Objectives**                | What goals need to be achieved                                           |
| **Operators**                 | Who is responsible for each action                                       |
| **Exploits/Attacks**          | What tools/techniques will be used                                       |
| **Targets**                   | What users, machines, or infrastructure are being attacked               |
| **Execution Plan Variations** | What to do if Plan A doesn’t work — alternatives or branching strategies |

🧠 Notes:
The structure is flexible — could be a full document or even a simple internal email.
Key: Clear task assignments and procedures for all operators.

✅ Answers:
When will the phishing campaign end? (mm/dd/yyyy)
10/23/2021
📌 Stated clearly in:
“Phishing campaign will last from 10/13/2021–10/23/2021.”
Are you permitted to attack 10.10.6.78? (Y/N)
N
📌 That IP is not listed among the allowed targets. Only 10.10.6.29 and named assets like BEAN-MAIL, BEAN-PROD, and bethebean.com are mentioned.
Unless explicitly included in the scope, 10.10.6.78 is out of scope.
When a stopping condition is encountered, you should continue working and determine the solution yourself without a team lead. (T/F)
False
📌 The plan says:
“In the event of any varying events… immediately contact a team lead and discuss how to continue.”

✅ Summary:
Planning and documentation are critical to a successful red team engagement — don’t skip them.
Every red team uses its own formats and processes — there is no strict universal standard.
This module is a framework, not a rulebook. It helps you understand key ideas.
Your main goal in any engagement is to meet the client’s objectives clearly and professionally.
Clear planning = efficient execution + better results + fewer misunderstandings.


🛑 END OF MODULE: Red Team Engagements

