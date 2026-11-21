# Coach and Admin Guide
Thank you for helping to maintain our GitHub organization! This guide will help you understand how. 

**Internal. For Break Through Tech coaches, staff and GitHub admins only.**

## First, read the README.
For real. It's [here](https://github.com/Break-Through-Tech/.github/blob/main/profile/README.md).

## Next, read the Contributing guide.
[This](https://github.com/Break-Through-Tech/.github/blob/main/contributing.md) will help you understand our best practices and how to help support Fellows in contributing effectively.

*Now that we've got that out of the way...*

## First Principle: A real-world organization
We've set up our GitHub organization to work like one at a real company using GitHub Enterprise. Access is limited to what each person needs, changes go through pull requests and reviews, the main branch is protected, and only approved tools are connected. **We do this on purpose**. Our goal is to give Fellows a real-world, work-like experience, so how the organization runs is part of what they learn. The habits they build here, like working on branches, writing clear pull requests, reviewing each other's code, and keeping secrets out of the repo, are the same ones they'll be expected to have on their first engineering team.

## Your role (and responsibility)
Your role is a lot like a **maintainer** of an open source project. Fellows are the contributors, and you keep the project healthy for them: you welcome them in, show them how things work, review their contributions, and hold the line on the guidelines, kindly and consistently. When you enforce a rule, explain why it exists. That's often the most valuable lesson in the moment.

**Your core responsibility is to help keep the organization safe, secure, and running effectively:**

- **Safe** means a respectful, welcoming place to learn. Model good review etiquette, keep feedback about the code and not the person, and make sure Fellows know they can report a mistake without getting in trouble.
- **Secure** means nothing gets in or out that shouldn't. No passwords, API keys, personal information, or confidential data in any repo, tools connected only to a single repo, and quick action on anything that looks wrong (see Red flags).
- **Running effectively** means the work keeps moving. Issues and Projects boards stay current, pull requests get reviewed promptly, branches get cleaned up, and each team's README and write-up are complete by the end of the program.

**This is a shared responsibility.**
Like maintainers in a large organization, coaches share responsibility for the whole organization, not just their own repos. That's why the Coaches team has Admin access on every project repo. If you notice a problem in another team's repo, like an exposed key, a tool connected to "All repositories," or a pull request that's been stuck for days, don't assume someone else has it. Fix it if it's urgent, and let that team's coach know. Cover for each other when someone is out, and keep teams consistent so Fellows get the same answer whichever coach they ask.

## Your access

You're a member of the **Coaches** team in our GitHub organization. The team has **Admin** access on every project repo, so you can install approved tools without waiting for an org owner. 

You have access to every project repo (not just the repos for the teams you supervise). Work mainly in your own teams' repos. If you would like to make a change in another coach's repo, let them coach know.

As a repo Admin, you **can**:

- Connect an approved tool to a project repo, and remove it
- Review, approve, and merge pull requests
- Add or remove Fellows and Challenge Advisors on a repo
- Manage Projects boards and repo settings

You **can't** (these stay with org owners):

- Connect anything to the whole organization
- Approve OAuth apps (apps that can't be limited to a single repo)
- Make a repo private, or delete or transfer a repo
- Change billing or organization settings

## How to Review and Approve Tool Connection requests

Fellows may ask you to connect a tool, like ChatGPT, Claude, or Cursor, to their team's repo. This guide explains what you can approve, what you can't, and how to set it up.

## What you can approve

### ✅ Approve

| Type of tool | Examples | Why it's low risk |
|---|---|---|
| AI assistants that only **read** code | ChatGPT's GitHub app, Claude's GitHub integration | They can't change anything in the repo |
| Review and quality tools | ReviewNB, pre-commit.ci | Free for public repos, limited to one repo |

### ⚠️ Approve with conditions

Check with your program manager before approving these, so teams in the same program get the same answer.

| Type of tool | Examples | Conditions |
|---|---|---|
| AI agents that **write code or open pull requests** | Codex, Claude Code, Cursor agents | Changes come in through pull requests only. The team reviews every change before merging. Fellows are responsible for any code they merge. |
| AI code reviewers | CodeRabbit, Sourcery | The team still does human reviews. |

### ⛔ Don't approve

Stop and send it to an org owner if any of these are true:

- The install screen doesn't offer **"Only select repositories"**
- It asks for organization permissions, member information, or repository administration
- It's an OAuth app, which can't be limited to one repo
- It needs a BTT payment method, BTT API key, or paid plan
- It asks for access to a private BTT repo

Most of these will be declined. Our firm rule: **tools are only connected to a team's own repo, never to the whole organization.**

## How to review a request

Ask the Fellow for the tool's name, which repo, what access it asks for, and why the team needs it. Then check:

1. **Can it be limited to this one repo?** If you're not sure, start the install and look for "Only select repositories."
2. **Does it read or write?** Read-only tools can be approved. Tools that write code or open pull requests need the conditions above.
3. **Does it cost BTT anything?** Fellows use their own accounts and free plans. If BTT would pay, don't approve it.
4. **What data will it see?** Repos are public, so code exposure is low risk. But if the team is using data the Challenge Advisor marked confidential, don't connect AI tools that could see it.

Also remind Fellows that many AI tools can use their conversations for model training, depending on their account settings. They should check their own settings.

## How to connect a tool

1. Go to the tool's GitHub App page and click **Install**. If it's already installed elsewhere in the organization, click **Configure**.
2. Choose the **Break Through Tech** organization.
3. Select **Only select repositories** and pick the team's repo. **Never choose "All repositories."**
4. Read the permissions screen before you confirm. If you see anything from "Don't approve," stop.
5. Record the approval (below).

To remove a tool, go to the repo's **Settings → GitHub Apps**, click **Configure** next to the tool, and remove the repo.

## Keep a record

Open an issue in the team's repo titled `Tool approved: [tool name]`. Include the date, who approved it, and any conditions. Close the issue when the tool is removed.

## When the program ends

Remove AI tools and agents from your teams' repos at the end of the program. Quality tools like ReviewNB can stay until the repo is archived.

## Red flags

Contact an org owner the same day if:

- A tool was connected to "All repositories" by mistake
- A Fellow authorized a tool for the whole organization
- A tool made changes nobody asked for, or pushed directly to `main`
- Something confidential was shared with an AI tool

The best way to reach an org owner is to email [it@breakthroughtech.org](it@breakthroughtech.org). Be sure to copy your PM or manager when you do, and allow at least one business day for a response. If something is truly urgent, ask a staff member to text or call Melissa Jones or Matt Brems right away. 


## Change log

- **v0.1 (Nov 2026):** First draft.
