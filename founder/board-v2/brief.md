# Board brief: SLEEP:ON (스르르), version 2

Source: version 2 of the founder's 1st-round business plan (revised after outside feedback) for a Korean government startup program ("2026년 2차 모두의 창업 프로젝트", 1R), Nov 2026. Solo founder (robotics/IT major, built the web MVP in Python, a paying Calm user). Everything below is what the founder claims; nothing has been independently verified.

## The idea

- What it is: a sleep-sound app. Instead of a sound that just plays all night (or stops on a fixed timer), the app synthesizes "tonight's" sleep sound on-device and adjusts it to the user's sleep: fades/stops when the user falls asleep, restarts when they wake, and wakes them gently in light sleep.
- Who it is for: adults who often take 30+ min to fall asleep but would not go to a clinic. First customers: 20s-30s who already use sleep sounds (late sleep onset: 82% of 20s, 70% of 30s per a sleep-tech company report).
- Price: basic mode (smartphone only) free. Pro subscription KRW 4,900/month or KRW 39,000/year, 14-day trial (wearable connection, morning report, smart alarm). From year 2: institution licences (dorms, shift-work sites) at KRW 2,000 per person per month.
- Where and how: Korea, iOS + Android (76% of survey respondents use Android). Organic acquisition (ASO, 20 short-form videos, share cards, dev-log channel), KRW 100k ad test in Dec 2026 to measure real install cost. Later: affiliate (creators, bedding brands, welfare malls), then institutions. Overseas (English/Japanese) from year 4.

## How it works (three tiers)

1. Basic (phone only): learns "your usual time to fall asleep" from a morning check-in, fades out then; one button to restart if you wake. Auto-starts at bedtime via iOS sleep schedule/Shortcuts. 10-second pre-sleep check-in picks the sound.
2. Wearable (e.g. Apple Watch via Health app): corrects the cut-off time each morning using actual sleep-onset time; for a light-sleep wake, uses the watch app's smart-alarm extended runtime session (official Apple feature, HR/motion, max 30 min before alarm). Apple's Health overnight sleep record is NOT available in real time (Apple developer forum answer). Galaxy Watch (Health Connect) in year 2.
3. Target: a heart-rate armband (e.g. Polar Verity Sense, BLE real-time HR) to detect the actual moment of falling asleep / waking and stop/restart in real time. This is the claimed main differentiator. Because it uses the standard Bluetooth heart-rate profile it works on both iOS and Android (survey: 76% Android, 67% among 20s-30s). To be tested in 2027 with 30 research armbands against morning logs and small-scale polysomnography, with pass criteria: sleep-onset detection delay ≤5 min on average, ≤1 wrong restart per night, 100% fallback to basic mode on disconnect. If it passes, armband support ships in Pro in year 2 via a commercial armband with a public SDK; if not, launch with basic + wearable modes and re-test the armband. No own hardware: a dedicated sleep band only considered in year 3 via partnership with a band maker if demand is shown.

Evidence the founder cites: one RCT of real-time sleep-state-matched sound (EEG headband) cut sleep onset ~10.5 min (Bressler 2024); HR falls around sleep onset; wrist PPG+motion classify 4 sleep stages at 76.4% (Wulterkens 2021); consumer devices detect wake only 18-54% (Chinoy 2021) — founder plans to change sound only when confident. All-night noise has weak evidence and one 2026 study saw reduced REM with all-night pink noise. Music for insomnia: moderate-quality evidence (Cochrane 2022). AI-personalized music for sleep: very low evidence.

Simulation on a public Apple Watch dataset (Walch 2019, 31 people): with a 30-min timer, 26/31 had sound running 10+ min after falling asleep, and 64 of 67 wake-ups happened after the sound had already stopped. The SLEEP:ON line applies the target rules to the public records before any sensor test (the plan now labels it as a simulation). The '2-minute' wake threshold is an initial setting to be tuned from pilot reports of wrong restarts/discomfort.

## Done so far
- Web MVP (basic mode + replay of real sleep records vs timer approach), QR demo.
- 6 synthesized sounds (rain, waves, slow chords) generated on-device, no audio files. Melodic AI music planned via a Korean AI-music company (inquiry email sent) or Mubert API ($199/mo).
- Demand survey, Nov 2026, n=100 (55 in 20s-30s, 35 40+, 10 teens, 5 shift workers): 39% take 30+ min to fall asleep; 37% have trouble 3+ days/week; 71% want "fades when asleep, resumes when awake"; 51% would try a 2-week trial. Willing to pay KRW 6,900/month: 11% overall, 16% among 20s-30s. Sub-segment: 16 respondents who have trouble falling asleep AND already use ASMR/music: 94% want the feature, 88% would try a 2-week trial (n=16). 48% say a fair price is under KRW 5,000/month. 35% refuse to pay at all.

## Market and competitors (founder's figures)
- Korea: 3.12M adults 20-69 have trouble falling asleep 2+ times/week (8.6%, Cho 2009 survey). Insomnia patients 769k in 2024, rising 4 years running. "Market" = 3.12M x KRW 39,000 = ~KRW 120B; year-3 target is 0.3% of that.
- Sleep Cycle (global): 768k paying subscribers, 26.6% operating margin (2025). Renight (Korea, sleep-sound app): ARR > KRW 1B (Jun 2024), 2M cumulative downloads, KRW 7,700/mo or 77,000/yr.
- Others: Sleep Cycle (annual only, KRW 45,900/yr), SleepHack (adjusts beats to sleep stage via wearable, KRW 14,000/mo), DreamTune AI (English only, KRW 8,800/mo). Samsung's 2026 AI air conditioner adjusts airflow by Galaxy Watch sleep stage. Founder notes Sleep Cycle and Samsung are moving toward sleep-adaptive control.

## Financial plan (founder's own estimates, before 15% store fee)

| | 2027 | 2028 | 2029 |
|---|---|---|---|
| New downloads | 30k | 120k | 250k |
| Paid subscribers | 900 | 3,888 | 8,744 |
| Individual revenue | KRW 35M | 152M | 341M |
| Institutions | 3 pilots (free) | 10 sites / 3,000 people | 30 sites / 9,000 people |
| Institution revenue | - | 72M | 216M |
| Total revenue | KRW 35M | 224M | 557M |

Formula: paid = new downloads x 3% + prior-year subs x 32% renewal; revenue = subs x 39,000 (annual price applied to all). Institution sensitivity (founder): at 100 seats per site instead of 300, year-3 revenue would be ~KRW 410M (individual 341M + institutions 72M); in December the founder will meet institutions to confirm the decision-maker, budget and number of paid seats. Median 35-day paid conversion for freemium apps is 2.1% (RevenueCat 2026); at 2.1% year-3 revenue would be ~KRW 450M. 1-year retention benchmark: 36% cheap apps, 23% expensive. Day-7 retention app average 13% (Adjust); targets: 40% in pilot, 20% after launch. iOS cost per install USD 9.11 (Singular 2025). 3-year cumulative 400k downloads = 1/5 of Renight's 2M.

Year-1 spend KRW 50M: dev environment/devices/servers 6.3M; pilot & user research 10M (incl. 100-person 4-week crossover pilot); trademark/terms/design 4.5M; AI music service 3.4M; 30 research armbands 5.5M; sleep-centre PSG validation & advisors 9.3M; content & ads 11M. Outsourced dev KRW 0. Hiring: 3 people (dev, sales, ops) in year 2, 1 data analyst in year 3. Founder says 2028 subscription revenue will exceed costs and the loan will be repaid from subscriptions. If the loan falls through, armband/validation scope shrinks.

## Timeline
Dec 2026: 10 interviews (incl. shift workers), KRW 100k ad test. Jan 2027: technical validation (wearable wake signal, armband real-time signal, all-night playback with screen off / battery, fallback to basic mode, auto-start). Feb 2027: first app version. Apr 2027: pilot (gates: 60% morning check-in response, 40% day-7 use). Jun 2027: free launch (gate: 1,000 users, 20% day-7). H2 2027: paid (gate: 30k downloads, 900 paid). Planned validation, split in two: (1) 100 pilot users (basic mode; watch owners use wearable mode), 4 weeks, 2 weeks timer vs 2 weeks SLEEP:ON in random order, comparing sleep-onset time, return-to-sleep, refreshment, ISI; (2) 30 armband users with the pass criteria above.

## Constraints and risks the founder names
- Regulatory: run as a wellness app, not a medical device (MFDS wellness criteria, 2026 revision); sensitive health data under separate consent, processed on-device, institutions get anonymous stats only.
- Risk 1, misjudging sleep/wake → act only when confident, compare app judgments with morning logs every 2 weeks.
- Risk 2, ad cost → recruit first users from survey contacts and institution pilots.
- Risk 3, solo-dev delays → core features only; outsource anything that fails the Jan 2027 check.
- Moat claim: accumulating data on "which sound fit which state"; trademark and patent filing under review.

## Separately computed unit economics (founder-cfo run on the original numbers, Nov 2026)
These are calculations from the plan's inputs plus the founder's stated salaries; they are not in the plan document.
- Korean App Store prices include 10% VAT, and the 15% store fee applies to the VAT-excluded price, so a KRW 39,000/yr subscriber nets ~KRW 30,136/yr (the plan's revenue table is before VAT and store fees).
- Founder's stated 2028 costs: 3 hires at KRW 3M/month each + founder KRW 2M/month; with ~10% employer insurance, ads at 2027 level and tools, fixed costs are ~KRW 13.4M/month.
- Break-even on individual subscriptions alone: ~5,347 paying subscribers per month. The plan's 2028 year-end target is 3,888.
- 2028 cash result (annual fees received up front): roughly -KRW 50M with no institution revenue, about +KRW 16M if institution revenue arrives in full as planned, before repaying the KRW 20M loan. The plan still states "subscription revenue will exceed costs from 2028" and "2027 is roughly break-even including the grant".
- The year-1 content/ad budget (KRW 11M) buys roughly 860 installs at the plan's own USD 9.11 cost per install; the 2027 target remains 30k downloads.
