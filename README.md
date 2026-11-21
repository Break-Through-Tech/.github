# .github
Welcome and README

# Welcome to Break Through Tech on GitHub

Welcome! This page explains how the Break Through Tech GitHub organization is set up, who can do what, and where to go for help. Please read it once when you join. It takes about five minutes. Ready to start contributing? Read our [Contributing Guide first](https://github.com/Break-Through-Tech/.github/blob/main/contributing.md).

## Why we use GitHub

Break Through Tech programs, starting with AI Studio, use GitHub so that:

- **Fellows work the way real engineering teams work:** branches, pull requests, issues, and project boards.
- **Fellows leave the program with a public portfolio** they can show employers and grad schools.
- **Coaches, Challenge Advisors, and staff can see progress** and help in one place.

## Who's who

There are four kinds of people in our organization. Your role decides what you can do.

| Role | Who | What you can do | Why it's set up this way |
|---|---|---|---|
| **Owner** | A small group of BTT staff: Melissa Jones, Matt Brems, Hari R. | Everything: settings, billing, adding people, creating repos | We keep this group small on purpose |
| **Member** | BTT staff, contractors, PMs, and Coaches (all with BTT email addresses) | Work in the repos you're given. Coaches can set up project boards and manage their own teams' repos | Coaches need to be members to create GitHub Projects boards for their teams |
| **Outside collaborator: Challenge Advisor** | Volunteer advisors from partner companies | Review and contribute to the specific repo(s) you're added to | Keeps settings and repo creation in BTT's hands |
| **Outside collaborator: Fellow** | Program participants | Write code, open pull requests, create issues and branches in your team's repo | Same as above |

**In short:** Fellows and Challenge Advisors are added to specific repositories, not to the whole organization.

## Public vs. private repositories

- **Project repositories are public.** Anyone on the internet can view them, even without a GitHub account. This allows your work to become a shareable portfolio.
- **Internal tools and templates are stored elsewhere.** Only the staff who need them can see them; they are stored in our BTT GitHub Codebase organization. Email it@breakthroughtech.org for more information.  

Because project repos are public, **never put these in any repo:**

- Passwords, API keys, or access tokens
- Personal information about anyone (names with contact info, student records, etc.)
- Any data a Challenge Advisor has marked as confidential

Admins will periodically scan repos for secrets and remove them if discovered.

> [!IMPORTANT]
> If you accidentally commit something sensitive, tell your Coach right away. Deleting the file is not enough, because it stays in the history. We'll help you clean it up. No one gets in trouble for reporting it quickly.

## How project repos are organized

Every project repo starts from the same template and includes:

- **Challenge Project Overview:** what the project is and what data you'll use (filled in by BTT and the Challenge Advisor)
- **Getting Started for Fellows:** where to learn about the project, find the data, and document your work
- **Project documentation template (`README.md`):** filled in by Fellows at the end. This becomes your portfolio write-up
- **A GitHub Projects board:** where your team tracks tasks, set up by your Coach

Repos are named `Company-TeamCode-project-name` (for example, `Accenture-1N-contract-review-challenge`).

<!-- DECISION NEEDED: add a program term tag such as F26, or a topic like ai-studio-fall-2026 -->

## Safety rules built into every project repo

These are turned on automatically. You don't need to do anything, but it helps to know they're there:

| Rule | What it means for you |
|---|---|
| **No deleting** | Only Coaches and BTT staff can delete branches or content |
| **No force pushes** | You can't overwrite shared history. This protects your teammates' work |
| **Pull request required to merge** | Changes go into the main branch through a pull request. Approval is not currently required, but asking a teammate or your Coach to review is strongly encouraged |

## What happens when the program ends

<!-- DECISION NEEDED: final retention policy. Text below is the proposal. -->

- Fellows keep access to their repo after the program for 12 months.
- Fellows have **12 months** after the program ends to fork (copy) the repo to their personal GitHub account. Your fork is yours to keep.
- After 12 months, BTT archives the repo. <!-- DECISION NEEDED: archive (read-only, still public) or make private -->
- We'll send a reminder before anything changes.

## Getting help

| If you need... | Go to... |
|---|---|
| Help with your project, Git, or your repo | Your Coach |
| Access to a repo, or to be added/removed | Your Coach |
| A new tool or app added to your repo | See "Requesting a tool" in the [Contributing guide](https://github.com/Break-Through-Tech/.github/blob/main/contributing.md), then ask your Coach |
| Something that looks like a security problem | Your Coach, who should escalate to [it@breakthroughtech.org](mailto:it@breakthroughtech.org) the same day |

## Who owns these rules

- **Organization governance (settings, README, contribution guidelines, connection request approvals):** BTT IT
- **Program requirements (whether a Program uses this GitHub org or not, and how)**: BTT Product team (Hari, Dom, Hi’ilei, Melissa F.)
- **Program run setup (templates, repos, Coach onboarding):** IT team, with Lead  PM
- **During Program run maintenance**: PMs and Coaches. Fellows help by keeping the Org clean and secure
- **After Program run clean up**: BTT IT, with Lead PMs

### Suggesting a change to these rules

We want this to work for the people using it. If a rule is getting in your way or something is missing:

1. Tell your Coach, who can escalate to [it@breakthroughtech.org](it@breakthroughtech.org), or open an issue in the `.github` repository with the label `governance`.
2. BTT IT reviews suggestions within two weeks.
3. Changes are noted at the bottom of this page.

## Related guides

- **[Contributing guide](https://github.com/Break-Through-Tech/.github/blob/main/contributing.md)** (Fellows and Challenge Advisors): how to work in a repo, etiquette, and requesting tools
- **Coach guide**: What Coaches can and can't do with their admin access

## Change log

- **v0.1 (Nov 2026):** First draft, based on the Sept 14 governance meeting (Melissa, Hari, Christine).
