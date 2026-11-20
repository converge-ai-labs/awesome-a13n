# Contributing to Awesome Agent Foundation

Suggest a plugin, runnable example, tool, or project built with a13n. [Open a resource suggestion](https://github.com/converge-ai-labs/awesome-a13n/issues/new?template=suggest-a-resource.yml) or open a pull request that adds one entry to the README.

## What to include

- **Public link:** Use the canonical project, documentation, or write-up. Search the README and open submissions for duplicates.
- **What it does:** Describe the problem it solves and how it uses a13n in one or two sentences.
- **How to try it:** Point to installation instructions, a runnable example, a demo, or a write-up with a concrete outcome. A case study can link to an article or demo without publishing its source code.
- **For Service App plugins:** Link the setup instructions and state the Service version or commit used to build or test the plugin. Give the upstream license if one is published; otherwise say that the upstream project does not specify one. App plugins run with Service process permissions. Listed projects are not security-reviewed or endorsed by this directory.

## Entry format

Add one resource per pull request. Choose the closest section and place the entry in alphabetical order by name. If none fits, suggest a section in the PR or issue, especially for a project or case study built with a13n.

```markdown
- [Project name](https://example.com/project) — Explain what it does for an a13n user. [Setup](https://example.com/project/setup).
```

## Local checks

With [uv](https://docs.astral.sh/uv/) installed, synchronize the locked development environment and install the Git hooks:

```bash
uv sync --locked
uv run --locked pre-commit install
uv run --locked pre-commit run --all-files
```

uv manages Python 3.13 and the development dependencies for both local checks and CI.

The hooks format Markdown (including GitHub-flavored tables), validate YAML and JSON, and check whitespace, final newlines, merge conflicts, filename case conflicts, and files larger than 256 KiB. If a hook updates files, review and stage the changes before committing again.

The **Auto lint** workflow runs the same checks on pull requests and pushes to `main`. After verifying automatic fixes, it appends a `style(lint): apply automatic formatting fixes` commit to same-repository PR branches or the branch being checked on push/manual runs. It never amends commits or force-pushes. Fixes are checked again within the same run, since pushes made with `GITHUB_TOKEN` do not trigger another workflow run.

Fork PRs are check-only: formatting changes are shown in the log and must be applied by the contributor. Non-fixable errors fail CI and prevent automatic commits.
