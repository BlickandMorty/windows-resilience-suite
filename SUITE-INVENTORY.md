# Source Inventory and Publication Map

## Histories reviewed completely

- `lockdown`: 164 turns across 17 pages; 187 user messages and 300 recorded file-change operations.
- `performance`: 129 turns across 13 pages; 131 user messages and 331 recorded file-change operations.
- `Keep X.com blocked`: 5 turns, including the permanent guardian, protected ACLs, HMAC manifests, optimization, and policy-maintenance work.
- `Find leftover game data`: 2 turns covering Steam, Epic, and Xbox remnant auditing and approved cleanup.
- `MyDell / Codex backup restore`: 3 turns covering user-profile migration, locked-file restore failures, and safe restore staging.
- `Reuse GAMD1`: reviewed, but music-download/stream-ripping material is intentionally excluded because it conflicts with the permanent music-streaming boundary. Its unrelated backup/documentation patterns were considered.

## Authoritative artifact families reconciled

### AI workspace safety

The expanded project scope adds a vendor-neutral enterprise boundary for annotation, evaluation, recruiting, and research workflows. It combines fail-closed agent preflight decisions with real Windows identities, project-specific zones, SID-based role mappings, NTFS enforcement, integrity manifests, a hash-chained evidence ledger, export approval, and scheduled verification. It explicitly rejects the false claim that an AI process can be distinguished from a human when both share one Windows identity.

### Windows lockdown

The historical source tree contains 59 numbered PowerShell stages, a shared library, a central JSON policy, browser policy generation, hosts-file enforcement, app/installer blocks, NextDNS integration, verification, packaging, and multiple compatibility repair stages. The installed system contains:

- a SYSTEM network enforcer;
- startup, sign-in, and hourly reapplication;
- a signed NextDNS installer cache and resilience logic;
- Chrome and Edge managed URL policies;
- a hosts-file fallback;
- executable-name restrictions;
- five protected copies of the standing rule;
- two guardian replicas that cross-repair;
- HMAC-authenticated manifests and repair baselines;
- SYSTEM-owned, non-writable protection artifacts;
- continuous and scheduled integrity checks.

Historical one-off download windows, temporary allow rules, raw NextDNS account/profile material, live manifests, live HMAC material, and machine-specific policies are not publishable. The public project keeps only install, strengthen, verify, export-denylist, and repair behavior.

### Protected files and agent policy

The later guardian work established an important technical boundary: an AI agent is not a Windows security principal. If the agent runs as the interactive user, Windows cannot distinguish it from that user. A protected SYSTEM task or separate service account can be authorized to update guarded files, but an administrator can ultimately take ownership unless credentials or device management are controlled externally.

The public protected-paths project therefore uses accurate terms:

- `ReadOnlyForUser`: the selected user gets read/execute access but no write/delete access;
- `SystemManaged`: SYSTEM owns and repairs the ACL and optionally restores file contents from a canonical copy;
- `IntegrityOnly`: hashes are monitored without changing access.

It never promises “only the AI can edit.” Reserved permanent-hard-gate targets cannot be unprotected through the public tool.

### Lean performance V2

The canonical performance family includes:

- audit-only, user-safe apply, protected admin finalize, optional ultra-minimal, restore, and verification modes;
- Dell/Intel/NVIDIA guardrails;
- service and scheduled-task baselines;
- protected task pruning;
- user privacy/UI/right-click adjustments;
- temporary-file and report retention cleanup;
- Delivery Optimization cleanup;
- SSD retrim/optimization;
- DISM and SFC verification/repair;
- Dell Command Update scanning and post-reboot verification;
- cold-shutdown and lid-close safety settings;
- startup, sign-in, post-update, daily, weekly, and self-heal maintenance;
- reports, status summaries, and SHA-256 manifests;
- backup publication and canonical-copy verification.

The public performance repository keeps conservative, reversible, broadly portable operations. Device-specific Dell update automation and aggressive service pruning are documented as optional extension points rather than enabled defaults.

### Gaming performance

The gaming work includes:

- adaptive AC/battery processor policies;
- NVIDIA/Intel per-application GPU routing;
- Steam library discovery and game inventory refresh;
- safe-windowed launch arguments for supported engines;
- display-mode safety checks;
- lid-close safety checks;
- hidden power-change and sign-in tasks;
- a small profile-control interface;
- drift repair and status reporting.

Machine-specific game paths and storefront inventories are replaced with discovery and an editable example configuration.

### Maintenance orchestration

The complete scheduler grew from five tasks to a robust set including:

- daily user maintenance;
- weekly elevated maintenance;
- startup SYSTEM refresh;
- post-sign-in user refresh;
- post-Windows-Update refresh;
- shutdown/restart marker handling;
- periodic self-heal/watchdog;
- task visibility-aware verification;
- hidden launchers and logs;
- explicit manual run modes for testing.

The public project keeps these as an independent orchestrator so users can install the scheduler without adopting every performance tweak.

### Cleanup and remnants

The reviewed cleanup work covered:

- Steam manifests versus orphaned directories;
- Epic manifests, launcher cache, and residual game settings;
- Xbox/Appx orphan packages;
- Riot, Ubisoft, Battle.net, and anti-cheat preservation;
- NVIDIA and Direct3D shader caches;
- crash dumps, stale installers, and old temp data;
- strict exact-path deletion guards;
- preview reports and post-clean verification.

The public cleanup project is audit-first. It emits a plan with hashes and requires a second, explicit approval step before deletion.

### Backup and integrity

The source work includes canonical ZIP publication, readable-archive tests, SHA-256 manifests, copy verification, retention, profile-path migration checks, and Codex-state backup/restore behavior. The public backup project separates backup creation, verification, and restore staging. It refuses to overwrite an active destination by default.

## Deliberate exclusions

- NextDNS API keys, profile IDs, account URLs, and live policy IDs.
- Guardian secrets, DPAPI blobs, live HMAC manifests, hashes, repair targets, and task identifiers from the protected laptop.
- Personal names, email addresses, user-profile paths, device IDs, installed-app inventories, game libraries, school data, and diagnostic reports.
- Historical ZIPs and duplicate source snapshots.
- Temporary scripts created solely to uninstall an app or delete a one-time exact path.
- Scripts that disable, remove, bypass, downgrade, or explain how to defeat a permanent protection.
- YouTube, X/Twitter, adult-content, or non-Qobuz music-streaming access/download helpers.
- Claims that local ACLs are mathematically irreversible while the operator remains a Windows administrator.

## Repository lineage

Every published project links back to this inventory through a `LINEAGE.md` file describing which original feature families it reconstructs. No live-machine file is copied verbatim unless it has been reviewed for portability, licensing, secrets, personal data, and safety.
