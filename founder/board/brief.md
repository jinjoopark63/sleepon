# Board brief: SLEEP:ON (스르르), plan version 6 (founder's own edit)

Source: the founder's latest 1st-round business plan for a Korean government startup program (Nov 26, 2026), edited by the founder after earlier board rounds, plus research done earlier (competitor scan, simulated buyer panels, a CFO model). Everything below is either the founder's plan text or a computed/researched result, labelled as such. No real customer has paid yet.

## The idea (plan v6, as written by the founder)

- **What it is:** a Korean sleep-sound app. It synthesizes the night's sleep sound on-device. Core idea in the plan: "learn when I fall asleep, and when I wake, resume from where the sound cut off; the goal is to do this without a button using heart rate."
- **Three tiers:**
  1. **Basic mode (smartphone only, free):** learns "usual time to fall asleep" from a morning check-in and fades out then; if you wake, one button press restarts the sound. Auto-restart at the moment of waking is a Pro feature.
  2. **Wearable (Pro):** Apple Watch via Health app corrects the cut-off time each morning; smart wake via the watch app's smart-alarm session (max 30 min before alarm). Galaxy Watch (Health Connect) in year 2.
  3. **Heart-rate armband (target, Pro):** real-time HR/motion over standard Bluetooth (iOS and Android) to stop at sleep onset and restart automatically on waking. Tested in 2027 with 30 research armbands; pass criteria: onset detection delay ≤5 min average, wrong restarts on ≤10% of nights, 100% fallback to basic mode on disconnect. If it passes, armband support ships in Pro in year 2 via a commercial armband with a public SDK; no own hardware.
- **Customer (plan v6):** adults who often take 30+ min to fall asleep but would not see a doctor; first customers are people who have trouble falling asleep and already play sleep sounds; meeting 20s-30s first. (An earlier draft narrowed the first segment to irregular-schedule workers such as shift workers; v6 removed that narrowing.)
- **Revenue model (plan v6):** basic mode free; Pro bundles auto-restart on waking (wearable/armband), smart wake and an effect report; "resume after waking" (wanted by 71% in the survey) is positioned as Pro's core. Pro KRW 4,900/month or 39,000/year (VAT incl.); 14-day trial, at the end the app shows how much sleep-onset time dropped, then the user pays. Institutional licences (KRW 2,000/person/month) from year 2 for shift-work sites and dorms.
- **Differentiation (plan v6):** AirPods (iOS 26) pause media when you fall asleep on Apple earbuds; Sleep Cycle fades sound; neither restarts. SLEEP:ON aims to learn sleep onset and fade out on speakers and Android too, and restart from where it cut off on waking.
- **Moat statement added in v6:** accumulate per-person records of "what counts as awake" and corrected sleep-onset timing.

## Evidence

**Founder's survey (Nov 2026, n=100):** 39% take 30+ min to fall asleep; 71% want "fades when asleep, resumes when awake"; 51% would try a 2-week trial; 11% would pay KRW 6,900/month (16% among 20s-30s); 48% say a fair price is under KRW 5,000; 35% refuse to pay; 76% use Android. Only 5 shift workers answered. 16 respondents with sleep trouble who already use ASMR/music: 94% want it, 88% would try.

**Market (plan):** 3.12M adults 20-69 with difficulty falling asleep 2+ times/week (2009 study); insomnia patients 769k in 2024 (the plan quotes 2024; HIRA reported 797,862 for 2025). Separate research (not in v6): about 1.8M Korean wage workers do shift work (22.5M × 8.0%, 2023 working-conditions survey), an estimated 0.3-0.58M with sleep problems; figures from search snippets, unverified.

**Competitor scan (Nov 2026, public sources, store pages not opened directly):** "stop when you fall asleep" exists (AirPods iOS 26, Sleep Cycle accelerometer fade, Pillow, Apple Watch utilities; Asleep sells mic-based auto-stop as an SDK; Samsung has a leaked, unshipped Galaxy Buds setting). No app found with evidence of resuming on waking or learning a personal onset time. Korean competitors: Renight (KRW 77,000/yr), 슬립루틴 (66,000), 마보 (47,000), 코끼리 (35,000-45,000); median of 9 paid apps KRW 47,000/yr. Top complaint across Calm/Endel/BetterSleep/Sleep Cycle: unwanted charges after trials. Research on phone-only sleep timing: error ~24-38 min vs diaries/watches; phone-motion apps detect wake poorly vs PSG.

**Simulated buyer panels (AI sub-agents, 20 each, upper bounds only):**
- Broad 20s-30s, an offer close to v6 (free basic mode with morning check-in and button resume; Pro = wearable features, report, smart alarm; trial without auto-charge): **0/20**. Main reasons: free YouTube + timer is enough (8), the report is self-reported so not proof (6), resume still needs grabbing the phone and auto needs a 2028 armband bought separately (7 mentioned).
- Broad 20s-30s with a 14-day alternating comparison trial and phone-based measurement: 2/20; a variant with auto-resume off by default: 0/20.
- Irregular-schedule 20s-30s (shift/overtime/freelance) with comparison trial and "learns minutes after phone is put down": **7/20**; all 7 cited the schedule-independent learning.
- Price answers (broad group, median KRW/month): bargain 1,900, getting expensive 3,900, too expensive 6,900.

## Numbers (CFO model v2.1, 2028 = first year with staff, VAT-excluded)
- Half monthly (4,900) / half annual (39,000) → avg KRW 3,705/subscriber-month; store fee 15%, refund allowance 5%, RevenueCat 1% → contribution KRW 2,923 (79%).
- Fixed costs 2028 with 2 staff (KRW 3M each) + founder 2M + ~10% insurance + ads + tools + bookkeeping ≈ KRW 10.3M/month.
- Break-even 3,516 paying subscribers/month; plan targets 300 (end 2027), 3,696 (end 2028), 8,683 (end 2029).
- 2028 operating result: −KRW 48M without institutions; about +17M if institution revenue arrives in full (as plan v6 states); loan repayment KRW 20M extra. Cash needed incl. 2027 budget ~KRW 99M. Margin at 8,683 subscribers: 47%.
- At 2.1% trial-to-paid instead of 3% the margin at plan falls sharply; the model assumes monthly subscribers stay all year.
- Max affordable install cost given value per subscriber and 3% conversion: roughly KRW 360-1,070, vs the plan's quoted iOS cost per install of USD 9.11 (~KRW 12,750).

## Timeline (plan v6)
Dec 2026: 10 interviews, KRW 100k ad + pre-order test (39,000 vs 49,000/yr), institution meetings. Jan 2027 technical check incl. "phone-estimated sleep onset vs watch, median nightly difference ≤30 min; if not met, show the effect comparison to watch users first". Feb first version, Apr pilot (100 users, 4-week crossover timer vs SLEEP:ON; 30 armband users), Jun free launch, H2 paid. Year-1 budget KRW 50M (grant 20M, loan 20M not yet approved, own 10M). Solo founder. Wellness app, data on-device.
