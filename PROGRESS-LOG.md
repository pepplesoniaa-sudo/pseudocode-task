# Progress Log - Pseudocoding Assignment

Purpose: a running record of every step - what was done, the evidence that exists, and the checklist.
Rules: newest entry at the bottom. Every claim is CONFIRMED (exact file and line, or pasted output) or
INFERRED. Nothing is invented. Anything missing is marked "Not completed yet". No secrets or credentials.
Owner: the student. This log is maintained by the tutor, but every artifact it points to is the student's
own work.

--------------------------------------------------------------------------------

## 2026-10-15 - Stage 0: Inspect and plan
Done:
- Inspected the Background jobs project read-only. Recorded the language, tools, and every exported
  function in src by file and line only (no behaviour described).
- Explained the whole assignment in plain English and gave a progress checklist.
- Explained 12 key terms with a single, separate shopping-cart example.
- Created the empty output folder tree (folders + one-line README each + a top-level README with
  headings only).
Evidence (CONFIRMED):
- Folder tree of C:\dev\pseudocode-task: 13 folders and 17 README.md files.
- README timestamps are all 10/15/2026 around 8:02 PM (see the file listing in the STEP 2 entry below).
- Language/tools from package.json lines 4-24 and tsconfig.json lines 1-12.
- Exported functions from a grep of src (file and line only).
Status: ACCEPTED by owner. (Owner then moved the folder to C:\dev\pseudocode-task.)

--------------------------------------------------------------------------------

## 2026-10-16 - Stage A1: tokenMatches (slot: permission / token check)

### Entry 1 - STEP 1 lines printed
Done: printed src\adminRoutes.ts lines 12-36 exactly, with line numbers, and nothing else about them.
Evidence (CONFIRMED): tool output showing lines 12-36 verbatim.
Note: test\api.test.ts was deliberately NOT opened (held back to keep the draft independent).

### Entry 2 - owner's notes and reasoning saved (proof of independent reading)
Done: saved the owner's pasted text verbatim, each with a timestamp line at the top.
Files (CONFIRMED by folder listing):
- part-a\own-functions\tokenMatches-notes.md ........ 2368 bytes, 10/16/2026 9:35:09 PM
- part-a\own-functions\tokenMatches-reasoning.md .... 1017 bytes, 10/16/2026 9:35:12 PM
Timestamp line added to each: "Saved (local time): 2026-10-16 21:34:57 +01:00".
These two files are the owner's proof that the reading was done BEFORE any tutor explanation.

### Entry 3 - running log created
Done: created this file (PROGRESS-LOG.md) so the work is recorded on disk, not only in chat.
Timestamp: 2026-10-16 21:36:46 +01:00.

### Entry 4 - STEP 2 lines 1 and 14 printed
Done: printed src\adminRoutes.ts line 1 and line 14 exactly. Stated ONLY whether line 14 passes an
encoding to digest (answer: no - the call is .digest() with empty parentheses). Nothing else about the
function described. Asked the owner to write their own conclusion about "can line 4 break".
Evidence (CONFIRMED): tool output showing line 1 and line 14 verbatim.

--------------------------------------------------------------------------------

## CURRENT CHECKLIST
 #  Item                                        Status             Evidence
 5  A1 own functions (3)                        In progress        1 of 3 started
 5a  - tokenMatches: lines shown                  Verified           lines 12-36 and lines 1,14 printed
 5b  - tokenMatches: notes + reasoning filed      Verified           two timestamped files, sizes listed
 5c  - tokenMatches: owner's conclusion          In progress        awaiting owner text
 5d  - tokenMatches: v1 draft written            Not started        -
 5e  - tokenMatches: hint review                 Not started        -
 5f  - tokenMatches: 3 traces + real run         Not started        -
 5g  - other two own functions                    Not started        -
 6  A2 library functions                          Not started        -
 7  A3 planted bug                                Not started        -
 8  B1 spec + 5 traces                            Not started        -
 9  B2 implementation                             Not started        -
10  C1 AI instruction                             Not started        -
11  C2 reverse-engineered pseudocode              Not started        -
12  C3 ten-input comparison                       Not started        -
13  C4 recording + listener                       Not started        -
14  Final README + post outline + checklist       Not started        -

--------------------------------------------------------------------------------

## 2026-10-16 21:37+ - Housekeeping run (this message)

### Entry 5 - STEP 2 result recorded (line 14)
Done: printed src\adminRoutes.ts line 14. Result: line 14 passes NO encoding to digest - CONFIRMED by
the empty brackets in ".digest()". Nothing else about the function was described.
Evidence (CONFIRMED): tool output of line 14 verbatim.

### Entry 6 - git init and root commit (owner ran it)
Done (owner action): repository initialised at C:\dev\pseudocode-task and a root commit made.
Evidence (CONFIRMED by read-only git):
- Root commit 5e5beb4 "Record progress so far", 17 files changed, 196 insertions.
- Branch master; working tree clean before housekeeping.

### Entry 7 - author email check still pending
Status: Not completed yet. The commit author email was read (owner asked to check it). The owner must
say whether it looks wrong. The tutor will NOT change git config.

### Entry 8 - open Explorer question
Status: Not completed yet. Open question: confirm the editor (Antigravity) has C:\dev\pseudocode-task
open as the workspace folder.

### Entry 9 - housekeeping files created (STEP 3)
Files created (CONFIRMED by listing):
- .gitignore
- evidence\README.md
- PSEUDOCODE-STANDARD.md
- FINAL-AUDIT.md

### Entry 10 - STEP 4 / STEP 5 given
Done: gave the Explorer check list and the reminder of work still owed by the owner.

--------------------------------------------------------------------------------

## CURRENT CHECKLIST (updated)
 #  Item                                        Status             Evidence
 5  A1 own functions (3)                        In progress        1 of 3 started
 5a  - tokenMatches: lines shown                  Verified           lines 12-36 and 1,14 printed
 5b  - tokenMatches: notes + reasoning filed      Verified           two timestamped files
 5c  - tokenMatches: my conclusion on line 4      In progress        awaiting owner text
 5d  - tokenMatches: v1 draft written             Not started        -
 5e  - tokenMatches: hint review                  Not started        -
 5f  - tokenMatches: 3 traces + real run          Not started        -
 5g  - other two own functions                    Not started        -
 6  A2 library functions                          Not started        -
 7  A3 planted bug                                Not started        -
 8  B1 spec + 5 traces                            Not started        -
 9  B2 implementation                             Not started        -
10  C1 AI instruction                             Not started        -
11  C2 reverse-engineered pseudocode              Not started        -
12  C3 ten-input comparison                       Not started        -
13  C4 recording + listener                       Not started        -
14  Final README + post outline + checklist       Not started        -
15  Housekeeping files (.gitignore, evidence, standard, audit)  Verified   created this run
