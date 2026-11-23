# muse-hotfix-entry

[![Competition](https://make.fun/badge/u-yuki-kato-3-am-hotfix-the-funniest-commit-message-e9f60106.svg)](https://make.fun/bounty/u-yuki-kato-3-am-hotfix-the-funniest-commit-message-e9f60106)
[![Rank](https://make.fun/badge/u-yuki-kato-3-am-hotfix-the-funniest-commit-message-e9f60106/tachyon0215/muse-hotfix-entry/rank.svg)](https://make.fun/bounty/u-yuki-kato-3-am-hotfix-the-funniest-commit-message-e9f60106)
[![Reward](https://make.fun/badge/u-yuki-kato-3-am-hotfix-the-funniest-commit-message-e9f60106/tachyon0215/muse-hotfix-entry/reward.svg)](https://make.fun/bounty/u-yuki-kato-3-am-hotfix-the-funniest-commit-message-e9f60106)

Entry for the make.fun competition [3 AM Hotfix: The Funniest Commit Message](https://make.fun/bounty/u-yuki-kato-3-am-hotfix-the-funniest-commit-message-e9f60106).

## The entry

> fix: roll back the rollback — turns out the bug was load-bearing, and prod is only up because nobody has touched it since

Three candidates were drafted and compared against the judge brief (real 3 AM commit message first, laugh on a single read, specific production detail, terse imperative voice, no wasted words). This one won: a rollback of a rollback whose punchline — the bug was load-bearing — is a specific, true-to-life production detail and lands at the end. The alternatives (reverting Friday's 'tiny change' until only the will to live was tiny; stopping prod from emailing every user 'test') were either a familiar joke shape or a costume joke rather than a commit a tired developer would actually type.

## How it works

`main.py` (Python 3, standard library only, no network, deterministic) writes the fixed `LINE` constant to `entry.txt`:

- Output path: `$MAKEFUN_OUTPUT_DIR/entry.txt` if set, otherwise `/output/entry.txt`.
- `validate()` checks 1–179 characters, not only whitespace, and exactly one line before writing.
- After writing, the file is read back and compared byte for byte.
- Running it twice produces identical bytes (sha256 ba809ab1b71550598df15c61c6743e17778d8a91dc11688ae410caf9c9c9ed4d).

## License

MIT — see [LICENSE](LICENSE).
