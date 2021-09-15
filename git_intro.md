# Git and Version Control

## What?
"Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency."

git is the software (we installed this through the XCode command line tools yesterday)

distributed = lives on more than one computer
versions in software: version 1.0, v1.5, version 2.0
version control = tracking changes to version
version control system: system for systematically traacking changes
- Crude version: resume.pdf, resume2.pdf, resume_FINAL.pdf
- Little more sophistication: track changes in a google doc
	- which author made which change(s) when and in what order
	- what's lacking here: WHY that change was made and if new users of that document need to know anything else specifically
- Git 
	- git's internals (kinda) work like a blockchain.
	- Example: in accounting, if you make a mistake, you don't delete it, you add another fact to the ledger that says "last entry to be ignored"
	- string of facts (even a mistake is a fact)
	- before computers, accounting ledgers were always kept in pen.
	- with git we're tracking all changes to any line of code/text in any file we're tracking.
- Analogy time for Git
	- Git is a permanent record with a time machine that has the (	ability to branch/navigate/merge parallel timelines)

- When we enable git, we're enabling those capabilities on an entire folder/directory. Subfolders can be tracked and all files can be tracked. For specific scenarios, like a file with a password in it, we'll specifically tell git to ignore certain sensitive files

## So What?
- A rather large trend in Data Science is adopting methods, tools, and workflows that are established best practices in software engineering.
- Tracking changes in a piece of analysis w/ hundreds/thousands of lines of code is much easier in git than google docs.

## Now What?
- turn regular ol' directories into git repositories. All repositories are folders, but not all folders are repos.
- git runs on a computer (your laptop, your desktop, or servers)
- a permanent record with a time machine is pretty cool... but what happens if your git enabled folder (your git repo) only lives on your laptop
- It's on US to ensure that your git repos are backed up. (GitHub makes this really easy and cheap)


## Some Concepts
- "Commits" are save points. Each commit is one or more changes to one or more files. 

- adding files/changes is like putting letters in an envelope.
- making a commit is like SEALING that envelope with a timestamp and your personal signature/stamp
- pushing means to upload one or more commits (any un-pushed commits will be pushed/uploaded)

BTW:
- completely avoid making repos inside of repos.

## Best Practices
- Make a new repo locally(laptop) and remotely (on github) for each new project
- One time setup: setup your repo locally and remotely.
- Wisdom: one repo per project. 

## Here's our workflow moving forward (best practices)
- Daily Workflow:
	- Do work (creating file(s), editing file(s), deleting stuff in a repo)
	- `git add .`
	- `git commit` then type out a meaningful commit message to tell a story
	- `git push`
- Make commits and push before lunch/end of the day (or any time you close laptop)
- Guidance:
	- If your code ain't in source control (on GitHub), it doesn't
 exist
 	- Commit early and commit often. Commiting after you add a feature or finish a stage of the DS pipeline. 
 	- Be sure to push every day.
