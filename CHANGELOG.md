# Changelog

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
