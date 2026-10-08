# Stage learning

**Learn at your level, one idea at a time, with a patient mentor.**

A Claude skill that teaches any concept like a patient mentor, built for people with a short attention span or ADHD.

Inspired by videos where an expert explains one concept at several levels, from a child to a fellow expert. Stage learning explains the same idea at the depth that fits you. The levels aren't a ladder you have to climb: a good explanation at your level is a complete session, and going deeper is always your choice.

Making explanations shorter isn't enough: short and dull is still dull. So it starts from what you already know, makes you curious before it explains, and builds each idea on what you just said.

## How it works

1. **It asks how familiar you are,** and that's all it asks to start:
   1. Never heard of it
   2. Heard of it, but couldn't explain it
   3. Can explain the basics
   4. I know quite a bit but would like to learn more

   Your answer sets how deep it starts. If you've already said how much you know, it skips this question. If you pick 4 on a broad topic, it asks which part you want to learn more about.
2. **One idea at a time.** Each idea opens with the real problem it solves, then a short explanation. It only asks you a question on the trickier ideas, so it never feels like a quiz. No "ready?" prompts; it flows like a conversation.
3. **It goes deeper when you're ready.** When you've got the basics, it asks if you want to go deeper. You never see levels, stage numbers, or step counters.
4. **A light ending.** When the core idea has landed, it closes with a conversational question like "How would you explain this to a friend?" Review questions go in your notes, so you can test yourself later.
5. **Notes saved automatically.** You get a `learning-notes-<topic>.md` file with what you can explain, tricky spots, and review questions. Upload it next time to pick up where you left off.

Wrong answers are welcome. If you get something wrong, it just explains the right answer clearly and carries on, with no fuss and no re-asking. Want another go? Just ask.

**You're in charge.** Whatever you ask for ("explain it all at once," "no questions," "longer explanations") comes first and stays that way until you change it.

It's designed around common ADHD challenges (holding things in mind, getting started, staying motivated), but it isn't a clinically validated method.

## Things you can say anytime

The mentor never shows you a list of commands, but it responds to these:

| Say | What happens |
|---|---|
| "too easy" / "harder" | A tougher challenge, or an offer to go deeper |
| "simpler" / "I'm lost" | Re-explains the current idea more simply |
| "shorter" / "longer" | Changes explanation length from then on |
| "example" | Another concrete example |
| "skip" | Moves on without answering |
| "save this" | Saves your notes |
| "done for today" | Stops right away and saves your notes |

## Example

> **You:** Teach me compound interest.
>
> **Mentor:** How familiar are you with compound interest?
>
> 1. Never heard of it
> 2. Heard of it, but couldn't explain it
> 3. Can explain the basics
> 4. I know quite a bit but would like to learn more
>
> **You:** 1
>
> **Mentor:** With compound interest, your savings can earn more interest in the second year even if you add nothing. That's because the first year's interest starts earning interest too...

## Installation

### In the Claude app (web, desktop)

Skills work on all Claude plans, including Free.

1. Download `stage-learning.zip` from this repo: click the file, then the download button.
2. In Claude, make sure **Code execution and file creation** is turned on: **Settings → Capabilities** (Free, Pro, Max), or **Organization settings → Plugins & skills** (Team, Enterprise).
3. Go to **Customize → Skills**, click **+**, choose **Create skill**, then **Upload a skill**, and select `stage-learning.zip`.
4. Start a new chat and ask to learn something, like "Teach me how vaccines work."

### In Claude Code

Clone the repo into your personal skills folder:

```
git clone https://github.com/GurungGaurab/stage-learning ~/.claude/skills/stage-learning
```

Then ask Claude Code to teach you something, or type `/stage-learning`.