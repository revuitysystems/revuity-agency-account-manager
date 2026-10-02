# Changelog

## Unreleased

- Added `SUBMISSION_READINESS.md` recording validation, runtime load, and invocation results. No change to plugin behavior.
- Added a privacy policy link to the manifest and README.
- Added `displayName` to the manifest and `SUBMISSION.md` for the directory submission. Switched the README icon to Markdown image syntax. No change to plugin behavior.
- Added the plugin icon files, an icon field in the manifest for the Anthropic directory listing, and a README icon section. No change to plugin behavior.

## 1.0.0 — Initial public release

- Initial public release of Agency Account Manager as a standalone plugin repository.
- Added the `agency-account-manager` plugin with the `account-operations` skill covering meeting prep and recaps, deliverable tracking, scope protection, client health and risk review, and renewal preparation.
- Includes source-discipline rules that keep proposed and approved scope and commercial changes distinct.
- Includes explicit authorization boundaries for external sends, scope and SOW changes, pricing and credits, contract amendments, and acceptance of client legal or security terms.
- Added a GitHub Actions workflow that validates the manifest, semantic version, skill frontmatter, and required documentation.

### Verification

Package validation runs in GitHub Actions. This release has not been installed or exercised in a user's Claude runtime by its authors; smoke-test the plugin in your own Claude environment after installing it.
