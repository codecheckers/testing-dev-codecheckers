# testing-dev-codecheckers

The testing counterpart of
[`codecheckers/codecheckers`](https://github.com/codecheckers/codecheckers),
for developing the register bot
[chekhov](https://github.com/codecheckers/chekhov) against.

**Every row here is invented.** The names, handles, ORCIDs and contacts are
placeholders, the ORCIDs are not real identifiers, and the fediverse addresses
and e-mails point at `example.invalid`, which cannot resolve. Nothing in this
repository describes a person.

The lists mirror the real ones column for column, because the bot reads them by
header:

| File | Columns |
|---|---|
| `codecheckers.csv` | `name,handle,ORCID,contact,fields,languages,ecr_until,ecr_checked,fediverse` |
| `institutional-codecheckers.csv` | `name,handle,ORCID,institution,fediverse` |
| `agile-codecheckers.csv` | `name,handle,ORCID,fediverse` |

Development and testing run against this repository and never against the real
one. `config/settings-development.yml` in chekhov is the single place that
names it.

## What is deliberately absent

`registration-runbook.md`, `annual-maintenance.md` and `not-a-bot.md` are not
copied. They are prose for people rather than data for the bot, and a stale
copy of a runbook is worse than no copy: read them in the real repository.
