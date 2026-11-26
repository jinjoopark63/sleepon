# SLEEP:ON (스르르): substitutes, platform threats, Korean market facts
Research date: 2026-11-25. Public web only.

**Method caveat:** In this session, direct page fetching failed for samsung.com and mt.co.kr (host not resolvable from the sandbox). Every fact below comes from web-search result text quoting the cited URL. I did not open the pages themselves, so check a figure on its page before using it in anything public. Wherever something could not be found, this file says so.

---

## 1. Substitutes (how Korean buyers handle this without a paid sleep app)

| Substitute | Price in Korea | Sleep-stop feature | Source |
|---|---|---|---|
| YouTube (free) sleep music / ASMR | Free with ads | **Fixed sleep timer** (10/15/20/30/45 min, 1 h), available to all users since Oct 2024 (earlier a Premium-only test in Aug 2024). Mobile is confirmed; desktop and TV are unclear. No sleep detection. | https://m.gsmarena.com/youtube_launches_sleep_timer_for_everyone_adds_finetuning_for_playback_speed-news-64943.php ; https://9to5google.com/2024/08/09/youtube-is-now-testing-a-built-in-sleep-timer-but-only-with-premium-subscribers/ ; https://theprint.in/tech/youtube-expands-sleep-timer-feature-to-all-users/2314302/ |
| YouTube Premium | KRW 14,900/mo (web/Android), KRW 19,500/mo (iOS App Store), as of Sep 2026 per secondary sources. **Premium Lite** (no YouTube Music): KRW 8,500 (web/Android) / KRW 10,900 (iOS), launched in Korea around Jan–Feb 2026. No family or student plan in Korea. | Same timer | https://www.lguplus.com/pogg/magazine/유튜브-프리미엄-할인-혜택-가격-알아보기 ; https://www.banksalad.com/articles/2023-유튜브-프리미엄-가격-정리-및-할인-방법-4가지 ; https://blog.youtube/intl/ko-kr/news-and-events/yt-premium-lite-kr/ ; https://www.newsis.com/view/NISX20260202_0003498858 (not verified on an official YouTube price page) |
| Spotify | Premium Individual **KRW 11,990/mo** (official KR page). A blog lists Basic at KRW 8,690, Student at 6,600 and Duo at 17,985 (unverified). | **Sleep timer** on mobile, desktop and Wear OS (Spotify newsroom, Aug 29 2025). Timer only. | https://www.spotify.com/kr/premium/ ; https://newsroom.spotify.com/tag/sleep-timer ; https://www.bohumpixel.com/post/스포티파이-프리미엄 |
| Apple Music | **KRW 8,900/mo** individual (apple.com/kr). A blog lists Family at 13,500. | No in-app sleep detection. iPhone **Clock timer → "Stop Playing"** stops any media when the timer ends (official Apple guide). | https://apple.com/kr/apple-music ; https://www.banksalad.com/articles/애플뮤직-가격-무료-가족공유-싸게-이용하는-팁 ; https://support.apple.com/en-kz/guide/iphone/iph96b1e460/13.0/ios |
| Melon | **Current monthly price: not found.** Reports from 2026: a bundle with YouTube Premium Lite at up to 20% off (Aug 2026); Melon considering an ad-supported tier (Jun 2026). | Not found in search (no source confirming a 취침예약 / sleep timer) | https://www.dailian.co.kr/news/view/1673895/ ; https://www.ceoscoredaily.com/page/view/2026062215075508612 |
| White-noise machine | MARPAC "백색소음기 돔" at **KRW 99,000** (wishbucket.io price tracker, recorded 2026-07-30; a similar item at 119,000). Coupang-affiliate blogs cite generic sleep white-noise devices at roughly KRW 10,000–35,000. **No Coupang, Naver or Danawa product page with a price was found.** | Device timers only, no detection | https://www.wishbucket.io/items/1707162 ; https://wikidocs.net/blog/@smartliving/27393/ |
| Free white-noise apps | e.g. "White Noise Pro" on the KR App Store (price not checked) | n/a | https://apps.apple.com/kr/app/white-noise-pro/id363936074 |

**Takeaway:** every mainstream substitute offers only a **fixed-duration timer**. None of the music or video apps found stops on detected sleep or resumes when the user wakes. The free timer (YouTube, Spotify, iOS Clock) is the "good enough" bar SLEEP:ON has to beat.

---

## 2. Platform threats

### Apple: ALREADY pauses audio when you fall asleep (AirPods)
- **iOS 26 "Pause Media When Falling Asleep"** (Apple's older page calls it "...While Falling Asleep"). Apple's support page says: "If you have AirPods 4, AirPods Pro 2, or AirPods Pro 3, you can choose to pause media automatically when you fall asleep." A newer Apple user guide also lists AirPods 5 and AirPods Max 2. It is available on iPhone/iPad and also on macOS Tahoe and tvOS 26. https://support.apple.com/en-mt/108764 ; https://support.apple.com/en-al/guide/airpods/dev57e5b7e58/web
- Apple has not published how it detects sleep. Press reports say it uses the AirPods' motion sensors and does **not** need an Apple Watch. https://www.macrumors.com/how-to/ios-26-airpods-auto-pause-media-when-asleep/ ; https://bgr.com/2002129/how-airpods-know-when-you-fall-asleep
- Sources disagree on the default: MacRumors says it is on by default, iGeeksBlog says it is off. https://www.macrumors.com/how-to/ios-26-airpods-auto-pause-media-when-asleep/ ; https://www.igeeksblog.com/airpods-auto-pause-when-you-fall-asleep/
- Beats headphones are reported to get it as well. https://www.macrumors.com/2025/07/01/beats-airpods-sleep-pause-ios-26/
- **Pause only.** No source found mentions resuming when the user wakes. A developer thread says apps get **no API or callback** telling them the reason for the pause (for example, it can pause meditation audio when the user is just lying still). https://developer.apple.com/forums/thread/842375
- Apple Watch: watchOS 26 added a **Sleep Score** (Series 6 and later, SE 2 and later, Ultra), with ranges adjusted in 26.2. https://www.macrumors.com/2025/09/10/watchos-26-sleep-score/ ; https://www.macrumors.com/2025/11/04/watchos-26-2-updates-sleep-score-ranges/ . Sleep Focus / Wind Down: **no official page was retrieved** and nothing found ties either one to pausing media.

### Samsung: no shipped "pause audio on sleep" found, but it is leaked and the sleep-detection plumbing exists
- **Galaxy Watch / Ring + SmartThings:** "when sleep is detected, Galaxy Ring/Watch turns off the lights and TV, adjusting temperature and airflow." This is a SmartThings Modes & Routines feature (Sleep → Turn on automatically). It needs Watch4–7, Ultra, Fit3 or Ring, and "may not be supported in certain countries." https://www.samsung.com/sa_en/smartthings/get-ideas/ ; https://news.samsung.com/us/samsung-announces-latest-smartthings-update/ ; Samsung US support also says the Watch "can detect when you've fallen asleep and turn these devices off": https://www.samsung.com/us/support/answer/ANS00090402/
- Korean community posts say the SmartThings 취침 setting can add "워치 수면 감지" to turn off lights/TV. A 2022 user request for a **media-pause-on-sleep routine** got a "will forward to the relevant team" reply from Samsung. https://r1.community.samsung.com/t5/smartthings/%EC%9E%90%EB%8F%99%ED%99%94-%EB%A3%A8%ED%8B%B4-%EC%B6%94%EA%B0%80%EC%97%90-%EC%A0%9C%EC%95%88%ED%95%A9%EB%8B%88%EB%8B%A4/m-p/16146951/highlight/true
- **Leak (not shipped):** an APK teardown of the Buds Manager app for the rumored **Galaxy Buds On** shows a setting, "**Pause media while you're asleep**", that "can automatically stop whatever you're listening to once your phone determines that you've fallen asleep." It reportedly **requires One UI 9.0+**, and the detection method is unclear (possibly a Galaxy Watch). Reported Sep 2026. https://www.soundguys.com/samsung-galaxy-buds-on-leak-162959/ ; https://9to5google.com/2026/09/10/samsung-galaxy-buds-on-open-ear-leak/ ; https://hothardware.com/news/samsung-galaxy-buds-on-leak-reveals-clip-on-design-and-ai-tricks
- Galaxy Buds4 / Buds4 Pro launched Feb 2026. **No sleep-pause feature found** for them. Existing Samsung pages only describe music stopping when the phone enters power-saving "sleep mode," which is unrelated. https://news.samsung.com/global/samsung-unveils-all-new-galaxy-buds4-series-with-ultimate-sound?pubDate=20260226 ; https://www.samsung.com/in/support/mobile-devices/galaxy-buds-music-stops-during-sleep-mode-of-mobile/
- **2026 AI 무풍 에어컨 "웨어러블 굿슬립":** the Galaxy Watch (or Ring) detects sleep onset and sleep stages, and the air conditioner fine-tunes temperature to match. Products: Bespoke AI 무풍콤보 갤러리 프로 (stand) and 무풍콤보 프로 벽걸이, announced 2026-02-05. Samsung says it is also researching radar sensors to detect sleep **without a wearable**. https://www.ddaily.co.kr/page/view/2026020513013497832 ; https://biz.sbs.co.kr/amp/article/20000221225 ; https://kpinews.kr/newsView/1065575368470752 ; https://news.samsung.com/sg/2026-windfree-intelligent-cooling ; Samsung KR newsroom: https://www.samsung.com/sec/business/insights/news/news_260209_05/ (could not be fetched)

### Google / Fitbit: ALREADY pauses audio on sleep (Pixel Watch + Pixel Buds)
- The Pixel Watch auto-bedtime mode uses Fitbit sleep detection. https://www.androidauthority.com/auto-bedtime-mode-pixel-watch-3-3483161 ; https://support.google.com/pixelphone/answer/13532591?hl=en
- A firmware update for **Pixel Buds Pro 2 / Pixel Buds 2a** pauses audio, silences notifications and disables touch controls once the paired **Pixel Watch** detects sleep. This requires a Pixel Watch. https://cordcuttersnews.com/google-rolls-out-a-massive-update-to-the-pixel-buds-earbuds/?amp=1 (single secondary source; Pixel has a small share in Korea)

**Threat summary:** Apple (AirPods, iOS 26) and Google (Pixel Buds with Pixel Watch) already stop audio on detected sleep. Samsung, which dominates Android in Korea, has only leaked it (Buds On, One UI 9). Its watch sleep detection already drives lights, TV and the air conditioner through SmartThings. Gaps that remain for SLEEP:ON, based on what was found: (a) none of the platforms is reported to **resume on waking**; (b) none **gradually fades** audio; (c) the features only work with each company's own earbuds or watch, so speaker playback and non-Apple/Pixel earbuds are not covered; (d) there is no personalized sleep-onset learning. Expect Samsung to close (c) for Galaxy users soon.

---

## 3. Korean market facts

**Insomnia patients (HIRA):**
- **2025: 797,862** patients treated for F51.0 (비기질성 불면증) or G47.0 (수면 개시 및 유지장애), up 19.2% from 669,536 in 2021. Benefit costs rose from KRW 18.0bn to 30.5bn. 60대 was the largest age group (204,706). Source: HIRA "지역별 불면증 진료현황(2021~2025)" as reported by 매일신문. https://www.imaeil.com/page/view/2026081412563077188
- 2024: 768,814 (2020: 658,675), 60.5% female (HIRA, via 머니투데이). Codes not confirmed. https://www.mt.co.kr/thebio/2026/05/30/2026052911275895752
- All sleep disorders (wider scope): about 1.35M treated in 2025 (1,346,196, versus 1,088,038 in 2021), per an English-language report. https://asianews.network/?p=287617 ; NHIS raw data: https://www.data.go.kr/data/15124322/fileData.do

**Share of adults with sleep difficulty:**
- Statistics Korea, **2024 생활시간조사** (released 2025-07-28), people aged 10+: share who said "잠을 이루지 못한다" rose from **7.3% (2019) to 11.9% (2024)**, increasing in every age group, with 60+ highest at 19.6%. Average sleep 8h01m, down 8 minutes (the first decline since 1999). Media use rose from 2h26m to 2h45m. https://www.newsis.com/view/NISX20250728_0003268438 (YTN reports 8h04m: https://www.ytn.co.kr/_ln/0102_202507282236382064). **A 20s–30s breakdown was not found.**
- Philips Korea / 한국리서치 (Mar 2025, n=2,000 adults; company survey): 68.6% have sleep disrupted by symptoms, with insomnia at 29.3%. https://zdnet.co.kr/view/?no=20250312132401 ; https://economist.co.kr/article/view/ecn202503130069
- 대한수면(연구)학회 "2024 한국인의 수면 실태" (Mar 2025): average sleep 6h58m, only 7% sleep well every night. It compiles third-party surveys and is not a primary epidemiological study. https://magazine.hankyung.com/business/article/202503131405b
- **Newer than Cho et al. 2009 (3.12M):** no newer peer-reviewed national count of "adults 20–69 with difficulty falling asleep 2+ times/week" was found. Closest items: a 2012 face-to-face survey (age 19–69) with ISI ≥11 insomnia at about 10.8% (https://pmc.ncbi.nlm.nih.gov/articles/PMC6952093 or nearby; see the search list), and an online survey of 4,000 adults aged 20–69 (Jan 2021–Feb 2022) reporting that insomnia prevalence rose during COVID (https://link.springer.com/content/pdf/10.1007/s41105-023-00464-2.pdf ; https://pmc.ncbi.nlm.nih.gov/articles/PMC10196317). **I could not extract the exact prevalence percentages from these papers. Open them before quoting.**

**Sleep economy / sleep-tech market size:**
- Korea: **KRW 480bn (2011) → about KRW 3 trillion (2021)**, 한국수면산업협회 estimate (cited by KB and others). This is the latest Korean figure found. **No 2024–2026 Korea-specific sleep-economy or 슬립테크 market size was found.** https://kbthink.com/main/economy/economic-in-depth-analysis/economic-knowledge-vitamin/2024/economic-knowledge-vitamin-2-240401.html ; https://www.gangnam.go.kr/gangnamlife/2025/html/vol357/sub01_08.html
- Global sleep economy: USD 432bn (2019) → 585bn (2024), Statista via 삼정KPMG (Aug 2024). https://kpmg.com/kr/ko/media/press-releases/2024/08/press-release-0808.html ; https://assets.kpmg.com/content/dam/kpmg/kr/pdf/2024/business-focus/kpmg-korea-sleeptech-20240805.pdf
- Global sleep tech: USD 32.1bn (about KRW 45 trillion) by 2026, per Global Market Insights. https://www.mt.co.kr/future/2025/01/08/2025010715312384966
- KPMG also reports Korean sleep-disorder patients rising from 860k (2018) to 1.1M (2022), +6.5%/yr. https://kpmg.com/kr/ko/insights/eri/2024/businessfocus-0805.html

## Not found / open items
- Melon's current price and whether it has a sleep timer
- A Korean white-noise machine price on Coupang, Naver or Danawa (only a price-tracker figure was found)
- An official YouTube KR Premium price page (prices come from secondary sources)
- Official Apple pages on Sleep Focus or Wind Down
- Korea-specific sleep-tech market size after 2021
- A 20s–30s-specific sleep-difficulty share
