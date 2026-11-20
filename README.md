# Awesome Agent Foundation (a13n)

A curated directory of App plugins, runnable examples, and tools for [Agent Foundation (a13n)](https://github.com/converge-ai-labs/agent-foundation).

Built a plugin, workflow, or project with a13n? [Suggest a resource](https://github.com/converge-ai-labs/awesome-a13n/issues/new?template=suggest-a-resource.yml) or [add it with a pull request](CONTRIBUTING.md).

[Documentation](https://a13n.converge.ai/docs/) · [Official examples](https://github.com/converge-ai-labs/agent-foundation/tree/main/examples)

## Contents

- [App Plugins](#app-plugins)
- [Examples & Recipes](#examples--recipes)
- [SDKs & Tools](#sdks--tools)
- [Contributing](#contributing)

## App Plugins

Installable application extensions for a13n Service. App plugins run with Service process permissions; review third-party packages before installing them.

**Build your own:** Start with the [App plugin authoring guide](https://github.com/converge-ai-labs/agent-foundation/blob/main/docs/a13n-service/app-plugins.md) and the [Cookiecutter template](https://github.com/converge-ai-labs/agent-foundation/tree/template/app-plugin) for full-stack, frontend-only, or backend-only projects.

- [a13n-channels](https://github.com/saurlax/a13n-channels) by [saurlax](https://github.com/saurlax) — Connect messaging platforms and event sources in Console, route incoming messages to agents, and let agents read permitted history and reply in the source channel. [Build and install](https://github.com/saurlax/a13n-channels#build-and-install) from source against its [pinned Service commit](https://github.com/saurlax/a13n-channels/blob/main/.service-ref). Upstream license not specified.

## Examples & Recipes

- [Agent application](https://github.com/converge-ai-labs/agent-foundation/tree/main/examples/agent-app) — Run an offline streaming chat with Harness and resume the same conversation after a restart.
- [MCP Apps counter](https://github.com/converge-ai-labs/agent-foundation/tree/main/examples/mcp-apps) — Open an interactive tool result in Harness UI and see how MCP interactions retain state between calls.
- [Reports App](https://github.com/converge-ai-labs/agent-foundation/tree/main/examples/service-app-plugin) — Build a Service App wheel with a reporting page, settings, and a workspace home view, using demo data.

## SDKs & Tools

Official clients for a13n Service:

- [Go SDK](https://github.com/converge-ai-labs/a13n-sdk-go)
- [Python SDK](https://github.com/converge-ai-labs/a13n-sdk-python)
- [Rust SDK and CLI](https://github.com/converge-ai-labs/a13n-sdk-rust) — Includes the remote `a13n-service-cli`.
- [TypeScript SDK](https://github.com/converge-ai-labs/a13n-sdk-typescript)

## Contributing

[Suggest a resource](https://github.com/converge-ai-labs/awesome-a13n/issues/new?template=suggest-a-resource.yml) or follow the [contribution guide](CONTRIBUTING.md). For a project or case study, tell us what you built, how you used a13n, and what someone can try or learn from it.

## License

This directory is licensed under the [MIT License](LICENSE). Linked projects and resources retain their own licenses.
