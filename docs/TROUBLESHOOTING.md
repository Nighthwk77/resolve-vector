# Troubleshooting

## The application will not open

If the build is not notarized yet, follow the first-launch instructions in [Installation](INSTALLATION.md). Confirm that the file came from the official Releases page and verify its checksum first.

## The selected port is already in use

Open **Resolve Vector → Runtime Port** and choose another available port. If Resolve Vector detects its own backend serving a different project, it asks before stopping and switching that backend.

## A provider is unavailable

Open **AI → Provider Health** and run the available checks. Confirm the provider URL, model name, credential source, account access, and local-server status.

## Work appears stuck

Check the visible progress state in the workspace, then open **View → Technical Activity** for lower-level events. Also check whether an approval or clarification is waiting for you.

## A project opens with the wrong context

Confirm the selected project and session. Start a new session when changing goals. Project memory can be reviewed under **View → Project Memory**.

## Find logs and diagnostics

Open **Help → Diagnostics and Logs**. Runtime logs are also stored under `~/Library/Logs/Resolve Vector`.

Before posting logs publicly, inspect them for project names, file paths, prompts, source excerpts, URLs, and credentials.

## Still need help?

Read [Support](../SUPPORT.md) and submit a structured bug report with sensitive information removed.
