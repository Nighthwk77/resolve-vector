# Privacy and Local Data

Resolve Vector is designed as a local-first, single-user application.

## Data stored locally

Project-specific state is stored under the selected project's `.vibe` directory. This can include configuration, run history, approvals, project memory, and protected provider credentials.

Application logs are stored under `~/Library/Logs/Resolve Vector`.

## Provider requests

When you configure a cloud AI provider, the context required for a request is sent to that provider. The provider's own terms, retention policy, and account settings apply.

Local model use can keep model requests on your Mac, depending on the server and configuration you choose.

## Credentials

Protected local credentials are stored in `.vibe/secrets.json` with owner-only file permissions. The file is excluded by the project-local `.vibe/.gitignore` created by Resolve Vector.

You remain responsible for keeping projects, backups, logs, and API credentials secure. Do not commit `.vibe/secrets.json`, publish diagnostic logs without reviewing them, or paste secrets into tasks.

## External advisors and web access

Advisor consultations and approved web requests may send selected content to third-party services. Resolve Vector asks for approval where required, but you should review the destination and submitted content.

## Removing local data

Deleting the application does not delete project data. Remove a project's `.vibe` directory only when you no longer need its configuration, history, memory, or locally stored credentials.
