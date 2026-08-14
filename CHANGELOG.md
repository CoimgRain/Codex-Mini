# Changelog

## v5.5.4 - 2026-08-14

- Added official DeepSeek wallet-balance rings with configurable amount ceilings and OpenCode Go 5-hour, weekly, and monthly quota rings that appear only for the detected provider.
- Remembered the selected DeepSeek balance ring, display state, and amount ceiling while refreshing provider usage every 30 seconds.
- Removed individual text, attachment, image, and video limits while retaining the membership plan's total monthly traffic quota.
- Stopped webpage refresh and background synchronization from repeatedly taking ownership of the task currently selected on the desktop.
- Fixed repeated DeepSeek balance-ring rendering that could freeze the mobile interface after a few swipes.
- Fixed newly created tasks being reclaimed by the previous task, switching away automatically, or receiving the first message in the wrong task.
- Improved cross-task send confirmation and terminal-state classification so failed or incomplete work is not reported as successfully completed.
- Fixed completed-task unread dots remaining visible after the task was opened.
- Published refreshed Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.


## v5.5.3 - 2026-08-11

- Made server membership records authoritative when restoring and displaying entitlements on macOS and Windows.
- Unified task-list and conversation refresh behavior for page open, foreground resume, notifications, and task-state changes.
- Adjusted the top status-capsule safe area for the latest system blur treatment.
- Fixed first-message routing after creating normal and project tasks so messages stay in the new task.
- Fixed completed-task unread dots not appearing or not clearing after the task was viewed.
- Fixed failed tasks occasionally being reported as completed.
- Fixed rename, archive, approval-card, and archive-confirmation actions against the latest GPT interface.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.5.2 - 2026-08-08

- Added forced task-list and conversation refresh after opening a task from a message notification.
- Restored fast-mode state reading and switching after the 5.5.1 frontend regression.
- Restored clipboard image paste into the attachment queue while preserving accompanying text.
- Improved queued-message detection and live synchronization for the updated GPT / Codex interface.
- Extended hour-and-minute duration formatting to running, completed, failed, and stopped tasks.
- Added atomic membership-state writes and local backup recovery to reduce entitlement loss during upgrades.
- Fixed Windows controlled-GPT relaunch after the GPT client had been closed.
- Fixed Windows Max membership upgrade recovery and several control-panel clipping issues.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.5.1 - 2026-08-06

- Reissued the fully validated macOS, Windows, and Android release under the correct GPT Mini v5.5.1 formal version.

- Added an animated right-side quick-action control with configurable visibility and spacing that adapts to the number of actions.
- Added independent collapse controls for pinned, project, SSH, and conversation task sections while keeping SSH tasks visible when projects are collapsed.
- Added web and discounted WeChat payment choices, Pro pricing, Max lifetime membership guidance, and per-device notification controls.
- Unified the macOS and Windows control-panel layout, typography, icons, status capsules, connection flow, and membership presentation without changing platform-specific startup behavior.
- Improved plan progress capsules, queued-message stacking, long-running duration formatting, image previews, and DeepSeek V4/V4-Pro model labels.
- Improved project task creation so project, branch, and Worktree choices remain aligned and the new task stays selected.
- Fixed brief replay of the previous completed reply after sending a new instruction, temporary mobile image expiry, and SSH sections disappearing after project collapse.
- Removed custom clipboard polling that interfered with native paste/read menus on iPhone, iPad, and Safari.
- Fixed Windows membership expansion, text overlap, payment alignment, and related control-panel spacing issues.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.5.0 - 2026-08-06

- Added an animated right-side quick-action control with configurable visibility and spacing that adapts to the number of actions.
- Added independent collapse controls for pinned, project, SSH, and conversation task sections while keeping SSH tasks visible when projects are collapsed.
- Added web and discounted WeChat payment choices, Pro pricing, Max lifetime membership guidance, and per-device notification controls.
- Unified the macOS and Windows control-panel layout, typography, icons, status capsules, connection flow, and membership presentation without changing platform-specific startup behavior.
- Improved plan progress capsules, queued-message stacking, long-running duration formatting, image previews, and DeepSeek V4/V4-Pro model labels.
- Improved project task creation so project, branch, and Worktree choices remain aligned and the new task stays selected.
- Fixed brief replay of the previous completed reply after sending a new instruction, temporary mobile image expiry, and SSH sections disappearing after project collapse.
- Removed custom clipboard polling that interfered with native paste/read menus on iPhone, iPad, and Safari.
- Fixed Windows membership expansion, text overlap, payment alignment, and related control-panel spacing issues.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.4.2 - 2026-07-29

- Added desktop Safari website-notification setup for saved Mac and Windows device profiles.
- Improved notification-click routing so same-device tasks open directly while cross-device tasks ask before switching through the existing device switcher.
- Replaced the full-screen cross-device prompt with a compact Liquid Glass notice below the top capsule.
- Increased the seven-day trial traffic allowance to 7 GiB.
- Added clear Max lifetime membership purchase and two-group QQ support guidance to the macOS and Windows control panels.
- Fixed Windows non-interactive SYSTEM launches from taking ownership of the signed-in user's GPT Mini state or backend.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.4.1 - 2026-07-26

- Improved Windows control-panel startup responsiveness by rendering the first screen before serial low-priority service and status work begins.
- Improved controlled GPT readiness checks with bounded TCP/CDP phases, cached Node discovery, and cooldown protection against repeated relaunches.
- Reduced repeated listener enumeration and synchronous status work that could make the Windows panel feel stuck while opening.
- Published the Windows x64 installer only; macOS remains on v5.4.0 and Android remains on v2.0.3.

## v5.4.0 - 2026-07-26

- Added goal and plan modes to the mobile interface, including native goal actions and full-screen Markdown plan review, adjustment, execution, and skip controls.
- Added complete touch scrolling for long plans while keeping the action area and adjustment input accessible.
- Improved the add menu with composer-matched Liquid Glass styling, full-row hit targets, outside dismissal, lower opening cost, and more stable mobile keyboard focus.
- Improved context usage reporting to follow the latest real GPT/Codex value after compaction instead of retaining a locally inferred older value.
- Improved entitlement resilience so transient network or service failures retain a locally valid membership and retry automatically.
- Fixed Windows control panels reusing an incompatible older backend, which could break Pro status, phone connectivity, notifications, new-task options, attachments, and version reporting together.
- Fixed web-push subscription failures, misleading new-task read errors, attachments downloading as file.json, missing icon/math assets, and incorrect local attachment routing.
- Fixed plan-card overlap, blocked touch scrolling, and add-menu areas that could not be tapped.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.3.6 - 2026-07-22

- Added automatic Worktree creation when selecting a non-main branch before creating a task on macOS and Windows.
- Added Mermaid flowchart rendering with dark-theme colors, full-screen viewing, and horizontal navigation.
- Added a unified pinned area for pinned tasks and pinned projects, plus an optional top fade-glass appearance setting.
- Improved task selection, project grouping, pin state, and ordering to follow the official GPT desktop task list more closely.
- Improved foreground resume and completed-result display while moving full-history reconciliation to the background.
- Fixed SSH groups disappearing after refresh, pinned items falling to the bottom, and completed replies replaying briefly after reopening a task.
- Fixed Windows update verification on PowerShell environments without `Get-FileHash` by using the built-in .NET SHA-256 implementation while retaining mandatory size and digest checks.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.3.5 - 2026-07-20

- Added Windows system-tray residency so minimizing or closing the control panel keeps GPT Mini available and the window can be restored from the tray.
- Improved project and task synchronization with the latest GPT sidebar identifiers, deletion state, pinned order, and provisional-to-final task identity changes on macOS and Windows.
- Improved SSH project and task ordering to follow the GPT sidebar before falling back to update time.
- Improved model, reasoning-level, and permission handling before the first message in a newly created blank task.
- Fixed newly created tasks jumping back to the previously selected task during list refresh.
- Fixed successful task creation being reported as failed when GPT had already entered the new blank task.
- Fixed branch detection for Git repositories that do not yet have an initial commit.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.3 universal WebView download assets.

## v5.3.4 - 2026-07-19

- Added new-task creation inside the currently selected SSH remote project on macOS and Windows.
- Improved entitlement-state synchronization and secure relay validation across both desktop platforms.
- Reworked completion and live-progress notification scanning to process only appended conversation data.
- Fixed notification scanning saturating the local backend when many recent or long conversations were present.
- Fixed model switching from sending a global Escape action that could interrupt a running task.
- Published matching Apple Silicon, Intel, Windows x64, and Android v2.0.2 universal WebView download assets.

## v5.3.3 - 2026-07-17

- Enabled the first public Windows one-click update target for users already running GPT Mini 5.3.2 or later.
- Improved new-task defaults to use local execution, the project's main/default branch, and no extra Worktree by default.
- Improved project task creation against the latest GPT sidebar project identifiers and branch-loading behavior.
- Improved desktop-upgrade prompts and settings typography hierarchy across the shared mobile interface.
- Fixed newly created tasks being replaced by the previously selected task during list refresh.
- Fixed project task creation failures being reported as a generic CDP port problem instead of the actual failing stage.
- Fixed highest and ultra reasoning badges temporarily using the medium-state color before live capabilities finished loading.
- Refreshed the GPT Mini v5.3.3 Android download asset to the independent repository's v2.0.0 universal WebView build.

## v5.3.2 - 2026-07-17

- Added customizable three-ring context, 5-hour quota, and weekly quota visualization.
- Added API Key and CCSwitch model-catalog discovery while preserving existing account and catalog behavior.
- Added an optional real-time progress notification setting, disabled by default.
- Improved model-specific reasoning-level discovery so the menu shows only capabilities supported by the current model.
- Improved model and reasoning menu caching, settings layout, version display, and Grok process-capsule presentation.
- Fixed API-login models appearing gray or switching to the wrong catalog entry.
- Fixed Kimi K3 and other relay models reporting a failed footer confirmation after a successful switch.
- Fixed queued-message guidance targeting after quota notices changed the composer layout.
- Fixed incomplete Grok/relay token events reducing context usage to an incorrect value near 1%.
- Fixed explicit user-stopped tasks being reported as model failures.
- Published matching Apple Silicon, Intel, Windows x64, and Android v1.25.10 ARM64 download assets for GPT Mini v5.3.2.

## v5.3.1 - 2026-07-16

- Added automatic controlled-mode handoff when GPT Mini is already running and the user opens the official GPT client, while preserving confirmation for an existing working session.
- Added the latest Android v1.25.6 ARM64 package from the independent Android release repository.
- Improved task-plan expansion, progress animation, high-refresh rendering, and completed-task history restoration.
- Improved automatic retry and recovery for initial configuration and encrypted LAN connection negotiation.
- Improved Mac controlled-mode handoff latency and Windows controlled-client status tolerance.
- Fixed normal-chat task creation, cross-project selection, and accidental project inheritance.
- Fixed branched tasks created as a new task or Worktree not appearing in the mobile task list.
- Fixed reasoning-strength badges showing state from another task after switching tasks.
- Published matching Apple Silicon, Intel, Windows x64, and Android download assets for GPT Mini v5.3.1.

## v5.3.0 - 2026-07-16

- Upgraded the public remote-access entry from HTTP to HTTPS on macOS and Windows. Users should rescan or recopy the full URL; existing iOS Home Screen Web Apps should be re-added from the HTTPS URL.
- Added project, runtime location, Git branch, and isolated Worktree choices when creating a task, plus Worktree markers in the task list.
- Added automatic encrypted LAN DataChannel routing with public-relay fallback and improved multi-device primary-device deduplication.
- Updated model labels to match the current official catalog and exposed the highest reasoning level only when the account actually supports it.
- Added Windows in-app update checks and one-click installation for future releases.
- Improved Liquid Glass cards, task-plan progress, queued-message presentation, iOS keyboard layout, task-state caching, and background polling efficiency.
- Changed completion notifications so background tasks no longer replace the task currently being viewed; navigation happens only after the user clicks the notification.
- Fixed iOS Home Screen Web App credential recovery, collapsed pinned/project task selection, minimized-window sending, missing projects, stale gray model badges, and duplicate Mac device entries.
- Published matching Apple Silicon, Intel, Windows x64, and Android download assets for GPT Mini v5.3.0.

## v5.2.2 - 2026-07-14

- Added incremental live rendering for GPT reasoning and final replies, with smoother handoff to completed task history.
- Added native task-plan cards with expandable steps, progress, and code-change summaries.
- Added iOS Bark notifications for Pro and Max users when tasks complete or stop with an error.
- Added Max multi-device connections with a fixed primary device, per-device colors, and quick switching.
- Improved model, reasoning, and standard/fast mode controls for newly created tasks.
- Improved model ordering, full/short model-name display, fast-mode status, and responsive control sizing.
- Improved cached task switching, iPad sidebar behavior, long task titles, pinned styling, and streaming Markdown rendering.
- Fixed repeated reasoning or reply content during live output and after task completion.
- Fixed Max entitlement state being lost during startup or after switching to a secondary device.
- Fixed internal process labels, bold stage markers, and non-reply content leaking into the main conversation.
- Published matching Apple Silicon, Intel, Windows, and Android download assets for GPT Mini v5.2.2.

## v5.2.1 - 2026-07-12

- Added online verification for bare domains so only real reachable websites become clickable links.
- Changed the context compression action to use GPT's native compact command instead of sending plain text.
- Improved localized failure details for quota, sign-in, network, connection-reset, and service errors.
- Improved automatic standard/fast mode refresh without opening the model or reasoning menu.
- Fixed newly created tasks becoming temporarily unselectable when the desktop client used a provisional task ID.
- Fixed internal reasoning-stage headings appearing as large bold reply text instead of compact process capsules.
- Fixed repeated normal-task creation on Windows after completing a reply.
- Fixed intermittent local relay connection resets during message sending and status refresh.
- Improved Mac guardian behavior after membership expiry, remote activation, and lid-close transitions.
- Fixed Android non-Liquid-Glass composer and light thread-menu visibility combinations.
- Published matching Apple Silicon, Intel, Windows, and Android download assets for GPT Mini v5.2.1.

## v5.2.0 - 2026-07-11

- Officially renamed the user-facing product from Codex Mini to GPT Mini while preserving existing settings, entitlement, thread, and access data during upgrades.
- Added compatibility with the merged ChatGPT/Codex desktop client on macOS and Windows, including controlled-client startup and current model/reasoning state detection.
- Introduced the Liquid Glass interface across thread navigation, status controls, composer, menus, and responsive mobile/tablet layouts.
- Added three-ring context and account-quota visualization, expanded model/reasoning controls, standard/fast mode switching, and per-status display customization.
- Improved cached thread switching, background refresh after returning to the page, 40-message history paging, and on-demand rendering of detailed process steps.
- Improved tool-process capsules with localized, natural-language labels while filtering internal stage markers and parser noise from replies.
- Expanded attachment and generated-image preview/download support, queue controls, clickable URLs, long thread titles, and mobile scrolling behavior.
- Fixed model selection briefly reverting to the previous model, duplicate pasted images, broken queue deletion, missing failure details, and stale thread content.
- Published matching Apple Silicon, Intel, Windows, and Android download assets for GPT Mini v5.2.0.

## v4.5.2 - 2026-06-30

- Published Apple Silicon, Intel, Windows, and Android download assets for Codex Mini v4.5.2.
- Added project thread expand/collapse behavior so large project lists stay compact.
- Improved mobile settings organization, entry icons, status-display ordering, and status indicator animation.
- Fixed internal process summaries and handoff notes appearing in mobile replies.
- Fixed attachment cards being inserted into the middle of replies or misdetected from Markdown text.
- Fixed the Mac guardian screen so changing thread-card visibility refreshes immediately.

## v4.4.2 - 2026-06-20

- Published Apple Silicon, Intel, and Windows installers for Codex Mini v4.4.2.
- Added older-thread loading for the mobile thread list.
- Fixed SSH remote threads being hidden by local thread pagination.
- Published a cleaner Windows installer payload with runtime files only, excluding internal docs, packaging scripts, and build source.

## Unreleased

- Converted this branch into a local-only open-source edition.
- Removed hosted access, payment, activation, and test-build distribution code paths.
- Kept the core local phone-to-Codex bridge, thread list, send, status, model menu, and macOS wrapper app.
