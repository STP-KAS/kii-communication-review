# Delivery: promised, proven, delivered

Checked 3–5 Oct 2026. Labels: [F] fact, [C] KII claim, [O] opinion. X post IDs open at `https://x.com/KaspaKii/status/<id>`.

## Balance table (as of 3 Oct 2026; updated 5 Oct)

| Item | Promised (when) | Proven (public evidence) | Delivered? |
| --- | --- | --- | --- |
| Mainnet covenant ("quine") | "First covenant on Kaspa mainnet" (30 Jun 2026, 2071995662867066890) | Genesis and 3 generations accepted on mainnet on 30 Jun 2026; genesis tx `1c1a4c549c664147814d9836e623373991622c1dc711a4227f206ad5f6a241c5` | **Yes.** "First" is unverified. |
| Portrait (covenant language) | Covenant language, 35 patterns, 5 "settled live on TN10" | Public MIT repo (1 commit, 1 Sep 2026). The TN10 txids could not be re-checked (3 Oct). | **Yes, testnet-only** (as labelled) |
| Post-quantum zkVM benchmark | PQ signature verification in a zkVM | Public repo; a third-party GPU benchmark | **Yes, research** |
| Optical mining study | Optical kHeavyHash feasibility | Public study, which concludes the idea is uncompetitive by 30–80x | **Yes, research** |
| WarpCore | ISO 20022 bridge; "open-source development" (Jan 2026); "Launching Today… sandbox environment for financial institutions" (5 Jan 2026, 2008147081047777382); "286 transaction type tests, 100% pass" (28 Mar 2026, 2037853916117742071); Fed/SEPA "READY FOR INTEGRATION" (30 Mar 2026, 2038753059149365327) | Detailed docs marked Draft; deployment "gated on audit" per its own docs; closed source; no public sandbox, test artefacts or named participant | **No public product** |
| Meridian | Institutional asset platform, KIT token | Docs marked draft; closed source | **No public product** |
| KiiWORKS | Trade documents, digital product passports, did:kaspa; "Pilots are moving forward" (27 Jul 2026). Since 3–5 Oct the website says "KiiWORKS anchors on Kaspa mainnet today". | Docs; closed source; partly stale (Testnet-12). No mainnet anchor txid published. The Workbench demo host went behind a password on 5 Oct. | **No public product** |
| "Trusted Trade" demo (never announced) | A brief (12 Aug 2026) says KII "has turned the trusted-trade concept into a running system" | Testnet-10 demo with synthetic data. By its own account, "A named counterparty", a legal opinion and an audit were still missing. Its txids did not resolve on the public TN10 API on 5 Oct (testnet resets void them, so this is weak evidence either way). Password-gated since 5 Oct. | **Demo only, now private** |
| "Completed our main flagship projects… June is going to be a blast!" | 30 Apr 2026 (2049806241333928434) | Only the quine and Portrait are public | **No** |
| **KONI** satellite node | CubeSat with a Kaspa node; "Launch window: 2026 - rideshare"; "All open-source. All community powered." (12 Apr 2025); later "satellites" (plural) | No hardware, launch contract, frequency coordination, licence filing, SatNOGS entry, code or named team. The dedicated page was removed. | **No.** Unpinned 3–4 Oct 2026 without a status update |
| GigaWatt / GWU stablecoin | Energy-backed, "carbon negative" settlement unit (2024–25) | Slides only; no spendable stablecoin exists on Kaspa L1 | **No** (dropped from the site) |
| ZET-EX exchange | Energy and carbon exchange (2024–25); "live demonstration" (Nov 2025 deck) | Screenshots in the deck only | **Demo only** |
| "KRC-20T (Trusted)" token standard | Oct 2024 | No spec in KIPs or KCCs | **No** |
| Kii Academy | Acceleration, mentorship, funding (Oct 2024) | Guidelines and a form | **Unknown** |
| ECB Pontes | "Officially applied" (30 Aug 2025, 1961718140099768694) | Not on the ECB's participant list (Oct 2025) | **No** |
| Named pilots and partners | "key financial partners" (14 Dec 2024), "pilots moving forward" | None named publicly | **Unverified** |
| Transparency | Team named (2024) | Team page removed; no entity number, funders or owners of the operating company | **Went backwards** |

## KONI in brief

- **Announced** on 12 Apr 2025 ([1910975894144888993](https://x.com/KaspaKii/status/1910975894144888993)): "We're sending a Kaspa node into space." The timeline post ([1910975898477551837](https://x.com/KaspaKii/status/1910975898477551837)) gave a "Launch window: 2026", a mission of "~24+ months" and "All open-source. All community powered."
- **17 May 2025:** "We will post more detailed project information early next week" ([1923745571203874985](https://x.com/KaspaKii/status/1923745571203874985)). A full-archive X search found **no such post** afterwards.
- **Sep–Nov 2025:** "The KONI satellites will reinforce this even further." The payloads would be "fully open to the R&D team for Dagknight testing". The Nov 2025 Dubai deck listed a "Satellite node pilot: testing platform in space".
- **What exists [F]:** a symbolic mission page (archived 10 Oct 2025; now 404) and posts. No hardware photos, launch provider, ITU/IARU coordination, licence, SatNOGS entry, repository, budget or team.
- **Pinned, then unpinned [F]:** it was the pinned post on 3 Oct 2026 (the date it was pinned is not known). It was unpinned between the evening of 3 Oct and about 09:44 CEST on 4 Oct, with no status update.
- **[O]** A 2026 launch now looks very unlikely. Unpinning without a word leaves the public question open: is KONI active, paused or stopped?

## Claims dated against the Kaspa protocol

The protocol milestones come from the community-maintained Kaspa master file (`STP-KAS/kaspa-master-file` at commit `4183b7a`):
- **Crescendo:** May 2025.
- **Toccata:** live on mainnet at DAA 474,165,565 on about 30 Jun 2026, with covenants (KIP-17), covenant IDs (KIP-20), a ZK precompile (KIP-16) and sequencing commitments (KIP-21).
- **Still not live:** vProgs (research), DAGKnight and a spendable L1 stablecoin.

| KII claim (date) | Months before Toccata covenants (30 Jun 2026) | Enabling layer still missing on 4 Oct 2026 |
| --- | --- | --- |
| WarpCore, GigaWatt StableCoin, ZET-EX introduced (4 Oct 2024) | **about 21** | Spendable L1 stablecoin |
| WarpCore "showcased with key financial partners" (14 Dec 2024) | about 18.5 | None identified |
| ISO 20022 via WarpCore (25 Mar 2025) | about 15 | None identified |
| Dubai deck: "MVP operational", "Global Sequencing Network" (Nov 2025) | about 7.5 | vProgs, the layer that would use sequencing |
| "Launching Today: WarpCore (Phase 1) sandbox" (5 Jan 2026) | about 6 | None identified |
| "286 transaction type tests, 100% pass" (28 Mar 2026) | about 3 | None identified |
| "Built, tested, ready for launch" (website until 3–5 Oct 2026) | after | No audit published; KII's own docs say "gated on audit" |

**[O]** Public product claims came between about 3 and 21 months before covenants reached mainnet. Two of them (the stablecoin and the "sequencing network" pitch) came before layers that do not exist even now.

**Fairness caveats:**
1. Not every claim needed Toccata. Anchoring a hash in a transaction does not need covenants, and KONI does not depend on programmability at all. The timing argument is strongest for the stablecoin, atomic payment-versus-payment, the "sequencing network" pitch and "ready for launch" without an audit.
2. KII built early, and its covenant was live on Toccata day. The criticism is about how products were described in public, not that work started early.
3. The master file is a community source. Where it cites a release tag or a merged KIP, that primary source is the authority.
