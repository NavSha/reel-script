---
name: reel-script
description: Write short vertical video scripts (Instagram reels, YouTube Shorts) for @build.with.navneet, @airtribe.live or a new channel, that a stranger keeps watching and acts on. Researches the facts, checks what similar channels already posted, finds one core idea with a takeaway the viewer can use, then writes the hook, body, analogy, comment-keyword CTA, DM resource and caption, and runs an AI-slop and honesty check. Use when someone asks for a reel script, a short video script, a hook, a reel caption or DM, or to review, tighten or fix an existing reel script. Not for long YouTube videos, carousels or blog posts.
---

# Reel script

One script at a time, about 45–60 seconds spoken. Most viewers do not follow the channel
(on our reels about 9 in 10 views come from strangers). A stranger keeps a reel only if it
is clear in two seconds and gives them something to use. Honesty is the brand: every
claim must survive a comment from someone who knows the topic.

Built from 19 scripts for @build.with.navneet (Oct–Nov 2026) and the edits the reviewer
made to each one. The before/after edits are in `references/hooks.md` and
`references/examples.md`.

## 0. Read the channel brief

Every channel has a short brief: audience, voice, close channels, CTA style, house rules,
where scripts live. `references/channel-brief.md` lists where each Airtribe channel's
brief lives (@build.with.navneet, @airtribe.live). Not listed? Look for `CHANNEL.md` next
to the scripts file, or ask the questions in that file in one message and save the
answers as `CHANNEL.md`. Do not guess the audience.

If the channel has an idea inbox (for example `ideas/inbox.md`), read it first and keep
the person's own words about why the idea caught their eye. An angle or keyword that a
bot added is a suggestion only.

## 1. Get the facts

- Start at the primary source: the company post, the filing, the founder's own words.
  Blocked (X often returns 402)? Try the `x-video-inspect` skill or `grok -p` for X posts,
  then a news outlet that quotes it. Say in Source notes what you could not open.
- Then get the reaction. Run the `last30days` skill when it is installed. A plain web search
  missed the whole Sarvam backlash; it lived on X and YouTube. No `last30days`? Do at least
  4 searches that include "X", "Reddit" and "YouTube" reaction, and say it was skipped.
- Write every fact with its source under **Source notes**. Mark numbers you worked out
  yourself as "our maths" and show the sum.
- **Sources disagree?** Use wording that is true under both ("a real coding project"),
  and note the conflict.
- **One person's claim** (a single tester's result) can go in only as theirs: "he says",
  "in his test". A number from an anonymous or unverified post stays out.
- **Freshness.** How old is the news on the likely shoot day? Past about 5 days, a pure
  news hook goes stale: lead with the takeaway instead, or park it.
- List the facts that can change before the shoot (share price, valuation, model list,
  prices, "still cloud-only"). They go in **Status** as a shoot-day re-check.

## 2. Check close channels

Look at the last ~6 reels of each close channel in the brief. If one covered the topic in
the last two weeks, find an angle they did not take, or drop the topic. (We skipped this
twice; both topics had already done 500K+ elsewhere.)

How: the brief says where (a browser session with cookies, or the latest weekly
competitor pull). If you cannot check, do not drop the topic: write "competitor check
not run" in **Status** so the reviewer runs it before the shoot.

## 3. Find the takeaway

Ask: after 50 seconds, what can the viewer do, try or decide? No answer means no script.

- News only, or scary only: find the useful angle, or park it. "AI might kill us" with no
  action was parked. Ashton Kutcher's Anthropic win became "bet on the shift in your own job".
- A news peg you cannot show: move to the closest thing you can. Google's new model was
  cloud-only, so the reel shows Google's free model running on a laptop.
- A meme: tie it to a skill. The Bond casting joke became "here is how I made my
  audition from one selfie".

Pick one of the five shapes that win (data: 13 channels, Sep 2026):
1. Named person or company + one number + stakes.
2. Free tool + a comment keyword for the link.
3. Something physical and surprising, with a benchmark.
4. Career or money utility.
5. Your own build, with receipts.

Opinion pieces and "should you switch?" takes did not win on any channel we tracked.
If no shape fits, the takeaway must be a concrete method the viewer can copy (a test, a
prompt, a setup). Record the shape in the **Format** line.

## 4. Write the hook

Rules and before/after examples: `references/hooks.md`. Short version:
- The first line carries a name, a number or a frame the viewer already knows.
- Tension in the first sentence: a loss, a twist, a contrast.
- Under 20 words, at most two sentences, quotes included. It must be true exactly as worded.
- If the reviewer gives you a hook, use it word for word.

## 5. Write the body

- **One core idea.** Side points go to the DM or to another reel.
- **One analogy from daily life**, said in 2–3 sentences. Ours that worked: land near a
  metro line before it opens; a "Made in India" phone (designed vs assembled); a taxi vs
  your own scooter; surfing one wave then paddling for the next.
- **About 3 numbers** (money, percentages, counts of users; dates and "three steps" don't
  count), spoken the way people say them: "seven and a half billion", not "$7.5B" or "1.6×".
- **No jargon the audience would not use.** "He invested", not "his fund". "The one that
  makes Claude", not "the frontier lab". Any name the audience may not know gets a
  "what it is" in about five words (the brief can list names they already know).
- **Reveal late, explain early.** Hold back a name if the frame is stronger (the actor is
  named on line 3). Explain any term the first time it appears.
- **110–150 words** for 45–60 seconds (about 2.5 spoken words a second).

## 6. End with the takeaway, then the CTA

- Takeaway first, as an action: "Start with one task you do every week. Do it with AI this week."
- CTA: "Comment KEYWORD and I'll send you …". The keyword is one word that matches the
  takeaway (070 used SHIFT, not KUTCHER), so it still makes sense after the news is old.
- Write the **DM in full**. It must be usable in about 10 minutes: steps, a link, a list.
  Put requirements here (RAM, price, OS), not in the script.
- No resource fits? End on a real question instead (072: "What do you think Perplexity's
  fourth bet will be?"). Do not invent a freebie.

## 7. Check before you show it

Run `references/checklist.md` top to bottom. It covers:
- **AI-slop**: invoke the `no-ai-slop` skill (Skill tool) on the script, DM and caption if
  installed, take its edits, and keep our block format. Then the patterns we kept catching.
- **Honesty**: overclaims, single-source claims, own maths, money and rumours.
- **Rights**: other people's faces, logos, music, AI labels.
- **Brand**: run the brand voice skill when the brief names one (for Airtribe, `airtribe-voice`).

Fix what fails. Do not show a script that fails a check.

## 8. Show it

Use the block format in `references/format.md`. Add it to the channel's scripts file as
`draft` if the brief names one (next number: grep for the highest `## NNN`). Commit,
push or republish only as far as the brief allows. Never post to a social account.

Reply in the order set in `references/format.md` ("Reply to the reviewer"): full script,
DM and caption, then **1–3 concrete suggested edits** with the new line written out.
No menu of ten hooks. One alternative hook at most.

## When the reviewer edits

- Apply the edit everywhere it fits in the batch, not only to the line they pointed at.
- Keep their lines word for word, even when a slop rule would change them (a joke may use
  "not X, Y" on purpose).
- If the edit is a lasting preference ("say invested, not fund"), add it to the channel
  brief's house rules so the next script starts with it.
