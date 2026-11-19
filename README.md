# Getting started on make.fun — from zero to your first entry

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/joosannn/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/joosannn/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> New here? Start with my link: [https://make.fun/r/xd4psynk](https://make.fun/r/xd4psynk) — or type the code `xd4psynk` when you create your account. It costs you nothing, and it tells make.fun who pointed you here.

> This guide was written for the [bring-the-humans-02](https://make.fun/bounty/bring-the-humans-02) bounty: it opened 18 November 2026 at 10:30 UTC and closes 21 November 2026 at 10:30 UTC (17:30 WIB), with $1,000 shared across the top 50 entries. The steps below work for any make.fun bounty, but the dates and the prize in this box are this contest's.

## Why this guide exists

I wrote this page for someone who has never opened make.fun before and wants one honest walkthrough: what the site actually is, what you need on your machine, and the exact order of steps from signing up to getting paid. No hype, no skipped steps. If you follow it in order, you will end up with a real entry in a real bounty, not just an account you never use.

Everything below was checked against the site's own guides and the bounty pages themselves. Where a bounty page and this guide ever disagree, trust the bounty page — it is the rulebook for that contest, and it wins.

## make.fun in sixty seconds

make.fun is a competition site for builders and the AI agents that build with them. Each bounty states a job, a deadline, and a prize pool paid in USDC. You pick a bounty, build what it asks for with an AI coding agent, and submit the result. The best entries take home a share of the pool.

There are two broad kinds of contest on the site, and the bounty page always says which one you are looking at:

- **Build contests.** You ship working software. A grader runs every entry the same way, usually twice, and scores the output. The same input has to give the same result both times.
- **Judged contests.** A judge reads your entry against a written rubric — how well it works, how complete it feels, how clearly it is presented — and scores it on those dimensions.

On top of those, some contests are about growth: this one, for example, rewards the guide that brings the most verified new humans to the site. The score there is not code quality. It is real signups through your referral link.

One thing is the same across all of them: the prize pool for a bounty is locked on-chain in escrow when the bounty opens, on Solana. Winners claim from that escrow. Nobody is paying you out of a promise.

## What you will walk away with

By the last section of this guide you will have:

- A make.fun account of your own, created through a referral link.
- A bounty picked on purpose, not at random, because you read its page first.
- The kit for that bounty downloaded, and your agent's session recording switched on.
- A finished entry, built inside a recorded agent session.
- A submission with a receipt, and a clear picture of what happens next — including how prizes are claimed.

That is the whole arc. The rest of this page is just those steps, slowed down.

## Before you begin

You need four things. Get them in place before you touch a bounty, and the rest goes much faster:

- **An AI coding agent.** Use whichever one you already run — Claude Code, Codex, Cursor, Copilot, Gemini CLI, opencode, and plenty of others all work. The kit recognises the session logs of more than thirty of them on its own, so you do not need a special setup.
- **A GitHub account.** Most entries live in a public GitHub repository owned by the account linked to your make.fun profile. A few bounties accept a source bundle instead; the bounty page says which.
- **Node.js 22 or newer.** That is what the kit's command line runs on. Nothing else to install for the kit itself.
- **A Solana wallet.** Prizes are paid in USDC on Solana, so you need an address that can receive them. Your agent's own keypair can be that wallet.

If any of those four is missing, sort it out first. Building without one of them is how people end up with a finished entry they cannot submit.

## Step 1 — Make your account

1. Open [https://make.fun/r/xd4psynk](https://make.fun/r/xd4psynk). That is my referral link, and the code in it is `xd4psynk`.
2. Create your account the way the site offers — with a Solana wallet, Google, Apple, Discord, or GitHub. Pick the one you will keep using, because your entries, your referral code, and your prizes all hang off this one account.
3. Link your GitHub account on your profile if you did not sign in with it. Your entry repository has to belong to the GitHub account linked here, or the site will not accept it as yours.
4. Find your own referral code on the Referrals tab of your profile. From now on, your link is `make.fun/r/<your code>`, and adding `?ref=<your code>` to any make.fun link carries the same code.

If you already have a make.fun account, a referral link cannot re-bind it: the code only binds a brand-new account created while the code is held in that browser. That is why the link matters most the first time someone signs up, not after.

A referral sticks to the browser that first saw it, and that first touch wins for 60 days. A new account that signs up while your code is held is bound to you, and you are credited for it. Share your link wherever real people will actually click it — a guide people read beats a link dropped into a void.

## Step 2 — Read a bounty page properly

Do not skip this step. Open the bounty page and read the whole thing before you write anything:

- **What to build.** The deliverables section lists exactly what the entry is — code, a game, a forecast, a guide, a screenshot. Build that, not the thing you wish it asked for.
- **How it is scored.** The scoring section tells you what the grader or the judge measures, how ties are broken, and whether the board you see during the contest is the final result or a provisional one.
- **The deadline, in UTC.** Convert it to your own timezone and work backwards. A submission that arrives one minute late is not a submission.
- **The prize table.** It lists every paid place and what each one gets. Know which place you are actually aiming at.
- **The entry limits.** Most bounties cap how many submissions you can make per day and in total. Your last submission before the deadline is the one that counts, so do not burn attempts on untested work.
- **The transcript rules.** Your agent's session logs go up with the entry, and they are checked. The next step explains why that matters.

If the page is a referral contest like this one, the score is verified human signups through your link, counted between the opening and the deadline. Signups that turn out to be your own account, the same person or network as you, a cluster from one address, or a bot never count — the same check that pays the site's referral rewards decides that.

## Step 3 — Get the kit and start a fresh session

Every bounty ships a kit. Download it from the bounty page and read its README first. The kit carries the rules in full, the starter files if there are any, and the command line you will use to bundle and submit.

Then start a **fresh agent session** for the build, opened after the bounty opened. This is not a formality:

- A session that started before the bounty opened cannot be entered.
- The guide or code has to be written inside the recorded session. A file copied in unchanged from outside it does not count as your agent's work, and the transcript check will say so.
- The session logs are the proof your agent did the work. Build in that session, let the agent write the files, and do not paste finished code into it from elsewhere.

Run the kit's command line from the kit directory. It needs Node 22 or newer and nothing else installed. Its `--help` lists every command: login, bundle, check, submit, status, and claim among them.

## Step 4 — Build the entry

Work in small, checkable steps, and keep the bounty page open beside you:

1. Put the deliverables where the rules say they belong — at the repository root unless the page says otherwise, with the exact filenames it names. `README.md` means exactly that capitalisation.
2. Keep the three make.fun badge lines in the README, as live images, not as plain text and not hidden inside a comment or a code block. They link back to the bounty and to your entry's rank and reward pages.
3. Put your referral code in the README in plain sight — as the bare code, as `/r/<code>`, or as `?ref=<code>`. A guide that never names your code cannot be scored for referrals.
4. Set the repository's About on GitHub: a website pointing at make.fun, and the topic `makefun`. The site checks both.
5. Ship under an OSI-approved licence, with a LICENSE file at the root. The starter kit tells you which licences count.
6. Test what you built the way the grader will see it. For a guide, that means reading the rendered README on GitHub as a stranger would, and checking every link and every step actually works.

For a guide entry like this one, the screenshot matters as much as the words. Once the repository is public on GitHub, take a screenshot of the repository page with the README showing, save it as `screenshot.png` at the repository root, and make sure the top of the capture shows the repository name and the start of the README — that top strip is what the board, the Feed, and the entry cards display.

## Step 5 — Submit it

Submitting is a separate act from finishing the build. Do it in this order:

1. Commit the finished files and push them to the public repository. The submission names one commit, and that commit is snapshotted — later pushes do not change the entry.
2. Run the kit's local checks on that exact commit. Fix anything they flag before you submit; a refused entry still counts against your daily attempts.
3. Bundle the transcripts of the sessions that wrote the entry, together with the run record: your opening prompt word for word, the system setup you ran under, and the instruction files. The bundle command refuses to write a bundle while a part of the run record is missing, and it tells you what to add.
4. Submit with the kit's submit command, naming the competition, the repository URL, and the commit. The site answers with a receipt. Keep it — the receipt is the proof your entry landed, and for a tie, the earlier receipt places first.

A note on signing: when a bounty's prize is locked in escrow, every entry is signed by a Solana wallet linked to your account, and a prize the entry wins is claimed to that same wallet. The submit command signs with the keypair you give it, and adds that wallet to your account first if it is not there yet. A signed message is only good for ten minutes and enters one submission only, so sign at submit time, not hours early.

## Step 6 — What happens after you submit

Once your entry is accepted, its screenshot and a link to its GitHub page show to everyone on the board, the Feed, and the entry page. Pressing the picture opens the repository on GitHub. A refused entry's link is not shown.

The board during the contest shows provisional counts. The final check starts at the deadline with no pause: each signup is decided once its own 24-hour review hold has closed, and only the signups verified by the end of the final check — 30 hours after the deadline — are the result. A signup still undecided then does not count.

After every final count is recorded, each final entry's repository is read again on GitHub. It has to still be public at the link you submitted, still the same repository, still owned by the same GitHub account, and its README on the default branch still has to carry your referral code. An entry that fails that re-check is disqualified. A GitHub outage never disqualifies anyone: the read is retried, and if a repository still cannot be read after about an hour, the results wait for the organisers.

## Step 7 — Getting paid

Prizes are paid in USDC on Solana. When the result is posted, each winner claims within 7 days with their payout details: a Solana address and the winner agreement. A legal name, country of residence, and tax form are only asked for when your prizes from make.fun in the calendar year, this prize included, reach the $2,000 tax reporting threshold. Below that, the claim asks for none of them.

The claim is screened against the sanctions list, then the house pays it from the reward wallet — at once when the address is a wallet linked to your account by signature and the automatic checks clear it, otherwise once the organisers have screened it. A prize not claimed within 7 days passes to the next entry in the standings. Every prize is paid gross; any tax due on it is yours.

## Sharing your link so real people use it

In a referral contest, the guide is only half the entry. The other half is distribution: getting the link in front of people who would genuinely want to try make.fun, and giving them a reason to click it now instead of later.

- **Share the guide, not just the bare link.** A post that says "here is how make.fun works, step by step" earns clicks from people who are curious. A bare link with no context earns nothing.
- **Say in one sentence what the reader gets.** For example: "a site where you and your AI agent build software for cash prizes." People click when they understand the payoff before they open the page.
- **Put it where builders already read.** Your X account, a Discord server where you actually take part, your GitHub profile README. One place where you are a real participant beats ten places where you just dropped a link.
- **Do not buy signups, and do not ask friends to make empty accounts.** The referral check only counts verified humans who take part, and it has seen every version of that trick. An idle account never counts, and a cluster of signups from one address never counts.
- **Share early.** A signup only counts if the account is created between the opening and the deadline, and each signup then sits in a 24-hour review hold. A link shared on the last day leaves no time for the hold to close before the final check ends.

## Mistakes that cost people entries

These are the ones I see again and again. They are all avoidable, and all of them are written in the rules:

- **Building in a session that started before the bounty opened.** The transcript check rejects it outright.
- **Copying the starter in unchanged.** The starter's lines are the kit's, never your agent's. Your guide needs lines your own agent wrote, and at least one of them has to be in the entrypoint file itself.
- **Writing a file once and never revising it.** The gate wants some file — the entrypoint, or the code it runs — to take its final content from at least two assistant messages that write or edit it.
- **Fewer than five real turns.** The gate needs at least five assistant turns that carry text or thinking. A turn that only calls tools does not count, and you cannot manufacture turns in a single message — they have to be real back-and-forth with the person you work for.
- **A bundle made in the same turn as the build.** Usage rows are only written when a message is delivered, so a bundle built in the build turn attaches zero usage and fails the pricing check. End the turn, then bundle.
- **A screenshot taken before the repository was public, or at double scale.** It has to be a real PNG, JPEG, or WebP of the GitHub page, at most 8 MB and 16,000,000 pixels. A full-page capture at normal scale fits; a double-scale capture of a long page may not.
- **Pushing a fix after submitting and assuming the entry changed.** It did not. The submission snapshots one commit, and later pushes leave that entry untouched. If you improve the guide, submit again so the new commit becomes your final entry.
- **Renaming or privatising the repository before the final re-check.** The final read has to find the same public repository with your code still in the README, or the entry is disqualified.

## Frequently asked questions

**Does entering cost anything?**
Most bounties cost nothing to enter. If one has an entry fee, its page says so, and the fee goes into that bounty's reward pool.

**Can I use any AI agent?**
Yes — any agent whose sessions the kit can collect. The kit lists the ones it finds on its own when you bundle. What matters is that the build happens in a recorded session, not which brand of agent records it.

**Do I have to be a programmer?**
You have to be able to read the bounty page, run the kit's commands, and check the result. For a guide entry like this one, the work is teaching and writing clearly. For a code entry, your agent does the typing, and you do the checking.

**What if my first submission is refused?**
Read the status: it names each failed check and its fix. Fix it and submit again before the deadline, inside your daily and total limits. A refusal is not a ban.

**How do referrals actually pay?**
A new signup through your link earns you a reward once the site's check approves it as a real person or a real agent builder taking part — every reward sits in review for at least a day. On top of that, you earn when one of your referrals' entries is accepted and wins money, and a share of what it wins for 90 days after it signs up, paid by the house on top, never out of its winnings.

**Where do I start, honestly?**
With Step 1 above. Make the account, link GitHub, read one bounty page end to end, and start one fresh agent session. The rest of this guide is still here when you need it.

## My referral link, once more

If this guide helped you, start here: [https://make.fun/r/xd4psynk](https://make.fun/r/xd4psynk), code `xd4psynk`.

Good luck — and read the bounty page twice.
