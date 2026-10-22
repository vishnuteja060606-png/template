\---

name: testing

description: Validates project functionality, integration, regressions, and main-branch stability.

\---



\# Testing Skill



Testing responsibilities:



\## Unit Testing



Verify individual functions.



\## Integration Testing



Verify:



Frontend

→ API

→ Backend

→ Database



\## Regression Testing



Verify previously working features after new changes.



\## Smoke Testing



Verify the application starts and core functionality works.



\## Main Branch Verification



After main receives a new commit:



1\. Pull latest main.

2\. Install dependencies if required.

3\. Run build.

4\. Run unit tests.

5\. Run integration tests.

6\. Run smoke tests.



If anything fails:



STOP.



Report:



\- failing test

\- suspected cause

\- affected feature

\- commit responsible if identifiable



Do not continue unrelated implementation until the issue is addressed.

