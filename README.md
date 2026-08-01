# .github

Default community health files for [@rishifter](https://github.com/rishifter)'s repositories.

GitHub falls back to the files in this repository whenever one of my other repositories
does not ship its own copy. Anything added here applies everywhere by default; committing
the same file to an individual repository overrides it for that repository only.

## What's here

| File | Applies to | Purpose |
| --- | --- | --- |
| [`pull_request_template.md`](pull_request_template.md) | Every new pull request | Prefills the PR description with a summary, issue links, type of change, testing steps and deployment notes. |

## Adding more defaults

GitHub recognises these filenames in the root of this repository (or in a `.github/`
or `docs/` folder inside it). None of them exist yet:

- `CONTRIBUTING.md` — how to set up, branch, and open a PR
- `SECURITY.md` — how to report a vulnerability, and where
- `SUPPORT.md` — where to ask questions
- `CODE_OF_CONDUCT.md` — expected conduct and the enforcement contact
- `GOVERNANCE.md` — who decides what
- `FUNDING.yml` — the sponsor button
- `ISSUE_TEMPLATE/` — issue forms, plus `config.yml` to add links or disable blank issues

## What is *not* inherited

These are per-repository and have to be committed to each repo that needs them:

- `.github/workflows/*` — though this repo can host **reusable** workflows, called with
  `uses: rishifter/.github/.github/workflows/<file>.yml@main`
- `.github/dependabot.yml`
- `CODEOWNERS`
- Labels, branch protection rules, and rulesets

## Notes

- This repository is public, so everything in it is visible to anyone.
- The profile README shown on my GitHub profile is **not** here — it lives in the
  `rishifter/rishifter` repository, which has to be public for GitHub to render it.
  A `profile/README.md` inside a `.github` repository only works for organisations,
  not personal accounts.
