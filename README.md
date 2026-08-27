# No-Slop OSS ![No-Slop OSS](https://img.shields.io/badge/no%20slop-oss-green)

> A checklist of no-slop contribution best practices when using AI (or not)
> in open source projects.

These days there are so many AI-generated repos and PRs without clear ownership,
often referred to as "AI slop". AI use is a reason for the slop, but some cases
it's not the only reason. Many new, genuine (human) contributors are simply
unfamiliar with open source workflows and project expectations, and AI tools can
sometimes amplify those gaps. It results in their contributions getting lost
among the noise and getting ignored by maintainers.

This checklist focuses on best practices that help contributors build trust and
submit high-quality contributions, whether they use AI or not. It's a checklist
for becoming the kind of contributor maintainers enjoy reviewing!

## Index

- [Checklist](#checklist)
  - [0. Contribute with purpose](#-0-contribute-with-purpose)
  - [1. Understand the project well](#-1-understand-the-project-well)
  - [2. Engage with the project community](#-2-engage-with-the-project-community)
  - [3. Set up your project environment thoroughly](#-3-set-up-your-project-environment-thoroughly)
  - [4. Understand the project's AI policies](#-4-understand-the-projects-ai-policies)
  - [5. Use AI as your tool, not as your replacement](#-5-use-ai-as-your-tool-not-as-your-replacement)
  - [6. Test, validate and document](#-6-test-validate-and-document)
  - [7. Choose the right issue](#-7-choose-the-right-issue)
  - [8. Starting to work on an issue](#-8-starting-to-work-on-an-issue)
  - [9. Communicate early and often](#-9-communicate-early-and-often)
  - [10. Submitting your contribution](#-10-submitting-your-contribution)
  - [11. Follow up](#-11-follow-up)
  - [12. What NOT to Do](#-12-what-not-to-do)
- [Note to project maintainers](#note-to-project-maintainers)
- [Contributing](#contributing)
- [Recommended articles & guides](#recommended-articles--guides)
- [Closing thoughts](#closing-thoughts)
- [LICENSE](#license)
- [AI policy](#ai-policy)

## Checklist

> Follow these guidelines to become a high quality, no-slop OSS contributor! 🌟

### ☐ 0. Contribute with purpose

- Contribute with the goal of creating value for the project, whether you're
  learning, solving a problem, or giving back to the community.
- Focus on making meaningful contributions rather than optimizing for visibility
  or metrics.
- Compete with your own progress, not with others. Choose collaboration over
  competition.

### ☐ 1. Understand the project well

- Read the project's readme, contributing, and code of conduct files.
- Study the project's goals, architecture, and tech stack.
- Explore existing issues, discussions, and pull requests to grasp community
  priorities.
- Read recent pull requests to understand the project's coding style, review
  expectations, and current development priorities.
- Check for project-specific guidelines (e.g., design docs, roadmaps, or
  architecture decisions).

### ☐ 2. Engage with the project community

- If appropriate for the project's community, introduce yourself in its public
  communication channels (Slack, Discord, mailing lists, etc).
  > **Example:** _Hi! I'm [Name], and I'd like to contribute to [Project]. I'm
  > particularly interested in [specific area]._
- Ask relevant questions in public forums, and not privately to avoid
  duplicating discussions.
  - Before asking a question, spend a few minutes searching existing issues,
    discussions, and documentation.
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
- If the project doesn't mention AI usage, avoid assuming it's acceptable.
  Consider asking maintainers if disclosure or other expectations aren't clear.
- Preferably disclose AI usage in your PR/issue irrespective of whether the
  project's AI policy demands it.

### ☐ 5. Use AI as your tool, not as your replacement

- Use AI to:
  - Brainstorm ideas or generate draft code snippets.
  - Automate repetitive tasks (e.g., formatting, testing scaffolding).
  - Document complex processes (e.g., setup instructions, troubleshooting).
- Never submit AI-generated code without:
  - Reviewing it line-by-line.
  - Testing it thoroughly.
  - Modifying it to fit the project's style.
- Make sure you can explain every change you submit, whether it was written by
  you or assisted by AI.

### ☐ 6. Test, validate and document

- Run the project's test suite and ensure no errors.
- Write new tests for your changes.
- Manually verify your changes work as intended.
- If using AI-generated tests, review them carefully for edge cases.
- Update documentation, examples, or changelog entries if your changes
  affect users.

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
  - If all those PRs are inactive, then you could pick up the issue after
    confirming with maintainers.
- Comment on the issue and confirm with the maintainers before starting work
  to avoid duplication.

> **Example:** _"I'd like to work on this. May I pick this up? I plan to
> implement it like this: [your brief plan]."_

### ☐ 9. Communicate early and often

- For larger changes, ask for feedback on your proposed approach before
  opening a PR.
- Be prepared for your proposed solution to be declined. Not every good idea
  aligns with a project's roadmap.
- Document your thought process in the issue/PR.
- Be responsive to feedback and iterate.

### ☐ 10. Submitting your contribution

- If the project has a pull request template, follow it thoroughly.
- Keep your pull request focused on a single logical change whenever possible.
- Create a new branch for your changes (e.g., `fix/issue-123`).
- Write clear, descriptive commit messages.
  - Follow the project's conventions (e.g., `Fix #123: [description]`).
  - If you used AI tools and if project encourages commit-level AI disclosure,
    use the project's preferred format (e.g. `Assisted-by` or `Co-authored-by`).
  - If project recommends DCO sign-off, provide one in your commits using
    `Signed-off-by`.

> **Example DCO sign-off along with AI disclosure with Assisted-By in commit:**

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
- Give the reviewers time to respond, avoid repeatedly asking for updates (e.g.
  every few hours).
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
- Do not rely on AI in place of understanding the codebase or engaging with
  the community.

## Note to project maintainers

Projects are welcome to adopt this checklist as [`NOSLOP.md`](NOSLOP.md),
incorporate parts of it into `CONTRIBUTING.md`, or simply share this repository
with contributors.

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

Open source succeeds through people as much as code. Building trust,
communicating clearly, and collaborating well are just as important as
writing software.

## License

[![CC0 Public domain. This work is free of known copyright restrictions.](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](LICENSE)

## AI policy

This project follows a strict no-AI policy and does not accept contributions with AI/LLM use in any form.

