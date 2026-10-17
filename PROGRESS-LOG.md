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

--------------------------------------------------------------------------------

### Entry 11 - STEP 6 commit (housekeeping)
Done: staged and committed ONLY the step 2-3 files. Exactly one git add and one git commit, as allowed.
Command run: git add PROGRESS-LOG.md .gitignore evidence PSEUDOCODE-STANDARD.md FINAL-AUDIT.md
Command run: git commit -m "Add housekeeping files and catch up progress log"
Evidence (CONFIRMED by read-only git):
- Commit a0b0b56, 5 files changed, 109 insertions.
  Files: .gitignore, FINAL-AUDIT.md, PSEUDOCODE-STANDARD.md, PROGRESS-LOG.md, evidence/README.md.
- Author/email: Sonia Pepple [pepplesoniaa@gmail.com] - same as root commit 5e5beb4.
- No git push was run. "git add ." was NOT used.
Note: this Entry 11 was appended AFTER the commit, so PROGRESS-LOG.md now carries one uncommitted
change (the entry you are reading). Expected; it will go into the next housekeeping commit.

--------------------------------------------------------------------------------

## 2026-10-17 01:12 +01:00 - Stage A1 STEP 1 (partial): file conclusion and v1 draft

### Entry 12 - owner's tokenMatches conclusion filed (copy only)
Done: created the new file below with the owner's pasted conclusion, verbatim, first line as the
requested timestamp. No wording was changed by the tutor. No existing file was edited or deleted.
Files (CONFIRMED by listing):
- part-a\own-functions\tokenMatches-conclusion.md ... 2641 bytes, 10/17/2026 1:10:57 AM (NEW)
- first line: "Timestamp: 2026-10-17 00:43:31 WAT (Africa/Lagos)"

### Entry 13 - owner's tokenMatches v1 draft NOT received
Status: Not completed yet. The STEP 1 message contained the placeholder "[PASTE MY V1 PSEUDOCODE HERE]"
but no v1 text. The existing template part-a\own-functions\tokenMatches.md (822 bytes,
10/15/2026 10:46:20 PM) is UNCHANGED. Per the no-invention rule the tutor did not write or guess it.
Blocker: owner must paste the v1 pseudocode. Because the v1 file is missing, the requested
"git add part-a" + "git commit -m ..." for STEP 1 was DELIBERATELY NOT run yet.

### Entry 14 - no other project touched
Done: only C:\dev\pseudocode-task was written. The Background jobs project (read-only, src only) was
not edited. No app, worker, database or test was run. test\api.test.ts was not opened. No secrets
printed. No git push.

### Checklist after this entry
- 5c tokenMatches conclusion ............ Verified  (new file, 2641 bytes)
- 5d tokenMatches v1 draft .............. Not started / blocked (v1 text not pasted)
- STEP 1 git commit .................... Not completed yet (waiting on v1)
- STEP 2 (confirm helper) .............. Not started yet this run
- STEP 3 (hints on v1) ................. Not started yet this run

--------------------------------------------------------------------------------

## 2026-10-17 01:25 +01:00 - Stage A1 STEP 1 completed: v1 draft filed, committed

### Entry 15 - owner's v1 pseudocode saved over the template (copy only)
Done: replaced part-a\own-functions\tokenMatches.md with the owner's pasted v1 text, verbatim (the old
headings-only template is gone). The tutor did not write, complete or correct any pseudocode; the text
is the owner's own.
Files (CONFIRMED by listing after the write):
- part-a\own-functions\tokenMatches.md ............ 1541 bytes, 10/17/2026 1:25:14 AM (was 822 bytes)
- part-a\own-functions\tokenMatches-conclusion.md . 2641 bytes, 10/17/2026 1:10:57 AM
Note (honesty): the very first write attempt to tokenMatches.md was malformed (a duplicated FAILS WHEN
block). It was immediately rewritten from the owner's pasted text. The logged size/time above is the
corrected final file. No source file and no existing user file other than the specified template was
touched.

### Entry 16 - git add + commit (as instructed)
Commands run (exactly as instructed, no "git add ." and no push):
- git add part-a
- git commit -m "Add tokenMatches conclusion and v1 draft"
Evidence (CONFIRMED by git show --stat HEAD):
- Commit 9ac8855, 2 files changed, 50 insertions(+), 26 deletions(-).
- new file: part-a/own-functions/tokenMatches-conclusion.md
- modified: part-a/own-functions/tokenMatches.md
- Author/email: Sonia Pepple <pepplesoniaa@gmail.com> (same as prior commits).
- Git note: "LF will be replaced by CRLF" warnings only; no error.
- git status after commit: only " M PROGRESS-LOG.md" (this entry, expected).

### Checklist after this entry
- 5d tokenMatches v1 draft .............. Verified  (filed + committed)
- STEP 1 ............................... Verified  (conclusion + v1 both filed, commit 9ac8855)
- STEP 2 (confirm helper, line 14) ..... Not started yet this run
- STEP 3 (hints on v1) ................. Not started yet this run

### Next
STEP 2 only: print src\adminRoutes.ts line 14 exactly, state only whether it passes an encoding to
digest, then ask the owner a question. Then STOP.

--------------------------------------------------------------------------------

## 2026-10-17 01:30 +01:00 - Stage A1 STEP 2: confirm the helper (read only)

### Entry 17 - src\adminRoutes.ts line 14 printed
Done: read the Background jobs project read-only and printed line 14 exactly, with line number, and
added only one statement: whether it passes an encoding to digest. Answer: NO encoding is passed
(the brackets in ".digest()" are empty). Nothing else about the function was described. No test file
was opened; no value or credential was printed.
Evidence (CONFIRMED): tool output of src\adminRoutes.ts line 14 verbatim:
  const sha256 = (value: string) => createHash("sha256").update(value).digest();
Asked the owner to write, in their own words, what this settles about their "assumption to verify".
The tutor did NOT say what it settles (hint-only rule).

### Checklist after this entry
- 5e tokenMatches hint review .......... In progress (STEP 2 question asked)
- STEP 2 ............................... Verified (line 14 printed, encoding question stated)
- STEP 3 (hints on v1) ................. Not started yet

--------------------------------------------------------------------------------

## 2026-10-17 01:34 +01:00 - Stage A1 STEP 2 (this run): state check + helper line 14

Permissions for this run: read-only on the Background jobs project src; write ONLY to append to this
PROGRESS-LOG.md; NO git writes.

### Entry 18 - current state verified with a real listing
Done: listed the two files and checked tokenMatches.md for a stray square bracket.
Files (CONFIRMED by listing):
- part-a\own-functions\tokenMatches.md ............ 1541 bytes, 10/17/2026 1:33:54 AM
- part-a\own-functions\tokenMatches-conclusion.md . 2641 bytes, 10/17/2026 1:10:57 AM
Bracket check (CONFIRMED two ways):
- Working file: 28 lines; first line "`tokenMatches` — v1 pseudocode"; last line ends "...`tokenMatches`
  alone."; a scan found NO "[" or "]" on any line.
- Committed content at commit 9ac8855: 28 lines; same first and last lines; NO bracket on any line.
- Answer to the owner's question: NO stray square bracket, on no line.
Note (honesty): tokenMatches.md mtime is now 1:33:54 AM (the commit was 1:25:23 AM), so the file was
touched after the commit - but its content still matches the committed version (28 lines, same first
and last lines). INFERRED: an editor touched it without changing the text. Not edited by the tutor.

### Entry 19 - src\adminRoutes.ts line 14 printed (read only)
Evidence (CONFIRMED): src\adminRoutes.ts line 14 verbatim:
  const sha256 = (value: string) => createHash("sha256").update(value).digest();
Statement made (only one): line 14 passes NO encoding to digest (".digest()" brackets are empty).
Then asked the owner to write, in their own words, what this settles about the "assumption to verify"
at the bottom of their v1. The tutor did NOT say what it settles. No test file was opened. No value or
credential printed.

### Entry 20 - STEP 3 held (gate not met)
Status: Not started yet / blocked. The owner's STEP 3 text says to give the 7 hint questions "after I
say my v2 conclusion is saved". That has not happened yet, so no hint questions were given. Awaiting
the owner's STEP 2 answer and their v2-conclusion message.

### Checklist after this entry
- 5d tokenMatches v1 draft ............. Verified (filed + committed, 9ac8855)
- 5e tokenMatches hint review .......... In progress (STEP 2 question asked, answer awaited)
- STEP 2 ............................... Verified (line 14 printed, no-encoding stated)
- STEP 3 (7 hint questions on v1) ...... Not started yet / blocked on owner's v2-conclusion message
- 5f tokenMatches 3 traces + real run .. Not started
- Nice to have: nothing new this run. Block on: owner's v2 conclusion + STEP 2 answer.
