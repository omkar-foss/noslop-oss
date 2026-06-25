# No-Slop OSS ![No-Slop OSS](https://img.shields.io/badge/no%20slop-oss-green)

> A checklist of no-slop contribution best practices when using AI (or not)
> in open source projects.

These days there's so many AI-generated repos and PRs without clear ownership,
what people call "AI slop". AI seems the main reason for the slop, but some
cases it's not the _only_ reason. There are cases where new contributors are
simply unaware of the best practices for contributing. This is quite some gap
that gets filled with contributors relying solely on AI tools, resulting in
slop. So awareness about open source best practices is very crucial, and even
more so now.

This checklist aims at preparing newcomers to start contributing to open source
projects in the best possible way, with or without using AI tools.

## Index

- [Checklist](#checklist)
  - [0. Contribute for the right reasons](#-0-contribute-for-the-right-reasons)
  - [1. Understand the project well](#-1-understand-the-project-well)
  - [2. Engage with the project community](#-2-engage-with-the-project-community)
  - [3. Set up your project environment thoroughly](#-3-set-up-your-project-environment-thoroughly)
  - [4. Understand the project's AI policies](#-4-understand-the-projects-ai-policies)
  - [5. Use AI as your tool, not as your replacement](#-5-use-ai-as-your-tool-not-as-your-replacement)
  - [6. Test and validate](#-6-test-and-validate)
  - [7. Choose the right issue](#-7-choose-the-right-issue)
  - [8. Starting to work on an issue](#-8-starting-to-work-on-an-issue)
  - [9. Communicate early and often](#-9-communicate-early-and-often)
  - [10. Submitting your contribution](#-10-submitting-your-contribution)
  - [11. Follow up](#-11-follow-up)
  - [12. What NOT to Do](#-12-what-not-to-do)
- [Note to project maintainers](#note-to-project-maintainers)
- [The 5 core open source principles](#the-5-core-open-source-principles)
  - [1. Transparency](#1-transparency)
  - [2. Community over code](#2-community-over-code)
  - [3. Process matters](#3-process-matters)
  - [4. Quality is a team effort](#4-quality-is-a-team-effort)
  - [5. Patience and persistence](#5-patience-and-persistence)
- [Contributing](#contributing)
- [Recommended articles & guides](#recommended-articles--guides)
- [Closing thoughts](#closing-thoughts)
- [LICENSE](#license)

## Checklist

> Follow these guidelines to become a high quality, no-slop OSS contributor.

### ☐ 0. Contribute for the right reasons

- Contribute to give back to the community, try not to chase vanity metrics
  like followers or stars.
- Compete with your own progress, not with others. Choose collaboration over
  competition.

### ☐ 1. Understand the project well

- Read the project's readme, contributing, and code of conduct
  files.
- Study the project's goals, architecture, and tech stack.
- Explore existing issues, discussions, and pull requests to grasp community
  priorities.
- Check for project-specific guidelines (e.g., design docs, roadmaps, or
  architecture decisions).

### ☐ 2. Engage with the project community

- Introduce yourself in the project's communication channels
  (Slack, Discord, mailing lists, etc).
  > **Example:** _Hi! I'm [Name], and I'd like to contribute to [Project]. I'm
  > particularly interested in [specific area]._
- Ask relevant questions in public forums, and not privately to avoid
  duplicating discussions.
- Read first, contribute later i.e. observe community discussions before
  jumping in.
- Follow the project's communication norms (e.g., response times, tone,
  meeting schedules).

### ☐ 3. Set up your project environment thoroughly

- Fork the repository and clone it locally.
- Set up the development environment exactly as documented in the project.
- Install dependencies and verify the project runs locally.
- Set up pre-commit hooks, linters, or formatters if recommended.

### ☐ 4. Understand the project's AI policies

- Check if the project has AI contribution policies (e.g. AI disclosure
  requirements).
  - If none exist, explicitly ask maintainers about their stance on AI tools.
- Disclose AI usage in your PR/issue without fail, irrespective of whether
  the project's AI policy demands it.

### ☐ 5. Use AI as your tool, not as your replacement

- Use AI to:
  - Brainstorm ideas or generate draft code snippets.
  - Automate repetitive tasks (e.g., formatting, testing scaffolding).
  - Document complex processes (e.g., setup instructions, troubleshooting).
- Never submit AI-generated code without:
  - Reviewing it line-by-line.
  - Testing it thoroughly.
  - Modifying it to fit the project's style.

### ☐ 6. Test and validate

- Run the project's test suite and ensure no errors.
- Write new tests for your changes.
- Manually verify your changes work as intended.
- If using AI-generated tests, review them carefully for edge cases.

### ☐ 7. Choose the right issue

- Start small with:
  - Bug fixes.
  - Documentation improvements.
  - Test additions.
  - Small feature implementations (labeled "good first issue").
- Avoid large or ambiguous changes until you're deeply familiar with the project.
- Check for "help wanted" or "needs review" labels in the issue tracker.

### ☐ 8. Starting to work on an issue

- Before raising a PR for an issue, check if there's one or more existing
  PRs for it. In case of existing PRs:
  - If any of those PRs are actively being updated, don't pick the issue as
    it could lead to duplicate effort. Find another issue to work on.
  - If all of those PRs are inactive, then probably you could pick up the issue.
- Comment on the issue and confirm with the maintainers before starting work
  to avoid duplication.

> **Example:** _"I'd like to work on this. May I pick this up? I plan to
> implement it like this: [your brief plan]."_

### ☐ 9. Communicate early and often

- Ask for feedback on your solution before submitting a PR.
- Document your thought process in the issue/PR.
- Be responsive to feedback and iterate.

### ☐ 10. Submitting your contribution

- If the project has a pull request template, follow it thoroughly.
- Create a new branch for your changes (e.g., `fix/issue-123`).
- Write clear, descriptive commit messages.
  - Follow the project's conventions (e.g., `Fix #123: [description]`).
  - If AI tools are used, disclose AI use in your commit description either with
    `Assisted-by` or `Co-authored-by`.
  - Provide DCO sign-off in your commits using `Signed-off-by`.

> **Example DCO sign-off along with AI disclosure in commit:**

```git
Improve error handling in user authentication module

- Added custom error classes for authentication failures
- Implemented retry logic for transient failures
- Updated tests to cover new error scenarios

Assisted-by: GitHub Copilot (for new error scenario tests)
Signed-off-by: Your Name <youremail@address.here>
```

- Include references to relevant issues in your PR description.
- In the PR description:
  - Disclose AI usage (e.g., "This PR includes AI-assisted code generation for
    [specific part]").
  - Explain your process and reasoning.
  - Link to any related discussions or issues.

### ☐ 11. Follow up

- Monitor your PR for feedback and be ready to make changes.
- Thank reviewers for their time and feedback.
- If your PR is closed, ask for feedback on how to improve, so you can learn
  from your mistakes.
- Celebrate your contribution, appreciate any help you received from other
  community members; open source is a community effort!

### ☐ 12. What NOT to do

- Do not submit AI-generated code without reviewing, understanding, and testing
  it.
- Do not ignore community guidelines or communication norms.
- Do not submit large changes without prior discussion and approval.
- Do not spam the issue tracker or PR queue with low-quality contributions.
- Do not assume AI tools can replace human collaboration; engage with the
  community.

## Note to project maintainers

You can use this checklist in your project as NOSLOP.md or in your
CONTRIBUTING.md file. Or you could also share it with others to spread
awareness.

## The 5 core open source principles

These are the core principles upon which this checklist is based.

### 1. Transparency

> **The more transparent the process, the easier it is for others to
> contribute.**

Document your process, share reasoning and disclose AI usage.

### 2. Community over code

> **A healthy project is built on relationships, not just code.**

Work together with other community members to enhance collaboration and ensure
project and community well-being. Community health is primary, code is
secondary.

### 3. Process matters

> **Good processes make it easy to do the right thing.**

Follow the project's contribution guidelines, even when using AI tools.

### 4. Quality is a team effort

> **No one person or tool can ensure quality, it's a community responsibility.**

Strive to work towards quality rather than quantity. Treat AI-generated code as
a draft, not a final submission.

### 5. Patience and persistence

> **Open source is a marathon, not a sprint.**

Iterate, learn from feedback, and keep improving.

## Contributing

Feel free to raise a PR in case you'd like to add something. Refer to the
[checklist above](#checklist) for contribution guidelines. All contributions
should abide by [this code of conduct](CODE_OF_CONDUCT.md).

## Recommended articles & guides

- [**GitHub's Open Source Guide**](https://opensource.guide/)
- [**How to Responsibly and Effectively Contribute to Open Source Using AI**](https://www.honeycomb.io/blog/responsibly-effectively-contribute-open-source-using-ai)
- [**Maintaining open source in the age of generative AI: Recommendations for maintainers and contributors**](https://blog.probabl.ai/maintaining-open-source-age-of-gen-ai)
- [**The Open Source Way**](https://www.theopensourceway.org/)

## Closing thoughts

Remember, open source is about people, and not just about churning out code. The
goal is to build trust, foster community, and create maintainable software
together.

## License

[![CC0 Public domain. This work is free of known copyright restrictions.](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](LICENSE)
