# BUILD_LOG — bring-the-humans-02 guide repo (@0xatlas)

Built: 2026-11-19 (WIB) by the guide-writing agent session for the
**bring-the-humans-02** bounty ("Bring the humans again", deadline **21 Nov 2026 17:30 WIB**,
$1,000 prize pool, top 50 entries paid).

> ⚠️ **This repo is NOT submitted yet, and cannot be submitted from here.**
> It is prepared content, ready to push the moment the owner completes the steps in
> "[Still needed from the account owner](#still-needed-from-the-account-owner)" below.

## What the guide is

`README.md` is an original, beginner-first getting-started tutorial for make.fun, written from
scratch in this session (draft, then a revision pass — it is not a copy of the kit's starter).
It takes a complete newcomer from zero to a first submitted entry and a claimed USDC reward:

- **Hook + 30-minute quick start** — the whole loop in 5 steps for impatient readers.
- **What make.fun is** — bounties, escrowed prizes in USDC on Solana, agents as teammates.
- **How a bounty works** — Open → Build → Submit → Checked → Scored → Paid, with the two rules
  that matter on day one (transcripts keep it fair; ties go to the earlier entry).
- **What you need** — agent, GitHub account, Node.js 22, Solana wallet; what you do *not* need.
- **Step 1 — Create your account** (via the referral link), link GitHub + wallet, connect the
  agent with `makefun login`.
- **Step 2 — Pick your first bounty** — how to choose (finishable, many paid places).
- **Step 3 — Download the kit** — `curl …/kit`, `RULES.txt`, `grade-local`.
- **Step 4 — Build with your agent** — fresh session after opening, MIT license, starter as a
  base, agent writes the code; includes a copy-paste opening prompt template.
- **Step 5 — Submit** — `bundle`, `check`, `submit` with exact commands.
- **Step 6 — Check, fix, resubmit** — `status`, common first-timer rejections table.
- **Step 7 — Claim your reward** — `claim`, 7-day window, tax-form note.
- **Agent autopilot** — the one-prompt "run the whole loop" option.
- **Your own referral link** — how referrals earn, and the call to sign up via this guide's link.
- **Beginner mistakes** (6), **FAQ** (8 questions), **Troubleshooting** table, **Links**.

Tone: direct, encouraging, honest about odds ("you will not win every bounty"), no jargon
without an explanation. Every command was checked against the kit's `RULES.txt` and
`starter/README.md` facts (login flow, bundle/check/submit/claim commands, escrow, transcript
gate, 7-day claim window).

## Referral link used

- Link: `https://make.fun/r/01tndkwt`
- Code: `01tndkwt` (appears as bare code, `/r/01tndkwt`, and `?ref=`-style link text in the README)

**Source of the code:** Donald's own referral link `https://make.fun/?ref=01tndkwt`, which he
gave on 2026-11-19 and instructed to use for make.fun registrations. It is used here as the
@0xatlas referral code — **the owner must verify it on the Referrals tab of the @0xatlas
make.fun profile before submitting** (see blockers). If the profile shows a different code,
replace `01tndkwt` everywhere in `README.md` (link + code) and re-commit.

## Repository structure

```text
make-fun-guide/                  (proposed repo name — see blockers)
├── README.md                    # the guide (entrypoint, ~24 KB, well under the 2 MB cap)
├── screenshot.png               # PLACEHOLDER mock of the GitHub repo page — MUST be replaced
│                                #   with a real screenshot after the repo is public on GitHub
├── LICENSE                      # MIT (OSI-approved, as required)
├── BUILD_LOG.md                 # this file (not part of the scored entry)
└── assets/
    ├── how-it-works.svg         # "How make.fun works" flow diagram (embedded in README)
    └── roadmap.svg              # "Zero to first entry" 5-step timeline (embedded in README)
```

- No `.github/README.md` exists (it would shadow the root README on GitHub and refuse the entry).
- Badge lines in `README.md` (required by the `repo_readme` check):
  - `https://make.fun/badge/bring-the-humans-02.svg`
  - `https://make.fun/badge/bring-the-humans-02/0xAtlas92/make-fun-guide/rank.svg`
  - `https://make.fun/badge/bring-the-humans-02/0xAtlas92/make-fun-guide/reward.svg`
  - all as live images (not in comments or code blocks), linking to the bounty page / leaderboard.
  - Owner `0xAtlas92` = the GitHub account linked to the make.fun account; repo name
    `make-fun-guide` = the proposed name — **if the owner creates the repo under a different
    name, update the two badge URLs to match before submitting.**
- `screenshot.png`: 1280×900 PNG, ~60 KB, 1,152,000 px (limits: ≤ 8 MB, ≤ 16,000,000 px).
  Its top shows the repository name and the start of the README, matching what the board/Feed
  crop shows. **It is a clearly-labelled placeholder drawn locally — the real screenshot must
  be taken of the published GitHub page and committed in its place before submitting.**
- After creating the repo on GitHub, the owner must also set the repo's **About**: website =
  the bounty page (`https://make.fun/bounty/bring-the-humans-02`) and topic `makefun`
  (the `repo_about` check).

## Verification done in this session

- [x] `README.md` names the referral code `01tndkwt` (bare, `/r/01tndkwt`, and full link).
- [x] `README.md` is ~24 KB (limit 2 MB), named exactly `README.md` at the repo root.
- [x] Three live make.fun badge lines present, not in comments/code blocks.
- [x] `LICENSE` is MIT (OSI-approved).
- [x] No `.github/README.md`.
- [x] `screenshot.png` is a valid PNG within size/pixel limits (placeholder — see above).
- [x] Guide re-read as a beginner: added the 30-minute quick start, fixed an HTML-entity leak
      in the FAQ code span, kept every step copy-pasteable with no assumed knowledge.
- [x] No secrets, credentials, API keys, private keys, seed phrases, passwords, or tokens
      anywhere in the repo or this log.

## Still needed from the account owner

These are the blockers — **nothing below can be done by the agent**; each needs Donald
(@0xatlas / GitHub `0xAtlas92`):

1. **Verify the referral code.** Open the @0xatlas make.fun profile → Referrals tab and confirm
   the code is `01tndkwt`. If it is different, tell the coordinator the correct code so the
   README can be updated and re-committed.
2. **Link GitHub on make.fun.** The @0xatlas make.fun profile must show GitHub `0xAtlas92`
   linked (sign in with GitHub, or link it on the profile). Without this, no repo can be entered.
3. **Create the public repo.** On GitHub as `0xAtlas92`, create public repo `make-fun-guide`
   (created after the competition opened, 2026-11-18T10:30:00Z — a new repo now satisfies this).
   If a different name is used, update the badge URLs in `README.md` to match.
4. **Push this content.** Push this repo's files to the new GitHub repo's default branch
   (local git remote is not yet set — the agent has no GitHub access and no token was used or asked for).
5. **Set the repo About on GitHub.** Website: `https://make.fun/bounty/bring-the-humans-02`;
   topic: `makefun`.
6. **Replace `screenshot.png`.** Once the repo is public, screenshot its GitHub page with the
   README showing (full page, normal scale, top showing repo name + README start), save as
   `screenshot.png` at the root, commit and push.
7. **Promote the referral link.** Share `https://make.fun/r/01tndkwt` (and the repo) — the score
   is the number of *verified human signups* through that link before the deadline
   (21 Nov 2026 17:30 WIB). Only real, active new accounts count; self-signups, same-network
   signups, idle/lurker accounts, and bots never count.
8. **Submit (coordinator's step).** Submit the public repo URL + commit with the agent session
   transcripts via the bounty page / kit (`makefun submit`), before the deadline. The entry's
   final re-check requires the repo to stay public, owned by the same GitHub account, with the
   referral code still in `README.md` on the default branch.

## Submission notes for the coordinator

- Entry type: referral/v1 guide — repo URL only; source bundles are not accepted for this bounty.
- Transcripts: this session's logs must be bundled (`makefun bundle`) and uploaded with the
  submission; the transcript gate requires the README to carry lines this agent wrote (it does —
  draft + revision in this session) and at least 5 assistant turns with text/thinking.
- Do NOT submit until blockers 1–6 above are done; a submission with a placeholder screenshot
  or a wrong referral code would be refused or unscored.
- Deadline: **21 Nov 2026 10:30 UTC / 17:30 WIB**. Final check runs 30 hours after that.
