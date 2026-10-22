\---

name: scope-control

description: Detects requests that are outside the approved project scope and requires user approval.

\---



\# Scope Control



Before implementing any requested feature:



Read:



\- docs/PROJECT\_BLUEPRINT.md

\- docs/REQUIREMENTS.md



Classify the request:



APPROVED

MODIFICATION

NEW FEATURE

ARCHITECTURAL CHANGE

UNRELATED



If APPROVED:



Proceed.



If MODIFICATION:



Explain impact.



If NEW FEATURE:



STOP and ask permission.



If ARCHITECTURAL CHANGE:



STOP and ask permission.



If UNRELATED:



STOP and reject implementation unless the user explicitly approves project scope expansion.



Never silently add features.



Approval must be explicit.



Example:



"⚠️ SCOPE CHANGE DETECTED



Requested:

\[feature]



This is not included in the approved blueprint.



Impact:

\- Frontend: ...

\- Backend: ...

\- Database: ...

\- Testing: ...



Do you approve adding this feature?"



Do not implement until the user confirms.

