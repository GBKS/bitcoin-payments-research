# Contributing

Thanks for helping. This is a small, experimental research notebook, so the process is light, but the content rules are strict: git history is public and permanent.

## Good places to start

- **Claims to verify.** Each item in the "To verify" list in [TODO.md](TODO.md) has its own [issue labeled `to verify`](https://github.com/GBKS/bitcoin-payments-research/issues?q=is%3Aopen+label%3A%22to+verify%22). These are the best first contributions, by hand or with an agent.
- **Help wanted.** Items marked **help wanted** in [TODO.md](TODO.md): non-English sources, research partners, studies we've missed.
- **Corrections.** If something is wrong or out of date, open an issue or a pull request with a source.

Before starting on an issue, comment on it to claim it, so two people (or two agents) don't do the same work.

## Content rules

The full rules are in [CLAUDE.md](CLAUDE.md) and [Method](01-method.md). The short version:

1. **Neutral research.** Compare kinds of product; don't recommend one.
2. **Public sources only.** Nothing from private conversations.
3. **Label what isn't verified,** inline: *[from memory]*, *[assumption]*, *[to verify]*. Anything unlabeled links to a source you actually opened.
4. **Say versus do.** Note where what people say differs from what they do.
5. **Privacy.** Anonymize individuals and small community accounts, even when their pages are public. No minors.
6. **Dates.** Update "Last updated" on any page you edit.

## Pull requests

- **One item per pull request,** linked to its issue.
- **Sources with quotes.** For every source you add, give the link and a short quote (at most about 25 words) that supports or contradicts the claim. Reviewers check the quote against the source.
- **Smallest change that works.** Change only the lines the item needs.
- **"Couldn't settle it" is a fine result.** Comment on the issue with what you found instead of forcing a verdict.
- **Say if an agent helped.** That's welcome; it just tells reviewers what to look for.

## Contributing with an agent

Coding agents (Claude Code, Codex, Cursor and others) can do this work. Fork the repo, open your agent in a clone of your fork with web access, and give it this prompt:

> You're helping with github.com/GBKS/bitcoin-payments-research, a public research notebook. Work in my fork of it.
>
> 1. Before changing anything, read `CONTRIBUTING.md`, `CLAUDE.md`, `01-method.md` and `TODO.md`. Follow their content rules exactly: public sources only, label anything unverified, anonymize individuals, no minors, update "Last updated" on any page you edit.
> 2. Pick **one** open issue labeled `to verify` that nobody has claimed in the comments and that no open pull request covers. Tell me which one before you start, and remind me to comment on the issue to claim it.
> 3. Find public sources for it and open every source you use. For each, note the URL and a quote of at most 25 words that supports or contradicts the claim.
> 4. Change only the lines needed. If the sources confirm the claim, add the link and remove the label. If they contradict it, correct the claim. If you can't settle it, change nothing and tell me why.
> 5. Don't open a pull request yourself. Show me the diff and the sources so I can check them. If I approve, open one pull request that links the issue, lists the sources and quotes, and says an agent helped.

You stay responsible for what your agent submits: please check its sources before approving. How agents might do more of this research over time is described in [Auto-research](90-auto-research.md).

## License

By contributing, you agree that your contributions are licensed under [CC BY 4.0](LICENSE), like the rest of the content.
