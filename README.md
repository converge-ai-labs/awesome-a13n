# Awesome Agent Foundation (a13n)

A curated collection of projects, practical use cases, integrations, and guides for [Agent Foundation (a13n)](https://github.com/converge-ai-labs/agent-foundation).

Discover what people build with a13n, how it works, and what you can reuse. This repository is an index: code and detailed documentation stay in their source repositories.

## Start here

- [Agent Foundation](https://github.com/converge-ai-labs/agent-foundation) — The open-source library and self-hosted platform for building and running your own agent systems.
- [Documentation](https://a13n.converge.ai/docs/) — Guides for Harness, Service, and Harness UI.
- [Official examples](https://github.com/converge-ai-labs/agent-foundation/tree/main/examples) — Runnable examples from the main repository.

## Contribute

This collection is just getting started. Have a project, use case, integration, or guide to share? Open an issue or pull request with a link, a short description of the problem it solves, and any available code or demo.

### Local checks

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

## License

This repository is licensed under the [MIT License](LICENSE). Linked projects and resources retain their own licenses.
