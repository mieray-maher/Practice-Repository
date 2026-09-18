# Reflection Questions

Answer these as you go — don't wait until the end. Some answers only exist
*after* you've done a step, so fill this in progressively.

Your answers will be reviewed alongside your code. Generic or copy-pasted
answers (that don't reference your actual output) will be sent back for
revision.

---

## Part 1 — Before touching anything (after reading CONTRIBUTING.md)

**1. What branch naming convention does this project use? Give an example
branch name you plan to use.**

> docs is the convention this project uses, e.g. docs/add-mieray-maher

**2. What commit message format is required? Write the exact commit message
you plan to use for your change.**

> the format required is <type>: <short summary>, the exact commit message is: "docs: adding my name to CONTIBUTORS markdown file"

**3. Does this project expect a linked issue before opening a PR, or is a PR
description enough?**

> Yes, this project expected a linked issue before opening a PR so that the PR description can explain the change and linked issue 

---

## Part 2 — After forking and cloning

**4. Paste the output of `git remote -v` from your local clone. Which remote
is `origin` and which is `upstream`, and why does that distinction matter?**

> The output:
origin  https://github.com/mieray-maher/Practice-Repository.git (fetch)
origin  https://github.com/mieray-maher/Practice-Repository.git (push)
upstream        https://github.com/IbrahimYasserM/Practice-Repository.git (fetch)
upstream        https://github.com/IbrahimYasserM/Practice-Repository.git (push)

origin is my fork, the copy of the repo but uner my own github.
upstream is the original repo of the task, I can pull from it so my fork and the upstream can stay in sync.
that distinction matter to identify which one I have access to. 

---

## Part 3 — After making your change

**5. Paste the output of `git log --oneline -3`. Do your commit message(s)
follow the convention from `CONTRIBUTING.md`?**

> The output: 
716575e (HEAD -> docs/add-mieray-maher, origin/docs/add-mieray-maher) Merge remo
te-tracking branch 'upstream/conflict-practice' into docs/add-mieray-maher
c8e1831 docs: adding my name to CONTIBUTORS markdown file
983499c (upstream/conflict-practice) Add Mohammed Nasser to CONTRIBUTORS.md

yes, it does.

---

## Part 4 — After hitting the seeded merge conflict

**6. What caused the conflict? Which file and lines were involved?**

> Both my branch and the upstream/conflict-practice branch added a line at the same location in the file so git couldn't automatically merge them because both changes touched the exact same lines.

**7. How did you resolve it — what did you keep, remove, or combine, and why?**

> I used the editor's "Accept Both Changes" option, then removed these leftover lines (<<<<<<<, =======, >>>>>>>) so the file cleanly listed all three names.
---

## Part 5 — After opening your PR

**8. Paste your PR link. How many commits and how many files changed does
your PR show?**

> PR link: https://github.com/IbrahimYasserM/Practice-Repository/pull/13
it shows 4 commits and 2 files changed

---

## Part 6 — Final reflection

**9. What's one thing about this workflow that surprised you, confused you,
or felt different from what you expected going in?**

> I think that this is my first PR and also first time to use the conventions

**10. If a teammate asked you to explain the difference between `fork`,
`clone`, `origin`, and `upstream` in one or two sentences each, what would
you say?**

> A fork is my own copy of someone else's repo made on github itself. A clone is downloading a copy of a repo (mine or someone else's) from github onto my local computer, so I can actually edit files and run git commands on it. Origin is just the default name git gives to the remote repo. An upstream is a remote I add manually through a git command to point at the original repo.
