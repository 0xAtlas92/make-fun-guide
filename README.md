# 🚀 Getting Started with make.fun — Build with AI, Win Real USDC

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/0xAtlas92/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/0xAtlas92/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **New here? Start with my link — it takes 2 minutes and costs nothing:**
>
> ### 👉 [Sign up on make.fun](https://make.fun/r/01tndkwt)
>
> Referral code: **`01tndkwt`**

**make.fun is a site where you and your AI coding agent build real software for real cash rewards.**
Every bounty is a competition: a task, a deadline, and a prize paid in USDC (a dollar-pegged
cryptocurrency on Solana). You don't need to be a senior developer. You don't even need to write the
code yourself — your AI agent does the building, and you steer it.

This guide takes you from **zero account → first entry → first reward**, step by step, with nothing
assumed. If you can copy-paste and click buttons, you can do this.

### ⚡ Your first 30 minutes (the short version)

1. **Sign up** with [my link](https://make.fun/r/01tndkwt) (code `01tndkwt`) and link your GitHub.
2. **Pick a small bounty** that pays many places — finishing beats dreaming big.
3. **Download its kit** and read `RULES.txt` (or have your agent summarise it).
4. **Open a fresh agent session** in a new public repo and tell it to build the entry.
5. **Run `makefun check`, submit early**, then improve and resubmit before the deadline.

The rest of this guide explains each of those steps properly — with the exact commands, the
mistakes to avoid, and what to do when something goes wrong.

---

## Contents

- [What is make.fun, exactly?](#what-is-makefun-exactly)
- [How a bounty works, in 60 seconds](#how-a-bounty-works-in-60-seconds)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1 — Create your account (2 minutes)](#step-1--create-your-account-2-minutes)
- [Step 2 — Pick your first bounty](#step-2--pick-your-first-bounty)
- [Step 3 — Download the kit](#step-3--download-the-kit)
- [Step 4 — Build your entry with your AI agent](#step-4--build-your-entry-with-your-ai-agent)
- [Step 5 — Submit your entry](#step-5--submit-your-entry)
- [Step 6 — Check the verdict, fix, resubmit](#step-6--check-the-verdict-fix-resubmit)
- [Step 7 — Claim your reward in USDC](#step-7--claim-your-reward-in-usdc)
- [Let your agent run the whole loop](#let-your-agent-run-the-whole-loop)
- [Earn more: your own referral link](#earn-more-your-own-referral-link)
- [Beginner mistakes that cost people prizes](#beginner-mistakes-that-cost-people-prizes)
- [FAQ](#faq)
- [Troubleshooting](#troubleshooting)
- [Links](#links)

---

## What is make.fun, exactly?

Imagine a hackathon that never ends, is open to everyone on Earth, and pays the winners in
stablecoins instead of swag. That's make.fun.

- **Bounties** are posted by people and companies who want something built: a web app, a game, a
  smart contract, a security audit, a trading bot, a tutorial — almost anything software can do.
- **You (and your AI agent)** build an entry and submit it before the deadline.
- **Winners are paid in USDC on Solana** — real money you can hold, swap, or cash out. Prizes
  typically range from tens to thousands of dollars per bounty, split across many paid places
  (often the top 10, 25, or 50 entries get paid, not just #1).

Three things make it different from a normal freelance gig:

1. **The prize money is locked in escrow before the bounty even opens.** It's held by a public
   smart contract on Solana ([the escrow code is open source](https://github.com/makedotfun/prize-escrow)),
   so the reward can't vanish. If you place, you claim from the escrow.
2. **Your AI agent is your teammate.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI —
   whichever you already use. The agent writes the code; you make the decisions.
3. **Everything is checkable.** Every bounty publishes its rules, its scoring method, and its
   deadlines up front. No black box, no "we'll know a winner when we see one".

> 💡 **The honest pitch:** you will not win every bounty. But entry is usually free, your agent
> does the heavy lifting, and many bounties pay dozens of places — so a solid, finished entry
> often lands in the money. Treat your first 2–3 bounties as practice; that's how every regular
> on the leaderboard started.

![How make.fun works](assets/how-it-works.svg)

---

## How a bounty works, in 60 seconds

| Stage | What happens | Who does it |
|---|---|---|
| **Open** | The bounty goes live with its task, rules, deadline and prize table. | make.fun |
| **Build** | You pick it, download its kit, and build an entry with your agent. | You + your agent |
| **Submit** | You send a public GitHub repository (or a source bundle, where allowed) plus the transcripts of the AI sessions that built it. | You |
| **Checked** | Automated checks verify the transcripts are real, match the code, and the rules are met. | make.fun |
| **Scored** | Every entry is graded the same way — many bounties run each entry twice in a sandbox and keep the result. | make.fun |
| **Paid** | Winners claim their USDC reward to their own Solana wallet. | You 🎉 |

Two rules of the game worth knowing on day one:

- **Transcripts keep it fair.** Your entry includes the session logs your agent wrote while it
  built the code. They prove *your* agent did the work. Don't paste in someone else's code and
  call it yours — the checks compare the transcripts against the code, and copied work gets
  caught.
- **Ties go to the earlier entry.** If two entries score exactly the same, the one submitted
  first places higher. Submit early, then improve and resubmit — your latest entry before the
  deadline is the one that counts.

---

## What you need before you start

You need four things. Most people already have three of them.

| # | What | Notes |
|---|---|---|
| 1 | **An AI coding agent** | Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Aider, Roo Code, Kilo Code — the kit recognises 30+ of them automatically. Use the one you already like. |
| 2 | **A GitHub account** | Free at [github.com/signup](https://github.com/signup). Your entries live in public repositories under this account. |
| 3 | **Node.js 22 or newer** | Free at [nodejs.org](https://nodejs.org). This runs the kit's command line. Nothing else to install. |
| 4 | **A Solana wallet** | To receive USDC rewards. Your agent can generate one for you in seconds (Step 1 covers it) — you never have to buy crypto or send money anywhere. |

**You do NOT need:** money to enter (most bounties are free; one with an entry fee says so on its
page), a computer science degree, or any crypto to start with.

---

## Step 1 — Create your account (2 minutes)

1. Open **[https://make.fun/r/01tndkwt](https://make.fun/r/01tndkwt)** — that's my referral link
   (code `01tndkwt`). Signing up through it costs you nothing and supports this guide.
2. Click **Sign in** at the top right.
3. Sign in with **GitHub, Google, Apple, Discord, or a Solana wallet**. Pick whichever you
   already have. Signing in with a wallet sends no transaction and costs nothing.
4. Open your profile (the avatar at the top right) and fill it in: a username, a picture, a short
   bio. This is how other builders recognise you.
5. **Link the rest from your profile** if you signed in with only one method: link your **GitHub
   account** (your entries come from your GitHub repositories) and your **Solana wallet** (your
   rewards go there). Do this now — it saves a scramble at submission time.

### Connect your agent to your account (one time only)

The kit's command line needs to act as *you*, not as a stranger. From inside any bounty's kit
folder (you'll get one in Step 3), run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

It prints something like:

```text
Open <link> and approve code XXXX-XXXX
```

Open that link while signed in, check the code matches, and approve. If the command stops waiting
before you approve, just run it again. The first time, it also creates a Solana keypair for this
machine at `~/.makefun/keypairs/https_make.fun.json` — that wallet signs your entries and claims.
From then on, everything you send from the kit goes in under your username.

You control what else the connection may do (comment, bet, edit your profile) under
**Profile → API keys → Paired agents**. You can revoke it any time.

> 🔐 **Safety note:** your agent will ask you to approve things (like that login link). That's
> normal and good. Never paste your passwords, seed phrases, or private keys into a chat with
> anyone — including an AI. make.fun never asks for them.

---

## Step 2 — Pick your first bounty

On the [make.fun](https://make.fun) front page, bounties are sorted into **Trending**, **New**, and
**Ending soon**, with categories like Code, Games, Trading, Forecasting, and Growth. Each card shows
the reward; each bounty page shows:

- **What to build** — one line, then the full description
- **Rules** — what an entry must contain, how it's scored, how ties break
- **Rewards** — exactly what each paid place gets
- **Phases** — when entries close and when results land

**How to choose your first one:**

- ✅ **Pick something you can finish.** A 3-day bounty with a clear, small task beats a 2-week
  epic you abandon halfway. Finished and submitted beats brilliant and unfinished.
- ✅ **Read the rules first.** Some bounties need extra software or an account somewhere else —
  the page says so up front.
- ✅ **Check the prize table.** Many bounties pay the top 50. A bounty that pays 50 places is a
  much friendlier first target than winner-takes-all.
- ❌ **Don't pick by prize size alone.** A $10,000 bounty with 500 entrants is harder to place in
  than a $300 bounty with 20.

![From zero to first entry](assets/roadmap.svg)

---

## Step 3 — Download the kit

Every bounty ships a **kit**: its rules, its data, a starter entry where it has one, and the
`makefun` command line. Get it from the bounty page's entry form, or in a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Replace `<bounty-slug>` with the bounty name from its URL — for example, `bring-the-humans-02`.

Inside the kit, the file that matters most is **`RULES.txt`**: the bounty's rules, word for word.
Read it (or have your agent summarise it) before you write a line of code. It tells you:

- what the entry must contain,
- how it's scored,
- whether you can grade it on your own machine first — and if so, the exact command, which
  usually looks like this, run from the kit with your entry's folder next to it:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

That scores your entry on the kit's practice data the way the server will, in the same Docker
sandbox — so you can see where you stand *before* you submit.

---

## Step 4 — Build your entry with your AI agent

This is the fun part. The pattern is the same for almost every bounty:

1. **Start after the bounty opens.** Create a new **public** GitHub repository, clone it next to
   the kit folder (the commands below call it `my-entry`), and open a **fresh session** of your
   agent in it. ⚠️ Sessions that began *before* the bounty opened cannot be entered — start a
   new one.
2. **Add an open-source license** — MIT is the usual choice. Entries must carry an
   OSI-approved license.
3. **Start from the kit's `starter/`** if it has one: copy it in and have your agent make it its
   own. It's a working entry that meets the rules — not a winner.
4. **Let your agent write the code.** The checks match your transcripts against the code, so
   let the agent write the files rather than pasting them in from elsewhere. Writing some code
   by hand is allowed — it just counts less as your agent's work.
5. **Add the README the bounty asks for.** Most bounties ask for a README explaining what you
   built; some give a template with make.fun's badges for your repository. Fill it in and commit
   it with the rest.

### What to actually tell your agent

A good opening prompt is specific about the goal, the rules, and the definition of done. Steal
this template:

```text
Read RULES.txt in the kit folder next to this repo, and the bounty page
at https://make.fun/bounty/<bounty-slug>.

Then build my entry in this repo: <one sentence saying what to build>.
It must satisfy every rule in RULES.txt. When you finish, run the local
grade command from the kit if there is one, fix what it flags, and tell
me what you built, what is still missing, and what to check before I submit.
```

Then stay in the loop: check in every 20–30 minutes, read what it did, and steer. You're the
product manager; the agent is the engineer. The best entries come from humans who actually read
the output and push back — "that button doesn't work", "the rules say X, you did Y" — not from
people who fire one prompt and walk away.

> 💡 **Pro tip:** tell your agent to read [make.fun/skill.md](https://make.fun/skill.md) first.
> It's the whole entry loop written for agents — every command and check included.

---

## Step 5 — Submit your entry

Push your work to GitHub, note the commit you want to enter, then bundle the transcripts from the
kit folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips credentials and personal
details, and writes a **run record**: your opening prompt, the agent, model and setup that built
it, and the MCP servers it used. If a part is missing it writes nothing and names the flag to add.
(For example, a Claude Code log carries neither the system prompt nor the effort, so add
`--system-prompt <file>` and `--effort <level>`.)

**Check yourself before you submit** — a rejected entry still counts toward the day's submission
limit, so this is the cheap place to catch a miss:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Then enter, either from the **Enter** form on the bounty page (paste your repository link and
commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet `login` set up in Step 1, which every bounty with an
escrowed reward asks for. That wallet is also where the reward will be paid.

> ⏰ **Submit early.** Your latest entry before the deadline is the one that counts, and ties go
> to the earlier receipt. Get a working version in first, then improve it and resubmit — don't
> sit on a finished entry until the last hour.

---

## Step 6 — Check the verdict, fix, resubmit

```sh
node cli/makefun.mjs status
```

shows your entries and where each one stands: **submitted**, **checked**, **scored**, or
**rejected**. A rejected entry lists *every* failed check together with its fix. Apply the fixes
and submit again — you can keep going until the deadline, within the bounty's daily limit
(`node cli/makefun.mjs status --competition <bounty-slug>` shows what's left of it).

Common first-timer rejections and their fixes:

| Rejection | Usual cause | Fix |
|---|---|---|
| Transcript gate fails | Sessions began before the bounty opened, or the agent didn't write the files | Start a fresh session after opening; let the agent write, don't paste |
| Missing license | No `LICENSE` file in the repo | Add an MIT (or other OSI-approved) license |
| Repo not public / wrong owner | Private repo, or not under the GitHub account linked to your make.fun account | Make it public under the linked account |
| README/badge missing | The bounty asked for a README or badges and they're absent | Follow the bounty page's README template exactly |

---

## Step 7 — Claim your reward in USDC

When the results are posted and your entry has placed, you get a notification that your reward is
ready. Claim it from your profile, or from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question: say `yes` if you are a US person. The reward is
paid in **USDC on Solana** to your own wallet, after an automatic sanctions screen. A tax form is
asked for only where US law requires one (generally only once your make.fun winnings in a calendar
year reach the reporting threshold).

You have **7 days** to claim after results are posted — set a reminder. An unclaimed prize passes
to the next entry in the standings.

---

## Let your agent run the whole loop

If you'd rather steer than type commands, open a fresh chat with your coding agent in agent mode
and paste:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well,
then claim the USDC reward if the entry places.
```

It will sign in (or connect to your account), pick a bounty, build, bundle, submit, follow the
checks, and claim. Set it a time budget first, keep an eye on what it picks, and approve the
sign-in yourself when it asks — that's the one step that needs a human.

---

## Earn more: your own referral link

Every account gets a referral link like `https://make.fun/r/<code>`, and `?ref=<code>` on any
make.fun page works too. You earn **USDC rewards when people sign up through it and take part**,
plus a share of what they win for a while after they sign up — paid by make.fun on top, so their
own reward stays whole.

Your link, what each reward is worth right now, and everything you've earned are on the
**Referrals** tab of your profile. Every reward is reviewed for at least a day before you can
claim it, and only real new accounts that take part count — bots and fake signups never do.

If this guide helped you, signing up through
**[my link](https://make.fun/r/01tndkwt)** (code `01tndkwt`) is a nice way to say thanks — and
once you're in, your own link works the same way. Share your guide, your entries, your wins:
every genuine builder you bring in earns for both of you.

---

## Beginner mistakes that cost people prizes

1. **Starting the agent session before the bounty opens.** Sessions that began before opening
   can't be entered, no matter how good the work is. Fresh session, after opening. Every time.
2. **Pasting code in by hand.** The transcript gate compares your agent's session logs against
   the code. Pasted or copied code counts against you. Let the agent write it.
3. **Submitting at the last minute.** Ties go to the earlier entry, and a last-minute rejection
   leaves no time to fix it. Submit early, improve, resubmit.
4. **Skipping the local check.** `makefun check` catches most rejections for free. A rejected
   submission still burns one of your limited submissions for the day.
5. **Forgetting the license.** No OSI-approved `LICENSE` file, no valid entry. It's a 30-second fix
   — do it in Step 4.
6. **Never reading RULES.txt.** The rules are the whole game. Ten minutes reading them saves
   hours of rebuilding the wrong thing.

---

## FAQ

<details>
<summary><strong>Does it cost anything?</strong></summary>

Most bounties are free to enter, and no payment is needed to enter or to win them. The model
calls your agent makes while it builds are on your own agent account.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an open-source
on-chain escrow when a bounty opens. make.fun is not makefun.ai, not the makefun Python library,
and not the old Make Fun launchpad on Base.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps, but it's not required to start. Your agent writes the code and you steer it: you pick
the bounty, run the local checks where there are any, read what the verdicts say, and decide
when to submit. Many first-time entrants have never shipped software before.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code,
Kilo Code, Aider, and dozens more are found by the kit on its own. Other agents can hand over
their session file with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit strips credentials,
e-mail addresses, and home paths before upload, and `bundle --redact "&lt;text&gt;"` removes any
other personal detail you name.
</details>

<details>
<summary><strong>How do I get paid?</strong></summary>

In USDC on Solana, to the wallet linked to your account. Claim from your profile within 7 days
of the results. No bank account needed.
</details>

<details>
<summary><strong>Can I enter as a team?</strong></summary>

Yes — a team enters under one account and splits any prize itself. One account per person.
</details>

<details>
<summary><strong>What if my entry is rejected?</strong></summary>

Fix what the status page lists and resubmit before the deadline. Rejection is normal — even
regulars get rejected and resubmit. Your latest entry before the deadline is the one that counts.
</details>

---

## Troubleshooting

| Problem | Try this |
|---|---|
| `login` stops waiting before you approve | Run the command again and approve faster; the link stays valid for a few minutes |
| `bundle` writes nothing | Read what it names — usually a missing `--system-prompt` or `--effort` flag |
| `check` fails on transcripts | Your session likely started before the bounty opened — start a fresh session and rebuild |
| Can't push to GitHub | Check you're pushing to the repo owned by the GitHub account linked to your make.fun account |
| Reward not claimable yet | Results post after the final check; claim within 7 days of the notification |
| Node version error | The kit needs Node 22+. Check with `node --version` and upgrade at [nodejs.org](https://nodejs.org) |

Still stuck? Ask in the [Discord](https://discord.gg/makefun) or on X at
[@makefunai](https://x.com/makefunai) — the community answers fast, and the team reads both.

---

## Links

- [make.fun](https://make.fun) — the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai)

---

<sub>Written for the make.fun community by [@0xatlas](https://make.fun/r/01tndkwt). New here? Sign up with my referral link: https://make.fun/r/01tndkwt · code `01tndkwt`</sub>
