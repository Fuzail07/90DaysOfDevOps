# Day 11 Challenge

## Files & Directories Created
access-code.txt, blueprints.pdf, escape-plan.txt, devops-files.txt, team-notes.txt, app-logs, bank-heist, heist-project, project-config.yaml
## Ownership Changes
changed apps-logs from root:root to berlin:heist-team
changed devops-file.txt from root to tokyo and then to berlin
changed heist-project from root:root to professor:planners
changed project-config.yaml from root:root to professor:heist-team


## Commands Used
groupadd, useradd, chgroup, chown, ls, mkdir.
## What I Learned
1. you can change ownership and group by using chown command
2. user must exist before using chown
3. most chown /chgrp commands needs sudo priviledges.
