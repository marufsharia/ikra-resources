

# Project Memory — ikra-resources
> 41 notes | Score threshold: >40

## Safety — Never Run Destructive Commands

> Dangerous commands are actively monitored.
> Critical/high risk commands trigger error notifications in real-time.

- **NEVER** run `rm -rf`, `del /s`, `rmdir`, `format`, or any command that deletes files/directories without EXPLICIT user approval.
- **NEVER** run `DROP TABLE`, `DELETE FROM`, `TRUNCATE`, or any destructive database operation.
- **NEVER** run `git push --force`, `git reset --hard`, or any command that rewrites history.
- **NEVER** run `npm publish`, `docker rm`, `terraform destroy`, or any irreversible deployment/infrastructure command.
- **NEVER** pipe remote scripts to shell (`curl | bash`, `wget | sh`).
- **ALWAYS** ask the user before running commands that modify system state, install packages, or make network requests.
- When in doubt, **show the command first** and wait for approval.

**Stack:** Unknown stack

## 📝 NOTE: 1 uncommitted file(s) in working tree.\n\n## Important Warnings

- **gotcha in hajj.json** — -   }
+  
- 
+     "tasks": [
-   {
+       {
-     "tasks": [

- **gotcha in hajj.json** — -   
+   {
+     "tasks": [
+       {
+         "id": 1,
+        
- **gotcha in hajj.json** — File updated (external): seed/hajj.json

Content summary (173 lines):


## Project Standards

- what-changed in duas_sample.json — confirmed 5x
- convention in hajj.json
- convention in hajj.json
- convention in hajj.json
- convention in hajj.json
- Replaced auth Today — ensures atomic multi-step database operations — confirmed 3x
- what-changed in hajj.json — confirmed 8x
- decision in hajj.json — confirmed 5x

## Recent Decisions

- decision in quran_surahs.json
- decision in duas_sample.json
- decision in duas_sample.json
- decision in hajj.json

## Learned Patterns

- Always: convention in hajj.json (seen 3x)

## Available Tools (ON-DEMAND only)
- `query(q)` — Deep search when stuck
- `find(query)` — Full-text lookup
> Context above IS your context. Do NOT call load() at startup.
