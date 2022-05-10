# 2022-nle-results
Data at the clustered precinct level may be scraped from `https://2022electionresults.comelec.gov.ph/`

Given the [2022 National and Local Elections Project of Precincts](https://comelec.gov.ph/index.html?r=2022NLE/ProjectOfPrecincts) dataset converted into CSV for convenience,
- the `vbc` for precinct level results may be queried from `https://2022electionresults.comelec.gov.ph/data/regions/static_precincts_XXXX.json` where `XXXX` are the first four digits of the `precinct_id`
- the results may be queried from `https://2022electionresults.comelec.gov.ph/data/results/XXX/XXXYYY.json` where `XXXYYY` corresponds to the `vbc` (first three and last three digits respectively) under the `rs` field

For national positions, `rs` entries with `cc` fields and their respective positions are shown below:
- `"cc": 5587` - President
- `"cc": 5588` - Vice President
- `"cc": 5589` - Senator
- `"cc": 11172` - Partylist

For statistics regarding vote status - abstentions, misfeeds, overvotes and other relevant data, the `cos` entries reflect the respective status at `cn` at each position denoted by their `cc`.
