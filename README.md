# Agent skills

AI agent skills to contribute to and maintain the [scaleway-terraform-modules](https://github.com/scaleway-terraform-modules) repositories.

> [!NOTE]
> Work in progress: the plugins are declared, the skills are being written.

## Workflow

The skills follow the same process as any other contribution, with or without AI:

| Step | Skill | Plugin | Result |
|---|---|---|---|
| 1. Discovery | `discover` | `contributing` | Candidate changes for a repository: fixes, features, refactoring, documentation |
| 2. Refinement | `refine` | `contributing` | A GitHub issue both the operator and the agent understand the same way, marked as refined |
| 3. Completion | `implement` | `contributing` | A pull request for a refined issue, or updates addressing review comments |
| 4. Review | `review` | `maintaining` | A pending review on a pull request, from a contributor or from step 3 |

Principles:

- **The operator stays in control.** The skills run locally and ask before anything visible on GitHub: pushing, opening a pull request or an issue, commenting, labelling, reviewing.
- **Same templates for everyone.** The skills use the issue and pull request templates of the repositories and of the organization's [`.github` repository](https://github.com/scaleway-terraform-modules/.github). They never keep their own copy.
- **One issue, one repository.** A change needed in several repositories gets one issue per repository.

## Installation

### Claude Code

```text
/plugin marketplace add scaleway-terraform-modules/agent-skills
/plugin install contributing@scaleway-terraform-modules
/plugin install maintaining@scaleway-terraform-modules
```

Maintainers install both plugins; contributors usually only need `contributing`.

### Other agents

The skills use the `SKILL.md` format, which other agents can read too. They live in `plugins/<plugin>/skills/<skill>/SKILL.md`.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md), and [AGENTS.md](AGENTS.md) for the conventions of this repository.

## License

[MPL-2.0](LICENSE)
