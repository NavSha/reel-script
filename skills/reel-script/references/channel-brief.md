# Channel brief

Each channel keeps one `CHANNEL.md` in its own repo, next to its scripts. The skill reads
it before every script. One copy only: reviewers add house rules there, so it stays current.

## Known Airtribe channels

| Channel | Brief | Scripts |
|---|---|---|
| Instagram @build.with.navneet (Navneet, first person) | `NavSha/navneet-socials` → `instagram/content/CHANNEL.md` | same folder, `scripts.md` |
| Instagram @airtribe.live (brand) | `NavSha/airtribe-socials`: no brief yet, ask the questions below | not set |

Both repos are private. No local clone? Read the brief with
`gh api repos/<owner>/<repo>/contents/<path> --jq .content | base64 -d`. No access? Ask
Navneet to add you; do not write a script for a known channel without its brief.

## New channel

If a channel has no brief, ask these questions in one message and save the answers in this shape.

```markdown
# CHANNEL.md · <handle>

## Audience
<Who watches, age, country, job. What they want from the channel.>

## Presenter and voice
<Who is on camera. First person or brand voice. Words they use and never use.
Brand voice skill to run, if any.>

## Close channels (check before every script)
<6–12 handles that post on the same topics for the same audience.>

## CTA style
<Comment keyword + DM resource? Link in bio? Question? Who sends the DMs?>

## Formats we can make
<Talking head, screen recordings, AI avatar, B-roll, carousels. What we cannot make.>

## House rules
<Lasting preferences from the reviewer, one line each, with the date.
Topics or claims never to make.>

## Where scripts live
<Path to the scripts file, how it is published or shared, who approves.>
```

## Questions to ask when there is no brief

1. Who is the audience (age, country, job), and what do they come to the channel for?
2. Who is on camera, and what voice: first person or brand?
3. Which 6–12 channels post on the same topics for the same audience?
4. How do you end reels: a comment keyword with a DM, a link, or a question?
5. What can you film or produce, and what can't you?
6. Anything never to say or show?
