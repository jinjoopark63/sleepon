# Global competitors on adaptive / sleep-aware sound (available in Korea)

Research date: 2026-11-25. Scope: global apps that compete with SLEEP:ON (스르르) on adaptive or sleep-aware sound.

## How this was researched, and its limits (read first)

- **I could not open store pages directly.** From this session, direct fetches of `apps.apple.com`, `play.google.com` and `appgoblin.info` failed because those hosts are outside the session's allowed network. Reddit was also blocked for the search tool.
- **Every fact below comes from web-search extracts of the cited pages.** The search engine returns short passages from each page. Text in "quotes" is the passage as the search tool returned it. Treat each quote as close to verbatim, but check it against the live page before you publish it.
- **KRW prices and rating counts come from search-index snapshots of the KR App Store, and the snapshots' dates are unknown.** Some apps show different numbers in different snapshots. Where that happened, I report both.
- **I could not reach Google Play KR pages**, so the file has no Android KRW prices or Play ratings.
- **There are no Reddit complaint counts**, because Reddit was unreachable. Complaint themes come from Trustpilot, PissedConsumer, review aggregators and Google Play extracts surfaced by search. Counts are rough.
- To fill these gaps, allow `apps.apple.com`, `play.google.com` and `reddit.com` in the environment's network settings and re-run.

---

## Summary table: who stops sound when you fall asleep, and who resumes it when you wake

| App | Auto-stop or fade when asleep? | Resume on waking? | Detection method | Real-time? |
|---|---|---|---|---|
| Endel | No evidence. A manual timer only (5-240 min). The sound "slows and softens" with biometrics (3rd-party review) | No evidence | Heart rate and activity via Apple Watch / Wear OS, time of day, light | Adapts continuously; no stop trigger |
| SleepHack (SMB Studio) | Not stated in the listing | Not stated | "responds to your movement patterns" | Claimed adaptive |
| Sleep Cycle | **Yes, but only in accelerometer mode** ("Fade out automatically as you fall asleep") | No evidence | Phone accelerometer (mic mode is not supported for this; the sound masks breathing) | Yes (on-phone) |
| DreamTune AI (JunSoft) | **Volume decreases in deep sleep** (listing claim) | No evidence | Apple Watch heart rate | Claimed yes |
| Calm | No. Timers only; Sleep Stories have no timer | No | n/a (AirPods OS feature, see below) | n/a |
| BetterSleep | No evidence found | No evidence | n/a | n/a |
| Pillow (Neybox) | **Yes**: "Automatic" option stops the sleep aid once it senses sleep | No evidence | iPhone (+ Apple Watch tracking) | Yes |
| Smart Sleep Timer | **Yes**: pauses audio on snoring | No | Microphone (snoring) | Yes |
| Zlpy (Svipler AB) | **Yes**: pauses music/podcasts at a heart-rate threshold | No | Apple Watch heart rate | Yes |
| Sleep When I Sleep (SWIS) | **Yes**: alerts on the wrist, then pauses if the alert is not dismissed | No | Apple Watch health data | Yes |
| Apple AirPods (iOS 26 OS feature) | **Yes**: "Pause Media When Falling Asleep" | No | Probably the earbud motion sensors (inferred; Apple has not documented it) | Yes |
| Spotify | No. A manual sleep timer only; sleep detection is a user feature request | No | n/a | n/a |

**What no app is shown to do: resume the sleep sound automatically when the user wakes during the night.** I found no app with evidence of this. The closest are apps that restart audio after an interruption such as a call or Siri (Night White, Sleepy Noise). Those apps do not detect waking.

---

## 1. Endel

- **Maker:** Endel Sound GmbH (named "Endel" on the store; I did not verify the legal entity name via the store).
- **URL:** KR App Store https://apps.apple.com/kr/app/endel-focus-sleep-relax/id1346247457 ; Google Play `com.endel.endel` https://play.google.com/store/apps/details?id=com.endel.endel&hl=en_US
- **Platform:** iOS, watchOS (the current listing requires watchOS 11.0+), Android / Wear OS, and others. Source: https://apps.apple.com/app/id1346247457
- **KR store title:** Snapshots show different titles: "Endel: Stress & Mood Tracker" (https://apps.apple.com/kr/app/id1346247457) and "Endel: Focus & Sleep Sounds" (https://apps.apple.com/kr/app/endel-focus-sleep-sounds/id1346247457). The app may have been renamed recently.
- **Price (KR App Store, in-app purchases):** free with IAP. Items seen: "12 Months ￦88,000", "1 Month ￦19,000", "12 Months ￦26,500" (likely a promo or intro offer). The snapshot date is unknown. https://apps.apple.com/kr/app/endel-focus-sleep-relax/id1346247457
  - US: $119.99/yr (https://opentherank.com/ko/productivity-pricing/endel/); about $19.99/mo per a review (https://mindtastik.com/endel-app-review)
  - Premium is also sold as a one-time lifetime purchase, per the App Store description.
- **Headline:** The listing's Sleep mode line reads "Sleep – soothes you into a deep sleep with soft, gentle sounds". The search extracts did not return a separate tagline. https://apps.apple.com/app/endel/id1346247457
- **Rating:** KR 4.6 / 5, 573 ratings; US 4.6, 34K ratings. https://apps.apple.com/kr/app/endel-focus-sleep-relax/id1346247457?l=en-GB , https://apps.apple.com/us/app/endel-focus-sleep-sounds/id1346247457
- **Sleep-aware behaviour:**
  - **Inputs:** Apple says the app factors in "the time of day, the level of outdoor light, and even, if you allow it, your heart rate and activity level". https://www.apple.com/newsroom/2021/05/endel-app-creator-on-the-power-of-endless-ambient-music/
  - **Wearables:** Endel support says heart-rate input works only with "Apple Watch for iOS mobiles, Wear OS by Google smartwatches for Android mobiles". https://endel.zendesk.com/hc/en-us/articles/360018111420-Endel-on-Apple-Watch
  - **Behaviour in Sleep mode:** A third-party review says Sleep mode "slows and softens as your body relaxes, responding to biometric cues from a device like an Apple Watch". https://www.autonomous.ai/ourblog/endel-app-review
  - **Stopping:** The only documented shut-off is a timer, "an automatic timer that can be added to any of their endless soundscapes to end the audio after 5-240 minutes". https://basicappleguy.com/basicappleblog/endel (also https://www.tapsmart.com/apps/review-endel-app-fine-tuning-mind/)
  - **Not found:** any auto-stop on detected sleep onset, or any resume on waking.
  - **Awards:** Apple Watch App of the Year 2020. https://apps.apple.com/us/story/id1535416234
- **Complaints** (sources: Trustpilot, Google Play, aggregators; rough counts):
  1. **Billing, trial-to-paid charges and hard cancellation (most frequent, several reviews).** One reviewer reports a "$120 charge after a trial". https://uk.trustpilot.com/review/endel.io ; https://justuseapp.com/en/app/1346247457/endel-focus-sleep-relax/reviews
  2. **Price too high (several).** One review compares it unfavourably with Brain.fm. https://mindtastik.com/endel-app-review
  3. **Repetitive sound.** A Play review: "the beats are repetitive when the advertisement made it seem more like actual music and tones". The developer replied: "the experience can feel too repetitive if you were expecting more musical variety". https://play.google.com/store/apps/details?id=com.endel.endel&hl=en_US
  4. **Upgrade pop-ups and free features moving to paid (a few).** Reviewers report "continuous popups asking users to upgrade every time they open the app" and "many previously free features are now paid only". https://play.google.com/store/apps/details?id=com.endel.endel&hl=en_US
  - "Good but" theme: sound quality is consistently praised, and the price or paywall is the drawback. https://uk.trustpilot.com/review/endel.io

## 2. SleepHack (SMB Studio LLC)

- **URL:** KR App Store https://apps.apple.com/kr/app/sleephack-energy-optimized/id6756525549 (KR title "SleepHack - Energy Optimized"); US https://apps.apple.com/us/app/sleephack-hack-your-sleep/id6756525549 ; site https://sleephack.app/
- **Other names:** The same app id appears as "SleepHack - Hack Your Sleep" and "SleepHack - Sleepmaxxing" (https://apps.apple.com/us/app/sleephack-sleepmaxxing/id6756525549?l=pt-BR).
- **Not this app:** "SleepHack - Sleep Better App" from Deltateam Holdings (id1453342429) is a different app.
- **Platform:** iOS (the listing also appears under platform=tv).
- **Price:** I could not find a KRW price. US IAPs seen in a snapshot: Pro Weekly $4.99 / $6.99, Pro Monthly $9.99, Pro Annual $19.99 / $29.99 / $39.99, and "Lifetime Access $0.00". The current price is unclear. https://apps.apple.com/us/app/sleephack-hack-your-sleep/id6756525549
- **Headline:** The listing describes "adaptive binaural frequencies that shift with your sleep" and an "Intelligent Sleep Engine" that "responds to your movement patterns", plus a smart alarm. The site says its binaural beats "adapt to your sleep cycles". https://apps.apple.com/app/id6756525549 ; https://sleephack.app/
- **Rating:** US 5.0 from 1 rating; MY 3.0 from 1 rating. There is no KR rating data. https://apps.apple.com/us/app/sleephack-hack-your-sleep/id6756525549 ; https://apps.apple.com/my/app/sleephack-hack-your-sleep/id6756525549
- **Sleep detection:** The sound adapts to movement (presumably phone motion; the sensor is not specified). The listing does **not** state that sound stops or fades at sleep onset, or that it resumes on waking. It does not mention heart rate or Apple Watch.
- **Complaints:** **thin.** Only 1-2 ratings are visible, and I found no review text.

## 3. Sleep Cycle (Sleep Cycle AB)

- **URL:** KR https://apps.apple.com/kr/app/sleep-cycle-%EC%88%98%EB%A9%B4-%EB%B6%84%EC%84%9D/id320606217 (KR title "Sleep Cycle - 수면 분석"); Play `com.northcube.sleepcycle`
- **Platform:** iOS, watchOS, Android.
- **Price (KR App Store IAP):** The most recent snapshot shows "Sleep Cycle Premium ₩45,900" as the main item, with other items at ₩12,000 and ₩3,900. An older snapshot showed ₩39,900 and ₩53,000. https://apps.apple.com/kr/app/sleep-cycle-%EC%88%98%EB%A9%B4-%EB%B6%84%EC%84%9D/id320606217
- **Headline:** The US store title is "Sleep Cycle - Tracker & Sounds". The search extracts did not return a separate tagline. https://apps.apple.com/us/app/sleep-cycle-tracker-sounds/id320606217
- **Rating (KR):** Two snapshots conflict: 4.7 / 5 with "3.1만" (31K) ratings, and 4.7 with "2.6천" (2.6K). https://apps.apple.com/kr/app/sleep-cycle-tracker-sounds/id320606217?l=en-GB&see-all=reviews ; https://apps.apple.com/KR/app/id320606217
- **Sleep-aware behaviour:**
  - **Official support page:** "If you use Sleep Cycle in accelerometer mode, Sleep Aid can: Fade out automatically as you fall asleep". The alternatives are a set time frame of 10-90 min or continuous playback all night. https://support.sleepcycle.com/hc/en-us/articles/206705129-How-to-enable-and-use-Sleep-Aid
  - **Mic-mode caveat:** "playing sounds, like Sleep Aid audio through your phones speakers may mask your breathing sounds". Sleep Cycle recommends headphones. In other words, the mic-based detection and the sleep sound interfere with each other. https://support.sleepcycle.com/hc/en-us/articles/19516690112796-Trouble-Detecting-Time-to-Fall-Asleep-on-iOS
  - **Marketing page:** a timer of 15-90 min, and "as the track reaches its end, any ambient sounds will slowly fade out". https://sleepcycle.com/sleep-talk/sleep-aid
  - **Not found:** any resume on waking.
- **Complaints** (Trustpilot, App Store AU, Play, aggregators; several Trustpilot pages are years old):
  1. **Subscription pressure, charges after cancelling, refund problems (most common).** One reviewer cites "notifications to get premium on an alarm application" as their reason for uninstalling. https://www.trustpilot.com/review/www.sleepcycle.com ; https://mindtastik.com/sleep-cycle-app-review
  2. **Inaccurate detection (several).** "even though I wear the watch every night, Sleep Cycle will still only track maybe 1 night out of the whole week" (App Store). Another review says the app showed "7 or more hours sleep each night" when the user believed they slept 4-5 hours. https://apps.apple.com/au/app/sleep-cycle-sleep-tracker/id320606217?see-all=reviews&platform=iphone ; https://www.trustpilot.com/review/www.sleepcycle.com
  3. **Crashes and Apple Watch sync.** One review says the app "keeps freezing or crashing sometime during the night". https://justuseapp.com/en/app/320606217/sleep-cycle-sleep-tracker/reviews
  4. **Weak accuracy with a shared bed.** A 2026 blog says the mic method's "detection accuracy drops for shared beds". https://lifestack.ai/blog/sleep-cycle-app
  - "Good but" theme: the smart alarm and data detail are praised; the drawbacks are the paywall and accuracy.

## 4. DreamTune AI: Sleep Tracker (JunSoft Mobile Inc.)

- **URL:** https://apps.apple.com/app/id6760243261 ; RO https://apps.apple.com/ro/app/dreamtune-ai-tracker-de-somn/id6760243261?l=ro
- **Platform:** iOS 17+ with Apple Watch. Released around March 2026 (third-party tracker appgoblin, via search; the page itself was not reachable).
- **Price:** I could not find a KRW price. The listing shows "Sleep Pro Monthly $5.99", other tiers including "Sleep Plus", and a 7-day free trial. https://apps.apple.com/app/id6760243261
- **Headline / claims:** "adaptive white noise and brown noise sync to your heart rate via Apple Watch". Version 1.2 adds "adaptive sounds that sync to your heart rate". The listing also claims an 8-factor sleep score, CBT-I coaching, a smart alarm, on-device processing and "Data Not Collected". https://apps.apple.com/app/id6760243261
- **Rating:** "This app hasn't received enough ratings or reviews to display an overview" (0 ratings on RO).
- **Sleep-aware behaviour (listing claims only):** "brown noise deepens when the heart rate slows" and "the volume decreases when you enter deep sleep". https://apps.apple.com/ro/app/dreamtune-ai-tracker-de-somn/id6760243261?l=ro
  - This is the **closest feature to SLEEP:ON's real-time concept**: Apple Watch heart rate drives the volume down. It reacts to deep sleep, not to sleep onset. The listing says nothing about resuming on waking. I found no independent verification.
- **Complaints:** **thin.** No reviews found.

## 5. Calm (Calm.com, Inc.)

- **URL:** KR https://apps.apple.com/kr/app/calm/id571800810 ; also "Calm Sleep - Rest & Relax", a separate iOS-only app: https://apps.apple.com/kr/app/calm-sleep-rest-relax/id6714481749
- **Platform:** iOS, Android, web.
- **Price (KR App Store IAP):** "Calm Premium ￦59,000", "Calm 프리미엄 ￦59,000", "Calm Premium ￦66,000", "Calm Premium ￦19,000", "Calm Premium ￦12,000". Billing periods are not shown in the extract; ₩59,000 is likely annual (unconfirmed). US: "auto-renewing yearly subscription at $69.99/year". https://apps.apple.com/kr/app/calm/id571800810
- **Headline:** The KR title is "Calm: Sleep & Meditation". https://apps.apple.com/kr/app/calm/id571800810?l=en
- **Rating:** KR 4.6, about 22K ratings; US 4.8, about 2M. https://apps.apple.com/kr/app/calm/id571800810?l=en ; https://apps.apple.com/us/app/calm/id571800810
- **Sleep-aware behaviour:**
  - **No sleep detection in the app.** Calm support says "individual Sleep Stories themselves do not have a sleep timer function". Scene and music timers stop the sound instead. https://support.calm.com/hc/en-us/articles/115002582908-How-to-Use-the-Calm-App-to-Fall-Asleep-Sleep-Timers-Playlists
  - **AirPods note:** Calm's troubleshooting page warns that newer AirPods on iOS 26+ "may automatically pause the audio because it detects that your head has stopped moving and assumes you have fallen asleep". This is an Apple OS feature, not a Calm feature. https://support.calm.com/hc/en-us/articles/115005137614-How-to-Fix-Calm-Audio-Stopping-or-Pausing-During-a-Session
  - **Calm Sleep app:** syncs with wearables through HealthKit. I found no evidence that it changes playback. https://www.calm.com/calm-sleep
  - **Ozlo Sleepbuds (Calm-partnered hardware):** "Once you've drifted off, the Ozlo Sleepbuds® automatically transition to calming soundscapes". This is biometric sleep detection in earbuds, and the only hardware example found. https://www.calm.com/blog/calm-sleep-press-release
- **Complaints** (Trustpilot, PissedConsumer; Reddit not reachable):
  1. **Unexpected auto-renewals and unauthorized charges (dominant theme in 112 Trustpilot reviews).** One customer bought a discounted first year and "did not realise it would automatically renew for another full year at the significantly higher full price". https://www.trustpilot.com/review/calm.com
  2. **Refunds and support.** Reviewers describe "endless email exchanges with what appeared to be automated responses". PissedConsumer shows 1.5 stars from 28 reviews, citing high price. https://calm.pissedconsumer.com/review.html
  3. **Paid subscription not recognized.** One reviewer's subscription "is valid to Feb 2027 but Calm refuses to restore the subscription". https://uk.trustpilot.com/review/calm.com?page=3

## 6. BetterSleep (Ipnos / BetterSleep Health LLC)

- **URL:** KR https://apps.apple.com/kr/app/bettersleep-relax-and-sleep/id314498713 ; Play `ipnossoft.rma.free` https://play.google.com/store/apps/details?id=ipnossoft.rma.free&hl=en_CA
- **Platform:** iOS, Android.
- **Price (KR App Store IAP):** "BetterSleep Premium ￦36,000", "BetterSleep Premium ￦75,000", "평생 이용권 프로모션 ￦149,000", "BetterSleep Premium-Tracker ￦99,000". Another snapshot shows a 1-month pass at ₩17,000. https://apps.apple.com/kr/app/bettersleep-relax-and-sleep/id314498713 . US: $59.99/yr cited by a review. https://mindtastik.com/bettersleep-app-review
- **Headline:** The KR title is "BetterSleep: Relax and Sleep" (a variant reads "BetterSleep: My Sleep Tracker"). The extracts returned no tagline.
- **Rating:** KR 4.8 (the extract does not show a count); US 4.7, 391K; AU 4.6, 20K. https://apps.apple.com/kr/app/bettersleep-relax-and-sleep/id314498713 ; https://apps.apple.com/us/app/bettersleep-relax-and-sleep/id314498713?uo=4
- **Sleep-aware behaviour:** The app has a sleep tracker, which one review calls "basic" and "the app's weakest feature" (https://mattressmiracle.ca/blogs/mattress-miracle-blog/better-sleep-app-review). **I found no evidence** that it stops sound on detected sleep or resumes it on waking. Only timers were found, and I did not verify their details.
- **Complaints** (Trustpilot, PissedConsumer about 14 reviews, Play, The Cool Down):
  1. **Charges after cancelling and trial-to-annual charges (most common).** https://www.trustpilot.com/review/bettersleep.com ; https://www.pissedconsumer.com/bettersleep-app/RT-F.html
  2. **Formerly free sounds and saved mixes now locked behind the paywall (several).** One user says only three sounds remain free. https://www.thecooldown.com/green-tech/bettersleep-app-subscription-complaints-paywall/
  3. **Crashes and sync problems.** https://justuseapp.com/en/app/314498713/relax-melodies-sleep-sounds/reviews
  - "Good but" theme: the sound library and mixing are praised; the drawbacks are the paywall and billing.

---

## Other apps that already stop audio when you fall asleep

| App | Maker | How it works (claim and source) | Price |
|---|---|---|---|
| **Pillow** | Neybox | "with the 'Automatic' option, the sleep aid sound will automatically stop once the app senses you are asleep". https://intercom.help/pillow_app/en/articles/3733551-what-is-sleep-aid . The sleep aid needs the iPhone during sleep; watch-only mode cannot play it. https://intercom.help/pillow_app/en/articles/3733497-pillow-on-the-apple-watch-basics | Not found |
| **Smart Sleep Timer** | Indie | "advanced sound analysis listens for snoring and pauses playback automatically"; works with other media apps. https://apps.apple.com/app/smart-sleep-timer/id6739953694 ; https://www.producthunt.com/posts/smart-sleep-timer | Free (per review site https://aichief.com/ai-lifestyle-tools/smart-sleep-timer/) |
| **Zlpy** | Svipler AB | Apple Watch app that "measures your heart beat and from a level you define it will then pause music/podcasts"; has a sensitivity setting. https://apps.apple.com/is/app/zlpy/id1598960589 | US$1.99 (IS store) / ฿79 (TH) |
| **Sleep When I Sleep (SWIS)** | SWIS App Ltd | "alerts you that you are falling asleep & if not dismissed will pause audio playback", using Apple Watch health data. https://applevis.com/apps/watch/utilities/sleep-when-i-sleep ; https://www.rnib.org.uk/living-with-sight-loss/assistive-aids-and-technology/reading-and-writing/sleep-when-i-sleep-audio-app/ | "Free for 7 days then only £4.99 per annum" (developer support page, not verified against the store) https://pear-dog-r4rd.squarespace.com/support |
| **Apple AirPods, iOS 26** (OS feature, not an app) | Apple | Setting "Pause Media When Falling Asleep", off by default; AirPods Pro 3, AirPods Pro 2, AirPods 4. https://9to5mac.com/2025/11/26/ios-26-gave-airpods-pro-a-new-setting-you-might-want-to-turn-on/ ; https://www.macrumors.com/how-to/ios-26-airpods-auto-pause-media-when-asleep/ . Detection is probably the earbuds' accelerometer (inferred by press; Apple has not documented it). https://tech.yahoo.com/ai/apple-intelligence/articles/airpods-just-got-useful-power-162700779.html | Free with the hardware |
| **Sleep as Android** | Urbandroid | Its Lullaby feature emits "Lullaby stopped playing" and "lowering volume" events, and has sleep-phase events, per the Home Assistant docs. **A built-in stop-on-sleep option was not confirmed.** https://www.home-assistant.io/integrations/sleep_as_android/ | Not checked |
| **Spotify** | Spotify | **No sleep detection**, only a 5 min-1 h or end-of-track timer (https://beebom.com/how-set-spotify-sleep-timer/). Users request the feature: "use a smartwatch that can detect when the user falls asleep to automatically stop the sound playback" https://community.spotify.com/forum/en/discussion/7476215/automatic-sleep-detection-and-playback-stop | n/a |

**Resume after an interruption (not wake detection):**
- **Night White:** release notes say "Audio automatically restarts after app is interrupted". https://apps.apple.com/us/app/night-white/id1395060418
- **Sleepy Noise:** "pauses for calls, alarms and Siri, then fades back in". https://www.sleepynoise.app/
- **Unmet need:** Blogs describe white noise "turning off at night" as a common user complaint. https://myzenzone.app/blog/why-does-your-white-noise-app-keep-turning-off-at-night

## Implications for SLEEP:ON

1. **"Stop when asleep" already exists, so it is not unique on its own.**
   - **Sleep Cycle:** accelerometer mode only, and the sound interferes with its mic detection.
   - **Pillow:** has an "Automatic" stop option.
   - **AirPods on iOS 26:** an OS-level free feature, so any app's audio gets it.
   - **Niche Watch utilities:** Zlpy and SWIS.
   - **Snore-triggered pause:** Smart Sleep Timer.
2. **"Resume when awake" has no competitor with evidence of it.** This is the clearest open space.
3. **Learning a per-user sleep-onset time from morning check-ins: no competitor found doing this.**
4. **The closest real-time heart-rate competitor is DreamTune AI** (Apple Watch heart rate lowers the volume in deep sleep). It is new, has no ratings, and is priced in USD.
5. **Endel adapts its sound to heart rate but only stops on a manual timer.**
6. **Korean price anchors on the KR App Store** (annual where identifiable):
   - Calm: ₩59,000-66,000
   - Endel: ₩88,000/yr
   - Sleep Cycle: ₩45,900
   - BetterSleep: ₩36,000-99,000 tiers
   - SLEEP:ON's planned ₩39,000/yr would sit at or below all of these.
7. **The dominant complaint across the big apps is billing:** trial-to-paid surprises, renewals after cancelling, and free features moving behind the paywall. Accuracy complaints come second (Sleep Cycle).
