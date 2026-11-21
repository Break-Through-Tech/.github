# Coach Guide: Approving Tool Connections

**Internal. For Break Through Tech coaches.**

Fellows may ask you to connect a tool, like ChatGPT, Claude, or Cursor, to their team's repo. This guide explains what you can approve, what you can't, and how to set it up.

Nothing else about how you work with your teams is changing.

<!-- Draft v0.1. Items marked DECISION NEEDED need input from Melissa Jones and Hari Raghavan. -->

## Your access

You're a member of the **Coaches** team in our GitHub organization. The team has **Admin** access on every project repo, so you can install approved tools without waiting for an org owner.

You have access to every project repo so coaches can cover for and support one another. Work mainly in your own teams' repos. If you make a change in another coach's repo, let that coach know.

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

<!-- DECISION NEEDED: org owner contact or Slack channel for escalations -->

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

<!-- DECISION NEEDED: confirm the issue-based record, or name a shared tracker instead. -->

## When the program ends

Remove AI tools and agents from your teams' repos at the end of the program. Quality tools like ReviewNB can stay until the repo is archived.

<!-- DECISION NEEDED: confirm end-of-program removal timing. -->

## Red flags

Contact an org owner the same day if:

- A tool was connected to "All repositories" by mistake
- A Fellow authorized a tool for the whole organization
- A tool made changes nobody asked for, or pushed directly to `main`
- Something confidential was shared with an AI tool

No one gets in trouble for reporting quickly, including you.

<!--
FOR ORG OWNERS: one-time setup this guide depends on
- Coaches are org Members (not outside collaborators) on the Coaches team.
- When each project repo is created, add the Coaches team with Admin. Coaches who join later get access automatically.
- Member privileges > GitHub Apps: repo admins may install GitHub Apps (GitHub's default).
- Member privileges > App access requests: Members only.
- Member privileges: turn off members changing repo visibility and deleting/transferring repos.
- Keep this guide in a PRIVATE repo.
-->

## Change log

- **v0.1 (Nov 2026):** First draft.
