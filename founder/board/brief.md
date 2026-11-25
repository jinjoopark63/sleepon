# Board brief: SLEEP:ON (스르르), version 4

Source: version 4 of a solo founder's 1st-round business plan for a Korean government startup program (Nov 2026), plus research done since the last board meeting: a competitor scan, simulated buyer panels, a pricing analysis, an offer redesign and a CFO model. Everything below is either the founder's plan or a computed/researched result, labelled as such. Nothing has been verified by real customers yet.

## The idea (plan v4)

- **What it is:** a Korean sleep-sound app. It synthesizes the night's sleep sound on-device and fades it out at the point the user usually falls asleep, learned not from clock time but as "minutes after the phone is put down", so it works when bedtime changes every day or the user sleeps in the daytime. If the user stirs in the night it resumes the sound quietly from where it stopped (phone-motion detection; the first 3 nights only log "we would have resumed here" without playing; it can be switched off or replaced by a lock-screen button). A heart-rate armband (Polar-type BLE, iOS and Android) is the later stage to do this in real time; tested in 2027 with pass criteria (onset detection delay ≤5 min, ≤1 wrong restart/night, 100% fallback), shipped in Pro in year 2 only if it passes. No own hardware.
- **First customer (changed in v4):** Korean adults in their 20s-30s whose bedtime is irregular (rotating/night shift workers, frequent overtime, freelancers) who often take 30+ min to fall asleep and already play sleep sounds. Previously the target was all 20s-30s with sleep difficulty.
- **Offer:** free tier = 3 basic sounds + 30/60-min sleep timer. Pro = learned fade-out, resume-on-stir, smart wake (with a watch), reports. **14-day comparison trial with no automatic charge**: nights alternate between a plain 30-min timer and SLEEP:ON; on day 14 the app shows side by side the time to fall asleep and the time to fall back asleep after waking, measured from phone put-down time and motion (watch data if available; morning check-in optional). If there is no difference it says "the free version suits you". After paying: if records do not improve within 30 days, refund help (Android direct refund; iPhone via Apple's refund request screen, Apple decides).
- **Price:** Pro KRW 4,900/month or 39,000/year (VAT included). December 2026 landing-page test: 39,000 vs 49,000/year.
- **Institutions (year 2+):** KRW 2,000 per person per month for shift-work sites (hospitals, logistics centres) and dorms.

## Evidence so far

**Real data (founder's survey, Nov 2026, n=100):** 39% take 30+ min to fall asleep; 71% want "fades when asleep, resumes when awake"; 51% would try a 2-week trial; 11% would pay KRW 6,900/month (16% among 20s-30s); 48% say a fair monthly price is under KRW 5,000; 35% refuse to pay at all; 76% use Android. Only 5 shift workers answered. 16 respondents who have trouble sleeping and already use ASMR/music: 94% want the feature.

**Competitor scan (public sources, Nov 2026; app-store pages could not be opened directly, figures come from search snapshots and need checking):**
- "Stop sound when you fall asleep" already exists: Apple AirPods on iOS 26 ("Pause Media When Falling Asleep", free, Apple earbuds only, pause only), Sleep Cycle (auto fade in accelerometer mode), Pillow, Apple Watch utilities (Zlpy, Sleep When I Sleep). Asleep (Korean sleep-tech firm) sells mic-based "stop the service when the user falls asleep" as an SDK. Samsung has a leaked, not shipped, Galaxy Buds "pause media while you're asleep" setting.
- No app or platform found with evidence of **resuming the sound when the user wakes**, or of **learning a personal sleep-onset time**.
- Korean competitors: Renight (AI-generated beats, KRW 77,000/yr, ~4.4K ratings, heavy marketing), 슬립루틴 (66,000/yr), 마보 (47,000/yr), 코끼리 (35,000-45,000/yr). Median annual price of 9 paid apps: KRW 47,000. SLEEP:ON's 39,000 is near the lowest.
- The most common complaint across Calm, Endel, BetterSleep, Sleep Cycle: unwanted charges after trials or cancellation.
- Insomnia patients in Korea: 797,862 in 2025 (HIRA). No national count of shift workers or of the narrowed segment was looked up yet; the plan still quotes 3.12M adults with difficulty falling asleep (2009 study).

**Simulated buyer panels (AI sub-agents, 20 per run, same seed; simulated buyers lean agreeable, treat as upper bounds, not evidence of real demand):**

| run | target | offer | would buy |
|---|---|---|---|
| 1 | all 20s-30s | earlier offer (feature-based, auto-billing-free trial) | 0/20 |
| 2 | all 20s-30s | comparison trial + phone measurement | 2/20 |
| 3 | all 20s-30s | auto-resume off by default, smaller free tier | 0/20 |
| 4 | irregular-schedule 20s-30s | current offer | 7/20 (35%) |

In run 4, all 7 buyers cited "learns minutes after the phone is put down, not clock time" and all chose the monthly plan "to check for one more month". Of the 13 who passed, 8 said free YouTube is enough, 4 did not trust that a phone by the bed can tell when they fell asleep. Price answers in run 4 (median, KRW/month): bargain 2,500, getting expensive 5,200, too expensive 8,450 (vs 1,900 / 3,900 / 6,900 for the broad group).

## Numbers (CFO model v2; 2028 = first year with staff; VAT-excluded)

- Assumptions: half monthly (4,900), half annual (39,000) → average KRW 3,705/subscriber-month; store fee 15%; refund allowance 5%. Contribution KRW 2,964 per subscriber-month (80%).
- Fixed costs 2028 (founder's stated salaries): 3 staff at KRW 3M/month + founder 2M + ~10% employer insurance + ads at 2027 level + tools ≈ KRW 13.4M/month.
- Break-even: **4,531 paying subscribers/month** (individual only). Plan targets: 300 (end 2027), 3,696 (end 2028), 8,683 (end 2029). Margin at 8,683: 38%.
- 2028 result: about −KRW 85M with no institution revenue; −50M if institution seats ramp from 0 to 3,000; −20M if institution revenue arrives in full as planned. Loan repayment of KRW 20M is extra. The 2027 budget (KRW 50M) does not cover 2028.
- Levers computed: hiring 2 staff in 2028 instead of 3 → break-even 3,417, 2028 result −45M; annual price 49,000 → break-even 4,111; both → break-even 3,100, 2028 result −38M (before institutions).
- Sensitivities: at 2.1% trial-to-paid (industry median) instead of 3%, margin at plan drops to 20%. The model assumes monthly subscribers stay all year; real monthly churn is higher.
- Plan v4 text now says "2028 near break-even including institutions, profit from 2029", and hires development and operations first, sales when subscribers near ~3,400.

## Timeline and validation (plan v4)
Dec 2026: 10 interviews (shift workers, overtime office workers), KRW 100k ad + pre-order test (39,000 vs 49,000), institution meetings (decision-maker, budget, paid seats). Jan 2027 technical check: wearable wake signal and armband real-time signal; all-night playback with screen off and battery; fallback to basic mode; bedtime auto-start; **agreement between phone-measured sleep/wake times and watch records**. Feb first version, Apr pilot (100 users, 4-week crossover: timer vs SLEEP:ON), Jun free launch, H2 paid. Targets 2027: 10k downloads, 300 paid.

## Constraints
Solo founder (robotics/IT major, built the web MVP). Wellness app, not a medical device; health data processed on-device. Year-1 budget KRW 50M; KRW 20M of it is a loan not yet approved.
