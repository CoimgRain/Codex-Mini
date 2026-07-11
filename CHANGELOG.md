# Changelog

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
