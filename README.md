# reel-script

A Claude Code skill for short vertical video scripts (Instagram reels, YouTube Shorts) that a stranger keeps watching and acts on.

It researches the facts, checks what similar channels already posted, finds one core idea with a takeaway the viewer can use, then writes the hook, body, analogy, comment-keyword CTA, DM and caption, and runs an AI-slop and honesty check.

Built from 19 reviewed scripts for Instagram @build.with.navneet (Oct–Nov 2026).

## Install

Paste this into Claude Code:

```text
Install the /reel-script skill globally from https://github.com/NavSha/reel-script
```

Or with `npx`:

```sh
npx skills add NavSha/reel-script --skill reel-script --global --yes
```

Or copy `skills/reel-script/` into `~/.claude/skills/`.

Works best with [no-ai-slop](https://github.com/petergyang/no-ai-slop) installed.

## Use

Ask Claude Code: "Write a reel script for <your channel> on <topic or link>". The first time, it asks six questions about your channel and saves the answers as `CHANNEL.md`.
