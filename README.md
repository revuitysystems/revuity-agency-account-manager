# Agency Account Manager

**A free Claude workflow plugin by [Revuity Systems](https://revuitysystems.com).**

A free Claude plugin for keeping client-service work moving across meetings, commitments, deliverables, approvals, scope, risks, follow-up, and renewals. It is built for agencies, consultancies, studios, and other client-service teams that want a clearer operating rhythm around client accounts.

- Plugin name: `agency-account-manager`
- Skill: `/agency-account-manager:account-operations`
- Version: 1.0.0
- License: MIT

## Good for

- Meeting preparation
- Meeting recaps
- Commitment tracking
- Deliverable status review
- Client approvals
- Scope-change detection
- Client risk review
- Follow-up planning
- Renewal preparation
- Account operating reviews

## How it works

The plugin treats every account as a set of promises, deliverables, decisions, risks, approvals, and outcomes. It separates client actions from internal actions, always preserves the difference between proposed and approved, and does not treat a suggestion, draft, meeting comment, or informal message as an approved scope or commercial change. Account health reviews rest on evidence such as missed commitments, approval delays, and unresolved issues, with observed facts kept apart from interpretation.

## Example requests

Once the plugin is loaded, ask in plain language or invoke the skill directly with `/agency-account-manager:account-operations`.

- "Prepare me for tomorrow's client meeting: open commitments, pending approvals, risks, scope questions, and a recommended agenda."
- "Turn these meeting notes into a recap that separates confirmed decisions, client actions, internal actions, and possible scope changes."
- "Flag anything in this request thread that may fall outside our signed scope and draft a neutral change brief."
- "Prepare the renewal conversation plan for this account using the outcomes we can evidence."

You supply the information, either by pasting it in or through tools you have already connected to Claude. The plugin does not collect data of its own, does not call any Revuity service, and has no executable code.

## Authority and safety boundaries

The plugin organizes, analyzes, drafts, and recommends. It does not alter terms automatically and does not invent ROI or outcome claims. Explicit human authorization is required for consequential external sends, scope or SOW changes, discounts, credits, pricing, or payment terms, contract amendments, invoice changes, promises of unapproved dates or resources, and acceptance of client legal or security terms.

When something is missing, stale, or in conflict, the plugin is written to stop and say so rather than guess.

## Data handling

Share only the account information a task needs. Avoid pasting passwords or confidential client material that the task does not require. Your contract confidentiality and privacy obligations still apply to anything you share with Claude.

## Install

This repository is a single Claude plugin with its manifest at `.claude-plugin/plugin.json` and its skill at `skills/account-operations/SKILL.md`.

To try it locally, clone the repository and start Claude Code with the plugin directory:

```bash
git clone https://github.com/revuitysystems/revuity-agency-account-manager.git
claude --plugin-dir ./revuity-agency-account-manager
```

Then run `/reload-plugins` and confirm `/agency-account-manager:account-operations` appears. To check the package without running it, use `claude plugin validate ./revuity-agency-account-manager`.

## Validation

A GitHub Actions workflow in this repository checks the manifest, semantic version, skill frontmatter, and required documentation on every push and pull request. See `.github/workflows/validate.yml`. Passing validation shows the package is well formed. It does not replace testing the plugin in your own Claude environment against your own policies.

## Built by Revuity Systems

Revuity Systems is an Operations Systems company. These public workflow plugins are free operating tools designed to make real work easier while demonstrating how Revuity thinks about roles, workflows, responsibility, authority, exceptions, outcomes, and operating cadence.

When an organization later needs the workflow adapted to its own systems, policies, data, approvals, integrations, or operating model, Revuity may help design or build that larger system. You do not need to talk to anyone to use this plugin.

More at [revuitysystems.com](https://revuitysystems.com). Questions or security concerns: info@revuitysystems.com.

## License

MIT. See [LICENSE](LICENSE).
