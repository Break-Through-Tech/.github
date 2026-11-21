# Contributing Guide for Fellows and Challenge Advisors

Welcome to your project repo! This guide covers how to work here, how to be a good teammate, and what to do when you need something. For the big picture, see our Governance page.

<!-- Draft v0.1. Items marked DECISION NEEDED are still being decided. -->
<!-- TODO: link "Governance page" above once the org profile README is live. -->

## Your access, in plain terms

- You've been added to your team's repo with **Write** access. You can create branches, push code, open pull requests, and create issues.
- You can **view** every other public Break Through Tech repo, but you can only make changes in yours.
- You **can't** create new repos, change settings, or delete things.
- **Want to connect a tool like ChatGPT, Claude, or Cursor to your repo?** Talk to your coach. See [Requesting a tool or app](#requesting-a-tool-or-app).

## How to work in your repo

1. **Start with the Getting Started page in your repo.** It explains the project, the data, and where to document your work.
2. **Track your tasks on your team's Projects board.** Create an issue for each task and link it to the board.
3. **Work on a branch, not directly on `main`.** Name it something clear, like `data-cleaning` or `jane-baseline-model`.
4. **Open a pull request when you're ready to add your work to `main`.** Write a short description: what you changed and why.
5. **Ask for a review.** Request a teammate to review (or your coach for bigger changes). You're technically able to merge your own pull request, but getting a second set of eyes is how professional teams work, and it's a great habit to show employers.
6. **Document as you go.** At the end, your team fills in the project write-up. This is your portfolio piece.

## Repo security and visibility

Anyone on the internet can see your repo. That's what makes it a great portfolio. It also means:

- **Never commit passwords, API keys, tokens, or `.env` files.** Use a `.gitignore`.
- **Never commit personal information about anyone.**
- **Only use data your Challenge Advisor has cleared for the project.**

> [!IMPORTANT]
> **Made a mistake?** Tell your coach right away. Deleting the file isn't enough since it stays in the history, and we'll help you fix it. Reporting quickly is always the right call.

## Etiquette

- **Be kind in reviews.** Comment on the code, not the person. "Could we rename this variable so it's clearer?" is better than "This is confusing."
- **Don't rewrite a teammate's work** without talking to them first.
- **Keep discussion in the repo** (issues and pull request comments) so the whole team and your coach can follow along.
- **Respond to review requests** within a day or two when you can.
- **Credit honestly.** On your résumé or LinkedIn, describe what you did on the project.

## Requesting a tool or app

Some tools, like ChatGPT, Claude, Cursor, or other AI assistants, can connect to GitHub. We're happy to consider these for legitimate project needs, with one firm rule:

> **Tools would only ever be connected to your team's repo. Never to the whole Break Through Tech organization.**

Connecting a tool to the organization could give it access to other teams' work and to BTT's private repos.

### How to request

**Talk to your coach.** Your coach can review your request and connect approved tools to your team's repo. Come ready to share:

- The tool's name
- Which repo you want it connected to
- What access it asks for (for example, read-only or permission to open pull requests)
- Why your team needs it

You'll hear back from your coach. <!-- DECISION NEEDED: response time, e.g., within 5 business days -->

> [!WARNING]
> **Please don't** use GitHub's "Request" button, click "Authorize for Break Through Tech," or choose "All repositories" when connecting a tool. These skip the review, and organization access can't be approved. If a tool asks for any of these, stop and talk to your coach.

### What to expect

- **AI assistants that only read your code** (for example, to explain it or answer questions about it) are usually approved for your team's repo.
- **AI tools that write code or open pull requests for you** may be approved, as long as your team reviews every change before merging. You're responsible for any code you merge, whoever or whatever wrote it.
- **Tools that need access to the whole organization** won't be approved.

Many AI tools let your account's conversations be used to train their models. Check the privacy settings on your own account, and never share data your Challenge Advisor has marked confidential.

<!--
ON HOLD: GitHub built-in features. Uncomment this section once the org billing issue is resolved
and the GitHub-recommended security configuration is applied to public project repos.

### Already built into your repo

These GitHub features are free for public repos. You don't need to request them:

- **Secret scanning and push protection:** blocks a push if it contains a password, API key, or token. If it stops you, that's working as intended. Remove the secret and ask your coach if you're stuck.
- **Code scanning (CodeQL):** flags possible security bugs in your pull requests.
- **Dependabot:** alerts you when a library you use has a known vulnerability, and may open a pull request to update it.
- **GitHub Actions:** runs automatic checks, like formatting and linting, on your pull requests. Ask your coach if you'd like help setting one up.
-->

### Other tools that are usually approved

These are free for public repos and only need access to your team's repo. Ask your coach the same way:

| Tool | What it does | Good for |
|---|---|---|
| **ReviewNB** | Readable diffs and comments for Jupyter notebooks | Teams working mainly in notebooks |
| **pre-commit.ci** | Runs formatting and lint checks on pull requests, and can fix them automatically | Keeping code clean and consistent |

<!-- TODO: confirm current free terms for pre-commit.ci before publishing. -->

<!--
ON HOLD: Codecov needs GitHub Actions to upload coverage. Add this row back to the end of the table above
once the org billing issue is resolved (and confirm Codecov's current free terms):
| **Codecov** | Shows how much of your code is covered by tests | Teams writing tests |
-->

### Tools we review case by case

**AI code reviewers** (such as CodeRabbit or Sourcery) post automated review comments on pull requests. They can be helpful, but they read all of your repo's code, and they don't replace a review from a teammate or your coach. If your team wants one, tell your coach how you'll still do human reviews.

### Tools you don't need to request

AI coding assistants that run in your own editor, like GitHub Copilot, don't connect to Break Through Tech's GitHub. As a student, you may be able to get them free through GitHub's student benefits. Follow your program's rules on AI use and never paste confidential project data into them.

<!-- DECISION NEEDED: confirm this matches AI Studio's AI use rules. -->

<!--
ADMIN CHECKLIST (move to the internal Coach and program manager guide):
- Install apps with "Only select repositories". Never "All repositories".
- Check the permissions screen: repo-level access only. Decline apps asking for org-wide or members access, and OAuth apps that can't be limited to one repo.
- Free terms apply to PUBLIC repos. Don't install on private internal repos without checking pricing.
- Pilot AI reviewers on one repo first, and check the vendor's data retention terms.
-->

## Working on other projects

There are two different situations here:

### 1. "I want to help another team with their project."

<!-- DECISION NEEDED: confirm this rule -->

- Check with your coach and their coach first.
- Open a pull request to their repo. Don't push directly.
- Their team reviews and approves before anything is merged. You never merge into another team's repo yourself.
- Keep your own team's work as your first priority.

### 2. "I saw another project and want to try it myself."

- All project repos are public, so you can fork one to your personal GitHub and work on it on your own.
- This is independent practice, not program work.
- On your résumé, describe it as a personal project based on a Break Through Tech challenge. Don't describe it as work done for the partner company.

## After the program

<!-- DECISION NEEDED: final retention policy. Text below is the proposal. -->

- You keep access to your team's repo after the program.
- You have **12 months** to fork the repo to your personal GitHub account. Your fork is yours to keep, and it's a good idea to do this early.
- After 12 months, Break Through Tech will archive the original repo. We'll send a reminder first.

## Questions?

Ask your coach first. For anything they can't answer, they'll connect you with the right person.

## Change log

- **v0.2 (Nov 2026):** Tool requests now go through your coach. Added guidance on AI tools and approved tools.
- **v0.1 (Sept 2026):** First draft, based on the Sept 14 governance meeting.
