# Harness Engineer for Codex

Publisher: Healthzone MD. Version: 1.0.1. Status: unsigned candidate; not a published marketplace download.

Archive: `harness-engineer-codex-1.0.1.zip`

SHA-256: `f6663c4d02a2a37b67ebcd52d095bdb492cc34b2addf28d7b0d7d70e945c0e66`

The following instructions are reproduced from this exact package README. Static checks are not malware or runtime compatibility certification.

---

# Harness Engineer for Codex — candidate 1.0.1

Native custom-agent TOML and a discoverable harness-engineering skill adapted from
the supplied Claude kit. No fixed model, shell installer, MCP connection or
credential is included. Review all files and the manifest before installation.

Manual setup: in a trusted test repository, copy the provided .codex/agents file
and .agents/skills/harness-engineering folder to the matching repository paths.
Back up existing definitions first; this name may already exist on your machine.
Do not replace your config.toml or AGENTS.md. Start a fresh Codex session and
confirm discovery. Invoke $harness-engineering for a focused audit; ask to use
the harness-engineer subagent only if your client supports custom agents.
If it does not, use the skill without claiming subagent execution.

Models and tools depend on the receiving host. Read-only prose is not a sandbox;
retain host permission controls and explicitly authorize consequential work.
Uninstall only the files you installed, or restore your backed-up definitions.
Do not install duplicate skill copies in multiple discovery locations.

The package was structurally validated, not installed or live-model tested on
your account. Runtime loading, behavior and client/version compatibility remain
to be confirmed. No paid calls were made. Provider/client charges may still apply.

## License and attribution

Originally built by Healthzone MD.
This package uses the Healthzone MD Personal-Use License v1.0; see LICENSE.txt
for the approved terms. Personal, noncommercial use and customization are allowed.
Original or modified copies may be shared without charge while retaining the
license and attribution. Identify modifications and do not imply endorsement.
Business use, sale, paid redistribution or commercial incorporation requires
separate written permission. Applicable third-party terms remain in effect.

Version 1.0.1 changes licensing, attribution and packaging metadata only.
Agent/skill instructions, resources and templates match the prior 1.0.0 package.
License approval is not security review, signing or marketplace publication.
This remains an unsigned candidate; no tools or execution permissions are granted.
The publisher's authority over third-party material was not independently verified.
