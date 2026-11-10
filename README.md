# Harness Agent Builder

Publisher: **Healthzone MD** | Ecosystem: **Codex** | Package version: **1.0.1**

## What it does

A text-only skill for planning reliable AI-agent workflows: task contracts,
context selection, tool boundaries, durable state, verification, and recovery.
It is not a standalone agent executable, MCP server, or preconfigured runtime.

## Availability and package identity

This documentation describes an **unsigned release candidate**, not a published
or approved marketplace download. No download is offered on this page yet.

Expected filename: `harness-agent-builder-1.0.1.zip`

SHA-256:

```text
d81abac46f7bcae8892de0c976abaee40f7f795d080d10ec37571e63eda6dbad
```

The ZIP contains:

- `README.md`: package-specific setup and limitations.
- `LICENSE.txt`: Healthzone MD Personal-Use License v1.0.
- `manifest.json`: package identity and file hashes.
- `harness-agent-builder/SKILL.md`: skill instructions.
- `harness-agent-builder/agents/openai.yaml`: host UI and invocation metadata.
- `harness-agent-builder/references/blueprint.md`: supporting workflow reference.

## Manual Codex setup

1. Obtain the exact approved package when it becomes available. Compare its hash
   against the approved product page; a matching hash identifies bytes, not safety.
2. Inspect the README, license, manifest, and all skill files. Extract into a new
   folder, without running installers or replacing existing files.
3. Copy the complete `harness-agent-builder` folder into your project's
   `.agents/skills/` directory. Current Codex documentation describes this location;
   the packaged README also mentions the source workspace's `.codex/skills`
   configuration. Confirm the supported location for your installed client.
4. Check the skill inventory. Restart Codex if the new skill does not appear.
5. Try a synthetic, read-only task using `$harness-agent-builder`, such as:
   "Plan a read-only review of a small example repository. Give me the task
   contract and verification checklist before taking any action."

See [official Codex skill documentation](https://learn.chatgpt.com/docs/build-skills)
for supported skill locations and per-skill controls. Do not install duplicate
copies in multiple discovery locations.

## Permissions, privacy, and cost

No executable scripts, installer, credentials, signing key, or dependency
installation are included. The package does not grant permissions, bypass host
policy, or make provider calls itself. A model following its instructions can
still use tools available in its host: review proposed actions and keep access
scoped to your task. Do not provide secrets or private records for a first trial.

The bundled metadata permits implicit invocation where supported. Use the host's
skill controls if you want to disable it or require explicit invocation.

Client subscriptions, model/API usage, and infrastructure may cost money
separately. Compatibility with other clients is not certified. ChatGPT and Claude
instruction packs are separate packages, not interchangeable installations.

## Updates and removal

Compare the approved version, license, and manifest before updating. Back up an
existing skill before replacing it. To uninstall, remove only the
`harness-agent-builder` folder you installed and refresh the client; do not delete
the entire skills directory. Revoke any separately granted credentials separately.
Removing the skill does not erase previous chats or provider-retained data.

## License

Originally built by **Healthzone MD**.

License identifier: `LicenseRef-Healthzone-MD-Personal-Use-1.0`.
The included `LICENSE.txt` contains the governing terms. Personal, noncommercial
use and customization are allowed. Copies may be shared without charge while
retaining the license and attribution. Modified copies must identify changes and
must not imply Healthzone MD endorsement. Business use, sale, paid redistribution,
or commercial incorporation requires separate written permission. Applicable
third-party terms remain effective.

## Evidence and limitations

Version 1.0.1 changes licensing and packaging metadata; the skill's core files
are unchanged from candidate 1.0.0. Local archive/hash checks, isolated static
scanning, and package review were completed. These are not malware certification,
client runtime certification, independent verification of third-party rights, or
marketplace publication approval. Signing and the marketplace release workflow
remain pending.
