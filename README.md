# bash sessions
session support for bash.  Saving is automatic, restoration is manual
## Getting started
Assuming that bash_sessions is installed at `~/lib/bash_sessions`, then add
```bash
source ~/lib/bash_sessions
```
then create a session
```bash
bsr_create project
```
Which will create a session named 'project', and enter the session.
The session name cannot contain the character '/'.
There is currently no
way to leave the session.  After you've killed the shell, you can re-enter the session by
```bash
bsr_enter project
```
If you want to know what sessions are available, you can run `bsr_list`

Currently, the only state that is saved and restored are the bash history, and the
pwd.