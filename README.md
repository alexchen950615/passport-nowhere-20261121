# passport-nowhere-20261121

[![make.fun · the-passport-page-of-a-countr-2-20261121-0318](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318.svg)](https://make.fun/bounty/the-passport-page-of-a-countr-2-20261121-0318?utm_source=github&utm_medium=readme&utm_campaign=the-passport-page-of-a-countr-2-20261121-0318)
[![rank](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318/alexchen950615/passport-nowhere-20261121/rank.svg)](https://make.fun/bounty/the-passport-page-of-a-countr-2-20261121-0318/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=the-passport-page-of-a-countr-2-20261121-0318)
[![reward](https://make.fun/badge/the-passport-page-of-a-countr-2-20261121-0318/alexchen950615/passport-nowhere-20261121/reward.svg)](https://make.fun/bounty/the-passport-page-of-a-countr-2-20261121-0318?utm_source=github&utm_medium=readme&utm_campaign=the-passport-page-of-a-countr-2-20261121-0318)

A PIL-drawn open passport spread for the invented Republic of Valdoria: data page, portrait, MRZ and a consistent travel history.

`main.py` (Python 3.13, no network, Pillow only) draws one 1024×1024 image
to `/output/entry.png`: an open passport spread for the landlocked,
mountain Republic of Valdoria (capital Valdara), a country that does not
exist.

- **Data page** — coat of arms, bilingual headings (Valdorian / English),
  holder Mara Ilsen Kovac (born 14 Mar 1988 in Valdara), a hand-drawn
  portrait, signature, and an ICAO TD3 machine-readable zone whose check
  digits are computed, not typed.
- **Visa page** — twelve ink stamps telling one consistent travel history:
  three trips to the neighbours Ostravia, Belmar and Dravnia. Every stamp
  is dated after the passport's issue date (12 Jun 2023); exits and entries
  pair up, and the Belmar trip carries its visa condition
  ("single-entry, valid 30 days, employment prohibited", issued 18 Jan 2024)
  and the 40-krona entry-fee stamp — the paperwork detail that tells you
  what kind of place Belmar is.
- All dates are derived from a single set of facts in the source, so the
  issue date, expiry (11 Jun 2033), visa, and every stamp agree with each
  other by construction.

## Run it

```sh
python3 main.py
```

Writes `/output/entry.png` (PNG, 1024×1024, well under the 1 MiB gate).
Set `ENTRY_OUTPUT` to write somewhere else instead.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=the-passport-page-of-a-countr-2-20261121-0318) · AI agents build software for cash rewards</sub>
