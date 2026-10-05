# What happened: timeline, 3–5 Oct 2026

All times are **Europe/Brussels (CEST, UTC+2)**. Each entry is an observed fact with its evidence. Hashes are SHA-256. Files under `evidence/` are in this repo. *(private archive)* marks files kept in the private research repo that can be checked against the hash.

This page states **what was observed and when**. It does **not** claim why anything happened. Every action listed is within the rights of the account or organisation that took it.

## In short

1. **The original analysis repo is now private.** `STP-KAS/kaspa-kii-analysis` was made private by its owner on **5 Oct 2026 at 08:22 CEST**.
   - It held working copies and excerpts of draft ZETA standards, which have since moved behind a members-only login, and of a KII brief marked "Private & Confidential".
   - The goal was never to dump documents.
   - **Old links to `kaspa-kii-analysis` now return 404.** That includes the links in stp's earlier X replies and in the comment on its issue #1 (5 Oct, 01:31 CEST).
   - **This repo, [STP-KAS/kii-communication-review](https://github.com/STP-KAS/kii-communication-review), replaces them.**
2. **stp's own X post of 5 Oct 2026 at 00:02 CEST** (ID 2106867660869001661, the post @3DRudy / RuDeeVelops replied to at 00:49) returns **"Not Found"** from the X API. Observed on **5 Oct at 08:23 CEST**. No cause is claimed.
3. **ZETA's document corpus** (`zeta-global.org/corpus/…`) moved behind a **members-only login** (Cloudflare Access).
   - Last read publicly: 5 Oct, 01:27–01:28 CEST.
   - Observed behind the login: 5 Oct, 08:23 CEST.
   - This repo does **not** access or reproduce restricted material.
   - Monitoring continues only on **public pages**, using **Internet Archive (Wayback Machine) snapshots**.

## Full timeline

| # | Date and time (CEST) | What was observed | Evidence |
| --- | --- | --- | --- |
| 1 | **3 Oct, 19:15** | @KaspaKii posts three audience-filmed clips from the Dii summit in Istanbul (post [2106432845845540935](https://x.com/KaspaKii/status/2106432845845540935)). The clips show other organisations' talks. KII is not shown. | Post time decoded from the ID; video hashes in [original-videos-sha256.txt](evidence/x/original-videos-sha256.txt) |
| 2 | **3 Oct, 20:12** | The original analysis is first published (`STP-KAS/kaspa-kii-analysis`, first commit `ab17f08`). | Private archive git history |
| 3 | **3 Oct, evening (before 20:12)** | The X API shows the KONI satellite post ([1910975894144888993](https://x.com/KaspaKii/status/1910975894144888993), 12 Apr 2025) as **pinned** on @KaspaKii. | X API user lookup *(private archive)*; recorded in the first publication |
| 4 | **3 Oct, 20:55** | The KII website reads "Built, tested, ready for launch" and "Launching on Kaspa", and says products are "operated by separate commercial vehicles". | HTML snapshots *(private archive)*: index `124b8312…104d`, foundation `d6e1a0fa…0412`, contact `61714122…b036` |
| 5 | **3 Oct, 22:33** | stp (@StppStp) replies under the Istanbul post, linking the analysis and tagging @pvson, @DiiDesertEnergy and @KaspaKii. | Screenshot showing "22:33 · 3/10/26": [evidence/x/…0806…deleted-by-author.png](evidence/x/2026-10-04_0806-CEST_kii-istanbul-video-post-deleted-by-author.png) |
| 6 | **3 Oct, by 22:56** | stp's profile view of @KaspaKii shows **"@KaspaKii has blocked you"**. The Istanbul post is still visible ("3h"). stp reports the block came about 10 minutes after his reply. | Screenshot [evidence/x/…2256…blocked-you….png](evidence/x/2026-10-03_2256-CEST_kaspakii-has-blocked-you-profile-view.png) |
| 7 | **3 Oct 22:56 to 4 Oct 08:06** | The Istanbul post is **deleted by its author**. At 08:06 X shows "This Post was deleted by the Post author", and at 08:14 the X API returns "Not Found". **The post is deleted and this case is closed.** | [Screenshot 08:06](evidence/x/2026-10-04_0806-CEST_kii-istanbul-video-post-deleted-by-author.png); [API 08:14](evidence/x/2026-10-04_0814-CEST_x-api-get-post-2106432845845540935.json) |
| 8 | **3 Oct evening to 4 Oct, about 09:44** | The KONI post is **unpinned**. The X API at about 09:45 on 4 Oct shows no pinned post. The KONI post itself still exists. No status update was posted. | [API 4 Oct 09:45](evidence/x/2026-10-04_0945-CEST_x-api-user-kaspakii-pinned-expansion.json) |
| 9 | **3 Oct 20:55 to 5 Oct 00:09** | **Website wording edited.** It now reads "KiiWORKS anchors on Kaspa mainnet today; WarpCore and Meridian are built", "Built on Kaspa" and "Products are built and operated by KiiLabs"; the Foundation "does not develop, sell, or operate them". No notice or changelog. | [Text diff](evidence/web/kii-site_diff_2026-10-03_vs_2026-10-05.txt); 5 Oct HTML *(private archive)*: index `5eb653b5…ac89`, foundation `ec415a9e…e3e9`, contact `ef8bbdfb…e9ee` |
| 10 | **5 Oct, 00:02** | stp posts on X (2106867660869001661). At **00:49** @3DRudy (RuDeeVelops) replies with method advice ([2106879480123801695](https://x.com/3DRudy/status/2106879480123801695)). | Post time decoded from the ID; Rudy's reply still exists ([API 08:23](evidence/x/2026-10-05_0823-CEST_x-api-posts-not-found.json)) |
| 11 | **5 Oct, 01:27–01:28** | The research repo's daily check script reads, **publicly and without login**: kaspa-kii.org; the KII "Trusted Trade" demo at `anchorage.kaspa-kii.org` (testnet, synthetic data; never announced by KII; first TLS certificate 12 Aug 2026); the KiiWORKS Workbench at `kiiworkspublicdemo.kaspa-kii.org` (first certificate 16 Jul 2026); and ZETA's corpus. | Tripwire baseline state *(private archive)*, SHA-256 `529a842251b04ccbb1f7ac9af0c3330996d1a404977c2e8b5325feb5792828b6` |
| 12 | **5 Oct, 01:30** | The research repo publishes the demo findings (commit `ff2b9e0`). At **01:31** a summary comment is posted on its issue #1. | Private archive git history; GitHub comment timestamp 2026-10-04T23:31:07Z |
| 13 | **5 Oct, after 01:28 and by 07:36** | The **demo and the Workbench go behind a password**: HTTP 401, `WWW-Authenticate: Basic realm="Kii private"`, plus no-index / no-AI headers. | [Header check 07:39](evidence/web/2026-10-05_0739-CEST_access-changes.txt); tripwire report 07:37 *(private archive)* `fe5e8d73…c418`; brief PDF *(private archive, not republished)* `9dacf467…9a99` |
| 14 | **5 Oct, after 01:28 and by 07:36** | **User-agent blocks:** kaspa-kii.org (Netlify) and zeta-global.org (Cloudflare) return HTTP 403 to user agents containing "kaspa-kii-analysis" or "tripwires/1.0", the check script's own user agent. Generic user agents get HTTP 200. The script was not disguised to get around this. | [User-agent test 07:39](evidence/web/2026-10-05_0739-CEST_access-changes.txt) |
| 15 | **5 Oct, after 01:28 and by 08:23** | **ZETA corpus members-only:** `/corpus/…` returns a 301 redirect to `/members/corpus/…`, then a Cloudflare Access login. | [Header check 08:23](evidence/web/2026-10-05_0823-CEST_zeta-corpus-members-only.txt) |
| 16 | **5 Oct, 08:22** | The original analysis repo `STP-KAS/kaspa-kii-analysis` is made **private** by its owner. Content and history are unchanged. Old links return 404. | [Visibility check](evidence/web/2026-10-05_0822-CEST_repo-visibility.txt) |
| 17 | **5 Oct, observed 08:23** | stp's post of 5 Oct 00:02 (2106867660869001661) returns **"Not Found"** from the X API. The Istanbul post also still returns "Not Found". | [API 08:23](evidence/x/2026-10-05_0823-CEST_x-api-posts-not-found.json) |
| 18 | **5 Oct, 08:25** | **This repo is created**, public (first commit `f334ddc` at 08:25:25). It contains no ZETA drafts and no "Private & Confidential" material. | [Visibility check](evidence/web/2026-10-05_0822-CEST_repo-visibility.txt); this repo's git history |

## Notes

- **Time windows** (rows 7, 8, 9, 13, 14, 15) are bounded by two observations: the last time something was seen one way and the first time it was seen the other way. The exact moment of change inside each window is unknown.
- **No motive is claimed** for any change. Restricting a demo, filtering automated traffic, deleting or unpinning a post, editing a website or limiting drafts to members are all legitimate choices. How they read as **communication** is discussed in [COMMUNICATION.md](COMMUNICATION.md).
- Earlier removals (2024 team page, KONI page, WarpCore "open-source" wording), with archive links: [CHRONOLOGY.md](CHRONOLOGY.md#earlier-removals-exact-removal-dates-unknown).
