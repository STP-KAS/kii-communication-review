# Chronology: content deleted, unpinned, password-gated or blocked (3–5 Oct 2026)

The full timeline, including the original repo going private and this repo's creation, is in [WHAT-HAPPENED.md](WHAT-HAPPENED.md).

All times are Brussels time (CEST, UTC+2). Each entry gives:
- the time window;
- what was public before;
- what changed;
- the evidence.

Hashes are SHA-256. Files under `evidence/` are in this repo. Files marked *(private archive)* are kept in the private research repo and can be checked against the hash on request.

**Context:** this analysis was first published on 3 Oct 2026 at 20:12 CEST, and stp shared it on X at 22:33 CEST. Several changes below followed publication. **The timing is recorded, but the reason for each change is unknown, and no cause is claimed.** Every change is within KII's (or ZETA's) rights.

| # | When (window) | What was public before | What changed | Evidence |
| --- | --- | --- | --- | --- |
| 1 | 3 Oct, between 22:33 and 22:56 | stp (@StppStp) could reply to and engage with @KaspaKii posts. At 22:33 he replied under the Istanbul video post, linking the research and tagging @pvson, @DiiDesertEnergy and @KaspaKii. | **@KaspaKii blocked @StppStp.** By 22:56 his profile view showed "@KaspaKii has blocked you". stp reports the block came about 10 minutes after his reply. | Screenshot [evidence/x/2026-10-03_2256-CEST_kaspakii-has-blocked-you-profile-view.png](evidence/x/2026-10-03_2256-CEST_kaspakii-has-blocked-you-profile-view.png) |
| 2 | 3 Oct 22:56 to 4 Oct 08:06 | KII post [2106432845845540935](https://x.com/KaspaKii/status/2106432845845540935) (3 Oct 19:15): three audience-filmed clips of other organisations' talks at the Dii summit in Istanbul. | **Deleted by its author.** At 08:06 on 4 Oct X showed "This Post was deleted by the Post author". At 08:14 the X API returned "Not Found", and it still does on 5 Oct at 08:23. **Case closed.** | Screenshot [evidence/x/2026-10-04_0806-CEST_kii-istanbul-video-post-deleted-by-author.png](evidence/x/2026-10-04_0806-CEST_kii-istanbul-video-post-deleted-by-author.png); [API 4 Oct 08:14](evidence/x/2026-10-04_0814-CEST_x-api-get-post-2106432845845540935.json); [API 5 Oct 08:23](evidence/x/2026-10-05_0823-CEST_x-api-posts-not-found.json); hashes of the three original videos, downloaded before deletion: [original-videos-sha256.txt](evidence/x/original-videos-sha256.txt) |
| 3 | 3 Oct evening (before 20:12) to 4 Oct about 09:44 | The KONI satellite announcement ([1910975894144888993](https://x.com/KaspaKii/status/1910975894144888993), 12 Apr 2025: "Launch window: 2026", "All open-source") was the **pinned post** on @KaspaKii, per the X API on the evening of 3 Oct. | **Unpinned**, with no status update. The post still exists (210,368 impressions on 4 Oct, 09:45). | [API user lookup, 4 Oct 09:45](evidence/x/2026-10-04_0945-CEST_x-api-user-kaspakii-pinned-expansion.json) (no `pinned_tweet_id`) |
| 4 | 3 Oct 20:55 to 5 Oct 00:09 | kaspa-kii.org: "Built, tested, ready for launch"; "Launching on Kaspa"; products "operated by separate commercial vehicles". | **Website wording edited:** "KiiWORKS anchors on Kaspa mainnet today; WarpCore and Meridian are built"; "Built on Kaspa"; "Products are built and operated by KiiLabs"; the Foundation "does not develop, sell, or operate them". No changelog or announcement. | [Text diff](evidence/web/kii-site_diff_2026-10-03_vs_2026-10-05.txt). HTML snapshots *(private archive)*: index `124b8312…104d` → `5eb653b5…ac89`; foundation `d6e1a0fa…0412` → `ec415a9e…e3e9`; contact `61714122…b036` → `ef8bbdfb…e9ee` |
| 5 | 5 Oct, after 01:28 (last public read) and by 07:36 | `anchorage.kaspa-kii.org`: a KII **"Trusted Trade"** demo (testnet-10, "SYNTHETIC DEMO DATA"), an operator console, a verifier and a 2-page brief. It was served **without login**, although the brief was marked "Private & Confidential". Its first TLS certificate dates from 12 Aug 2026. It was found through certificate-transparency logs and documented in the research repo at 01:30. | **Put behind a password:** HTTP 401, `WWW-Authenticate: Basic realm="Kii private"`, `X-Robots-Tag: noindex, nofollow, noarchive, nosnippet, noimageindex, noai, noimageai`. KII never announced the demo on X or its website. | [Header check 07:39](evidence/web/2026-10-05_0739-CEST_access-changes.txt). Brief PDF *(private archive, not republished)*: `9dacf4678b865723bfbd75c5b27fb4f4d936a4991fc08efa5fbc56c382da9a99`; console run.json *(private archive)*: `64c05ca7904ce7404b1cd1fd0e367a4e7cc9467a64271d2b7b6f0e85906adf26`. No Wayback capture exists. |
| 6 | 5 Oct, same window | `kiiworkspublicdemo.kaspa-kii.org`: the **KiiWORKS Workbench**, a browser UI that needed the user's own node. Served without login; first certificate 16 Jul 2026. | **Put behind the same password** (HTTP 401, realm "Kii private", same no-index/no-AI headers). | [Header check 07:39](evidence/web/2026-10-05_0739-CEST_access-changes.txt) |
| 7 | 5 Oct, after 01:28 and by 07:36; still in place at 08:22 | kaspa-kii.org (Netlify) and zeta-global.org (Cloudflare) answered the research repo's daily check script normally. Its user agent identifies itself: `kaspa-kii-analysis-tripwires/1.0 (+repo URL)`. | **User-agent block on both sites:** HTTP 403 for user agents containing "kaspa-kii-analysis" or "tripwires/1.0". Generic user agents still get HTTP 200. The same rule appeared on two hosts at two providers in the same window. *Inference, not verified:* this is consistent with one party configuring both sites. The script was **not** disguised to get around the block. | [User-agent test 07:39](evidence/web/2026-10-05_0739-CEST_access-changes.txt) (one request per user agent) |
| 8 | ZETA's site, 5 Oct, between 01:28 and 08:23 | ZETA's draft standards library (`zeta-global.org/corpus/…`), some of which treat Kaspa as a reference implementation, was publicly readable, as on 4 Oct. | **Moved behind a members-only login:** a 301 redirect to `/members/corpus/…`, then a Cloudflare Access login. ZETA is a separate organisation, but KII people hold senior roles there (chairman and secretary general per ZETA's site). This repo republishes none of that material. | [Header check 08:23](evidence/web/2026-10-05_0823-CEST_zeta-corpus-members-only.txt) |
| 9 | By 5 Oct 08:23 | stp's own post [2106867660869001661](https://x.com/StppStp/status/2106867660869001661) (5 Oct 00:02, time decoded from the ID), to which @3DRudy replied at 00:49. | The X API returns **"Not Found"**. Recorded for completeness; no further comment. | [API 5 Oct 08:23](evidence/x/2026-10-05_0823-CEST_x-api-posts-not-found.json) |

## Earlier removals (exact removal dates unknown)

| What was public | Archive | Now |
| --- | --- | --- |
| Team page `/about-us/` naming the chairman, secretary general, board and staff (2024) | [Wayback, 17 Nov 2024](https://web.archive.org/web/20241117000000*/kaspa-kii.org/about-us/) | 404; the site names no people |
| KONI mission page `/koni/` | [Wayback, 10 Oct 2025](https://web.archive.org/web/20251010071310/https://kaspa-kii.org/koni/) | 404 |
| WarpCore: "open-source development and global community governance" | [Wayback, Jan 2026](https://web.archive.org/web/2026*/kaspa-kii.org/warpcore/) | "Closed source. Open surface." |
| `/roadmap/`, `/initiatives/` (GigaWatt, ZET-EX), `/kii-academy/`, `/launch-of-kii/` | [Wayback URL list](https://web.archive.org/web/*/kaspa-kii.org/*) | Removed |
| The Dubai summit deck (Nov 2025), linked from a KII post | n/a | Link dead (404) |

## Reading this chronology [O]

None of these steps is improper on its own:
- an organisation may block an account, delete a post, unpin a project, edit its site, password-protect a demo or filter automated traffic;
- ZETA may restrict its drafts to members.

Taken together with the delivery record in [DELIVERY.md](DELIVERY.md), they show a communication style that **withdraws material instead of explaining it**. A dated status page and a short public note ("demo moved to private access; contact us for a walkthrough") would have cost little and said more.
