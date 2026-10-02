# Changelog

## v2.0.0 — 2026-10-02
- New quote bank from the latest web version: 66 quotes across Beginner,
  Everyday, and Expert, plus an All Levels round. Every round mixes
  "Who said it?" with "Real or misattributed?" questions, and every answer
  shows the real source and the story behind the quote.
- "How to check a quote before you share it" tips are always on screen.
- Real app look: black launch screen with the big logo (no white box on
  Android 12+), a bigger launcher icon that fits round, squircle, and square
  shapes without clipping the frame, solid app bar, and About / Privacy /
  Credits panels.
- Android back button asks before quitting a round, returns to the level
  picker from results, and asks before exiting.
- Phones and tablets, portrait and landscape: rotates freely, smaller
  start-screen logo on landscape phones.
- Removed the social, fundraising, and "Back to games" links from the new web
  version; a content security policy blocks all network access.
- The `INTERNET` permission that Capacitor merges in is now stripped from the
  final manifest.
- APK renamed to `WGRALGO-WhoSaidIt-v2.0.0.apk`, the same
  `WGRALGO-<AppName>-v<version>.apk` naming as every WGRALGO app.
- Version 2.0.0 (versionCode 200). Signed with a new key: uninstall v1.0.0
  before installing v2.0.0.
- `.gitignore` now excludes keystores and secrets; added GitHub Actions debug
  builds, a signed release workflow, `tools/validate-release.sh`, and
  `tools/build-icons.py`.

## v1.0.0 — 2026-05-26
- Initial GitHub-ready Android APK release.
- Added offline quote-recognition educational game.
- Added randomized 10-question rounds drawn from an 80+ question, attribution-checked quote bank.
- Added 14 wisdom categories: Knowledge, Education, Power, Freedom, Courage, Justice, Leadership, Money and Work, Critical Thinking, Creativity, Discipline, Community, History, Technology and Change.
- Added score tracking, progress bar, difficulty badges, instant correct/incorrect feedback, real-speaker reveal, and quote explanations.
- Added final results screen with five-tier rating system and Play Again.
- Rebuilt the in-app UI as a true standalone app: removed social media bar, GoFundMe bar, WordPress menus, and website footer navigation.
- Switched package name to `org.wgralgo.whosaiditknowledgeweapon`, versionName `1.0.0`, versionCode `100`.
- Removed the `INTERNET` permission; app is fully offline.
- New WGRALGO black-and-gold launcher icon and splash screen built from the official Who Said It? emblem (no white square).
- Added GPLv3 license, privacy statement, contributors file, README, and release-notes folder.
