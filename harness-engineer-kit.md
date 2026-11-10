# Harness Engineer for Claude Code

Publisher: Healthzone MD. Version: 1.0.1. Status: unsigned candidate; not a published marketplace download.

Archive: `harness-engineer-kit-1.0.1.zip`

SHA-256: `cc3f92db4cf19ee91d179ee4bf54198fc21528856019435bf99862b64eb0bd38`

The following instructions are reproduced from this exact package README. Static checks are not malware or runtime compatibility certification.

---

# Harness Engineer + Harness Engineering Skill

Claude Code release candidate, package version 1.0.1 (first marketplace packaging
version; the source kit declares no release version).

This bundle includes the `harness-engineer` agent definition and its companion
`harness-engineering` skill, with references, JSON templates and source documentation.
It is distinct from the separately packaged Codex `harness-agent-builder` skill.
It is not a standalone application or a guaranteed cross-client agent.

## Important installation warning

The source kit's `install.sh` was deliberately excluded. It unconditionally removes
the existing harness-engineering skill directory and overwrites the agent file.
The original files remain unchanged on the publisher's machine. The included
`harness-kit/README.md` is historical source documentation: its one-command installer
instructions do NOT apply to this package. Follow the manual steps below instead.

## Manual installation

1. Verify the ZIP SHA-256 against the approved product page before installing.
2. Extract into a new temporary folder and inspect every file. `manifest.json`
   records included file hashes and the excluded installer's hash/reason.
3. The supplied kit targets Claude Code's user-level `.claude/skills` and
   `.claude/agents` directories. Confirm your installed client supports these
   locations and formats; desktop visibility and other clients were not tested.
4. Back up any existing `harness-engineering` skill folder and `harness-engineer.md`
   agent file. Compare versions; do not silently overwrite your customizations.
5. Copy `harness-kit/skills/harness-engineering` into your chosen supported skills
   directory, and `harness-kit/agents/harness-engineer.md` into the matching agents
   directory. Preserve all skill subfolders and filenames.
6. Refresh the client's agent/skill inventory or start a fresh session. Confirm
   both definitions are available. Try the source kit's explicit invocation:
   `/harness-engineering audit this repo`, in a disposable non-sensitive repository.
   Review the resulting plan before authorizing any changes.

Keep the supplied `assets/templates/AGENTS.md` as a template. Do not copy it over
your repository's existing agent policy without reviewing and approving its rules.
PROMPT.md is source generation guidance, not an installer or required command.

## Permissions and execution

Downloading or unpacking grants no tool permissions. The supplied agent declares
Read, Grep, Glob and Bash. Bash can modify files and execute commands: the source
agent's "read-only by default" language is an instruction, NOT an enforced sandbox.
Use client permission controls to enforce read-only operation, restrict paths and
require approvals for writes, command execution, network access and spending.
Proactive invocation is requested in the source agent description; configure the
host to match your desired invocation/approval policy.

No scripts, binaries, model credentials, signing keys or runtime dependencies are
included in this distribution. The agent's host can still perform consequential
actions if its operator grants those capabilities. This package does not enforce
or alter the host's security controls.

## Compatibility, cost, update and uninstall

Source-targeted ecosystem: Claude Code. Compatibility with Codex, other hosts,
particular client versions and desktop panels has not been validated. Your model
or client subscription/API usage may cost money; package contents make no API calls.

Updates are manual: inspect the new approved package and manifest, back up the
old definitions, then replace only the intended skill folder and agent file.
To uninstall, remove only those installed definitions and refresh the client.
No package-created service, database or background worker needs removal.

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
