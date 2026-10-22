\# HACKATHON PROJECT - AGENT CONSTITUTION



\## 1. PROJECT AUTHORITY



The following documents define the approved project:



1\. docs/PROJECT\_BLUEPRINT.md

2\. docs/REQUIREMENTS.md

3\. docs/ARCHITECTURE.md

4\. docs/API\_CONTRACT.md

5\. docs/DATABASE\_CONTRACT.md

6\. docs/UI\_CONTRACT.md

7\. docs/DECISIONS.md



These documents are authoritative.



Do not invent requirements that are not present in these documents.



\---



\## 2. SCOPE CONTROL



Before implementing any requested feature:



1\. Determine whether it exists in REQUIREMENTS.md.

2\. Determine whether it exists in PROJECT\_BLUEPRINT.md.

3\. Determine whether it fits the approved architecture.



If the requested functionality is outside the approved scope:



STOP.



Do not implement it automatically.



Report:



\- Requested feature

\- Why it is outside scope

\- Files that would be affected

\- Architecture impact

\- Estimated complexity

\- Potential risks



Then ask the user for explicit approval.



Never silently expand project scope.



\---



\## 3. ARCHITECTURE CONTROL



The approved architecture must not be changed without permission.



Do not:



\- replace frameworks

\- replace databases

\- replace authentication systems

\- change API architecture

\- change folder architecture

\- introduce new major dependencies



without explicit approval.



Small implementation decisions may be made autonomously if they do not affect the approved architecture.



\---



\## 4. FRONTEND/BACKEND SEPARATION



Frontend and backend communicate only through approved contracts.



Frontend developers must use:



docs/API\_CONTRACT.md



Backend developers must implement:



docs/API\_CONTRACT.md



Neither side may arbitrarily change the contract.



If a contract change is required:



STOP.



Explain:



\- current contract

\- proposed change

\- reason

\- frontend impact

\- backend impact

\- testing impact



Ask for approval.



\---



\## 5. API CONTRACT



Every API must define:



\- endpoint

\- HTTP method

\- authentication

\- request headers

\- request body

\- response body

\- success status

\- error status

\- validation rules

\- error format



Use the exact structures defined in API\_CONTRACT.md.



Do not invent response formats.



\---



\## 6. BACKEND RULES



Backend code must:



\- follow the approved architecture

\- use service/controller/repository separation where specified

\- validate input

\- return standardized responses

\- handle errors consistently

\- never expose secrets

\- never expose internal implementation details



Backend must not modify frontend code unless explicitly requested.



\---



\## 7. FRONTEND RULES



Frontend code must:



\- follow UI\_CONTRACT.md

\- consume APIs according to API\_CONTRACT.md

\- not assume undocumented backend behavior

\- handle loading states

\- handle error states

\- handle empty states

\- handle successful states



Frontend must not modify backend implementation.



\---



\## 8. TESTING RULES



Every feature must have appropriate tests.



Before considering a feature complete:



1\. Run tests.

2\. Run lint/static analysis.

3\. Run build/type checks where applicable.

4\. Fix failures.

5\. Report results.



Never claim a feature works without verification.



\---



\## 9. MAIN BRANCH RULE



main represents stable, tested functionality.



Never directly modify main.



Never force push main.



Before merging into main:



1\. Feature implementation complete.

2\. Tests pass.

3\. Integration test passes.

4\. Scope check passes.

5\. Contract check passes.

6\. Code review passes.



\---



\## 10. POST-MERGE VERIFICATION



After a commit is merged into main and pulled:



STOP before continuing with unrelated development.



Run:



1\. dependency installation check

2\. build

3\. unit tests

4\. integration tests

5\. smoke tests



If any test fails:



STOP.



Identify the regression.



Do not continue implementing unrelated features until the issue is reported.



\---



\## 11. SECURITY



Never:



\- expose API keys

\- commit .env

\- commit credentials

\- hardcode passwords

\- hardcode tokens

\- disable authentication for convenience

\- bypass validation



Use environment variables.



\---



\## 12. CHANGE CONTROL



If a requested change affects:



\- architecture

\- database schema

\- API contract

\- authentication

\- project scope

\- major dependencies

\- deployment architecture



approval is mandatory.



\---



\## 13. AI BEHAVIOR



Do not blindly execute user instructions.



First determine:



\- scope

\- architecture impact

\- dependency impact

\- contract impact

\- testing impact



For safe implementation tasks, proceed.



For architectural or scope-changing tasks, ask permission.



\---



\## 14. TOKEN EFFICIENCY



Do not repeatedly explain the entire project.



Read the relevant document only.



Use progressive disclosure.



Prefer concise summaries.



Do not load unrelated documentation when solving a focused task.

