<p align="center">
  <img src="docs/assets/app-icon.png" width="96" height="96" alt="SideSchedule app icon">
</p>

<h1 align="center">SideSchedule</h1>

<p align="center">
  A day-calendar sidebar for macOS that keeps its own strip of screen, the way the Dock does.<br>
  <a href="https://didact.digital/sideschedule/">Website</a> ·
  <a href="https://github.com/4IngoJ/sideschedule/releases/latest/download/SideSchedule.dmg">Download</a> ·
  <a href="https://github.com/4IngoJ/sideschedule/releases">Release notes</a>
</p>

![SideSchedule docked at the edge of a Mac desktop](docs/assets/og-image.png)

Most calendar apps show you your day and then disappear behind whatever window you open next. SideSchedule stays. It reserves a strip at the left or right edge of your screen, and any window that slides under it gets pushed back out, so your next meeting is always in view.

## What you get

- **Your real calendar.** Reads and edits Apple Calendar, which means iCloud, Google, Exchange and CalDAV all work. Drag to reschedule, drop a file or text to block time.
- **Meeting notes as Markdown files.** Type during the call; each note saves as a `.md` file with YAML frontmatter in a folder you pick. Obsidian and Logseq read them as-is.
- **One-click join** for Zoom, Google Meet, Microsoft Teams, Webex and FaceTime, straight into the native app.
- **Next free 30 minutes** in the header, so you don't scan the day for a gap.
- **Auto-hide** to a thin strip that still shows the join button and a countdown.
- **Local-first.** No account, no analytics, no telemetry.

Works on macOS 13 Ventura or later, Apple silicon and Intel, in English, German, French, Spanish, Italian and Portuguese.

## Install

Download [SideSchedule.dmg](https://github.com/4IngoJ/sideschedule/releases/latest/download/SideSchedule.dmg), drag the app to Applications, and allow Calendar and Accessibility access on first launch. It's signed with a Developer ID and notarized by Apple.

Or with Homebrew:

```sh
brew install --cask 4ingoj/tap/sideschedule
```

## Price

Free for 14 days with everything unlocked. After that, [€12.99 once](https://4ingoj.lemonsqueezy.com/checkout/buy/e72e0987-c650-42d1-a936-908168e003f5) for two Macs, with all future updates included. No subscription.

Questions: hello@didact.digital

---

## About this repository

This repo holds the built app, the [Sparkle](https://sparkle-project.org) update feed and the website in `docs/`. The source code is private. `SUFeedURL` in the app points at:

```
https://github.com/4IngoJ/sideschedule/releases/latest/download/appcast.xml
```

which resolves to the `appcast.xml` asset on whichever release is tagged latest.
