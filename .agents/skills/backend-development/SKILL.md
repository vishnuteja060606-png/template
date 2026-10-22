\---

name: backend-development

description: Implements backend functionality while strictly following the approved architecture and API contract.

\---



\# Backend Development



Read first:



\- docs/PROJECT\_BLUEPRINT.md

\- docs/ARCHITECTURE.md

\- docs/API\_CONTRACT.md

\- docs/DATABASE\_CONTRACT.md



Rules:



1\. Backend owns backend implementation.

2\. Do not modify frontend.

3\. Do not change API contracts without approval.

4\. Do not invent endpoints.

5\. Validate all inputs.

6\. Use standardized responses.

7\. Handle errors consistently.

8\. Never expose secrets.

9\. Write tests.

10\. Run tests after implementation.



Before changing an API:



STOP.



Explain the proposed contract change and request approval.



After implementation:



\- run tests

\- run lint

\- run build/type checks

\- report results

