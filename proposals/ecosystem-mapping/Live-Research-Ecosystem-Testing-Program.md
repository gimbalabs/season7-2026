# Gimbalabs Product Research; Direction to Self-Sustainability

**Status:** Draft  
**Funding requested:** 9,500 ADA  
**Duration:** 7 weeks  
**Tracks:** Layer 2 (Thursday); DeFi (Wednesday); joint AI meeting (week 7)

## Gimbalabs Primary Driver

To provide open, replicable safe spaces to learn, to explore, and to empower individuals and organizations anywhere so that we can solve meaningful problems.

Gimbalabs funds experiments, not just activities. This program must leave evidence, reusable notes and code, and a working product that can be submitted next.

## Proposal Driver

### Current Situation

The goal is to find what people need. The first direction comes from the Cardano Foundation’s [2025 State of the Developer Ecosystem survey](https://cardano-foundation.github.io/state-of-the-developer-ecosystem/2025/#which-category-of-cardano-decentralized-applications-dapps-are-you-currently-working-on-or-most-interested-in). Developers named identity and authentication as the dApp category they are working on or most interested in, then DeFi and stablecoins, then core infrastructure. The Foundation’s [results write-up](https://cardanofoundation.org/blog/2025-developer-ecosystem-survey-results) records the same order.

Cardano builders often discuss Layer 2 designs, bridges, oracles, and DeFi tools before those tools are tested for cost, speed, trust, and failure. Project Catalyst’s recent themes — stablecoins, programmable tokens, oracles, and verifiable identity — are useful starting points, not a build list. The survey decides where to look first. The sessions then test what already exists.

In addition, to the funding and sustainability of Gimbalabs, The next Project Catalyst round may not have an ecosystem or general category with what we witnessed with the pilot phase. Also a research pitch without a working product would have nowhere clear to go.


### Effects

Gimbalabs would miss the round, or submit an idea that has not been tested against products that already exist.

### Need

Test the products listed below, then finish with a prototype product minimum of test running on preprod. The ask is **9,500 ADA** over 7 weeks. That is 9,000 ADA for the work, plus 500 ADA for project-lead coordination.

## Proposal

### 1. Title or Brief Description

**Gimbalabs Product Research Direction to Self-Sustainability**

Twelve test sessions in six weeks, two per week. Wednesday is DeFi. Thursday is Layer 2. Week 7 is one joint meeting. The output is tested products and working builds for the next Catalyst round.

### 2. Background or Rationale

Test first. Build second. The first direction is the Cardano Foundation survey: identity and authentication, then DeFi and stablecoins, then core infrastructure. The categories below are the test list, not seven products Gimbalabs must invent.

**Thursday — Layer 2.**

- **Problem.** Hydra still asks users to run a node, stay online, and coordinate in a fixed group.
- **Question.** Can we keep Hydra’s transaction and settlement model, and still let clients come and go?
- **Hypothesis.** Hydra can keep Cardano settlement. A shared operator layer and clients who are not always online cover the rest.
- **Conclusion.** Week 5 states the conclusion from the tests. It is not chosen in advance. It may be a payment channel, a bridge, an oracle, another small product.
- **Proposed solution.** Week 6 decision and practicality, the product named in that conclusion.

**Wednesday — DeFi.** Project Catalyst Pilot 2026 is the reason these four areas are the starting list: identity and verifiable credentials, stablecoins, programmable tokens, and oracles. That list is a hypothesis about what the ecosystem needs. It is not a plan to build four products.

- **Problem.** Cardano already has tools in these areas, and some projects have stalled. It is not clear what a developer or user still cannot do easily.
- **Question.** What remains hard despite existing tools, and is that gap large enough to justify another product?
- **Hypothesis.** Comparing a working Cardano tool with a working tool from another ecosystem will show the gap, if there is one.
- **Conclusion.** Week 5 ranks the gaps, including closed projects. Week 6 names one product, or no build.
- **Proposed solution.** One small proof of concept, only if the tests support it. One person can run this track. Three is the maximum.

Rules:

1. Test every product on the lists before starting a build.
2. Week 6 and onward delivers a working project that can be used to rise funds to continue building, give announcements let people test or show interests.
3. Publish notes, code, setup steps, and recordings.


### 3. Intended Outcome

After 7 weeks:

- Every product listed below has been tested in a session.
- One Layer 2 product chosen from the week-6 onward evidence.
- One DeFi proof of concept chosen in week 6, or a written decision not to build.
- Notes from the week-7 meeting on what was built and how AI can help in blockchain.
- A public reason for each build that was kept or dropped.

### 4. Details of the Proposal

Each session: name one Cardano problem, find the products for that week, test them, record speed, cost, setup, trust, and limits, then publish whether a prototype is justified. The list below is the plan, not a claim that every feature exists. Week 1 can replace a product that cannot be tested.

The livestream is the public part. Research, brainstorming, coding, testing, and writing happen between sessions. The budget pays for that work.

Test every product in that week’s row before starting a build. Wednesday is DeFi. Thursday is Layer 2.

#### Track A — Thursday, Layer 2

A tool is in the test only if we can run a real local network, read the code, stop nodes on purpose, and reuse an idea in a Cardano prototype. Hydra stays the baseline. [Core Lightning](https://github.com/ElementsProject/lightning), [CometBFT](https://github.com/cometbft/cometbft), and the [OP Stack](https://github.com/ethereum-optimism/optimism) answer three different questions. They are not three candidates for the same product.

| Week | Session | What we test | Question | Output |
| --- | --- | --- | --- | --- |
| 1 | Hydra baseline | [Hydra](https://github.com/cardano-scaling/hydra), plus a read of the Tail design | How does Hydra work with Cardano L1, and is Tail mature enough to deploy? | A note on setup, settlement, and Tail’s maturity. Tail is not given its own deploy session unless that note says it is ready. |
| 2 | Asynchronous payment channels | Core Lightning | Can a client pay without running its own node? | Payment success, reconnect time, routing failures, and what happens when the channel operator is offline. |
| 3 | Distributed consensus | CometBFT | Can independent operators agree, and survive some of them going offline? | Finality time, throughput as validators are added, failures tolerated, and recovery. Progress still needs more than two-thirds of voting power online. |
| 4 | Shared execution | OP Stack | Can many clients share one execution network and talk to it by RPC? | Transactions per second, confirmation time, load from many clients, sequencer downtime, and L1 settlement time. The usual sequencer is not decentralized. |
| 5 | Product choice | Weeks 1–4, plus Hydrozoa, Gummiworm, and Strike Node | What gap did the tests actually show? | One written choice. See the decision below. |
| 6 | Build | The week-5 choice, with Hydra as the baseline | Can that product run on preprod? | A working prototype, or a public decision not to build. |

**Week 6 decision**

1. Name the gap the tests showed: discovery, uptime, agreement, throughput, cross-Head coordination, or something else.
2. Compare at least two existing implementations. Say whether the gap can be filled by reuse, or needs a new piece.
3. Pick the smallest product that closes that gap and can be tested.

Possible results, only if the evidence points there:

- A Hydra network that is easier to join.
- A shared operator-discovery service.
- A cross-Head payment or coordination layer.
- A bridge or an oracle.
- No build.

A bridge or an oracle is not chosen because it was on a list. The result that matters is:

- More users.
- Less work per user.
- Measured throughput.
- Safe operation when some participants disconnect.

A higher transaction count by itself is not the result.

#### Track B — Wednesday, DeFi

Each session runs a working demo, reads the implementation, compares at least one alternative, writes down what fails, and says whether Cardano should reuse it, integrate it, or build something smaller. Eight products are tested so a week is a comparison, not a single demo.

| Week | Area | What we test | Question | Output |
| --- | --- | --- | --- | --- |
| 1 | Identity and verifiable credentials | Veridian Wallet; Ethereum Attestation Service | Can an organisation issue a credential that another app can check, without putting personal documents on-chain? | One issued credential, one check in a second app, the trust model, and the integration effort. Veridian is the first identity case. It does not cover the whole category. It uses KERI and ACDC. |
| 2 | Stablecoins | USDM; USDCx; Circle CCTP on a route it actually supports | Is the gap the coin, or the path from a bank or exchange onto Cardano and back? | Steps, fees, time, wallets, and trust for each path. USDM and USDCx are different designs. Check CCTP’s supported-chain list before treating Cardano as included. Also note how DJED and iUSD differ. They are not the same kind of dollar asset. |
| 3 | Programmable tokens | CIP-0113; ERC-3643 / T-REX | Which issuer controls are useful, and how hard is a full Cardano integration? | The same cases on both: allowed transfer, blocked transfer, freeze, pause, recovery, and admin changes. Test the current CIP-0113 implementation. |
| 4 | Oracles | Pyth; CHARLI3 | Is a pull-based price easier or cheaper for a Cardano app than a feed pushed on-chain? | Freshness, verification, cost, and what the app does when the price is stale or missing. CHARLI3 has both a push and a pull design. Confirm which feeds are available before the benchmark. |
| 5 | Failures and missing pieces | The weakest results from weeks 1–4; Ardana; Spectrum Finance | Which failures were technical, and which were funding, liquidity, distribution, or rules? | A ranked list of gaps. Ardana stopped in November 2022. Spectrum Finance closed in August 2025. These are postmortems, not live demos, unless the code still runs. |
| 6 | Choose one direction | The week-5 ranking | Is one small capability worth a proof of concept? | One working proof of concept, or a written decision not to build. |

Every product is recorded on the same sheet: setup time, what it actually does, steps for another app to use it, failure and recovery, who can issue or freeze or verify, fees, maintenance, the Cardano gap, and a verdict. The verdict is one of: reuse, integrate, contribute, build an adapter, prototype a missing piece, or do nothing.

Week 7 is not a test session. Both teams meet, share what was tested and built, and discuss how AI can help in blockchain.

**A prototype must include** a named problem, a comparison with at least two tested products, a test someone else can run, a threat model and known limits, measurements where they apply, an open repository, setup steps, and a short roadmap. The week-6 result must run on preprod. That is the condition for the final payment.

**Out of scope:** a full security audit, a production bridge, liquidity provision, token rewards.

**Treasury return.** If the community accepts this term, every later funding round a project from this program wins returns **10% of that new funding** to the Gimbalabs treasury.

### 5. Impact and Benefits

- Gimbalabs contributors get working products they can maintain after a long time, worth mentioning that Andamio is currently doing this.
- Independent Funding source to the Gimabalbs treasury without direct external grants.

### 6. Evaluation Criteria

Views are not the success test. The program succeeds if:

- Every product on the lists above was tested, and the notes are public.
- The week-6 products can work in production, or the report says why a build was dropped.
- The products are concrete enough to submit in the next Catalyst round.
- The week-7 note on AI and blockchain is public.

A “do not build” result can close a category. It does not unlock the week-6 payment.

### 7. Timeline

Six test weeks, then one joint week. **Wednesday: DeFi. Thursday: Layer 2.** Week 7 is both teams together. No extra budget for week 7.

| Week | Wednesday — DeFi | Thursday — Layer 2 | Pay |
| --- | --- | --- | --- |
| 1 | Veridian and Ethereum Attestation Service | Hydra, and a Tail review | Medium |
| 2 | USDM, USDCx, and Circle CCTP | Core Lightning | Research, equal |
| 3 | CIP-0113 and ERC-3643 | CometBFT | Research, equal |
| 4 | Pyth and CHARLI3 | OP Stack | Research, equal |
| 5 | Failures and ranked gaps | Choose the Layer 2 product | Research, equal |
| 6 onward | Build the chosen DeFi proof, or publish no-build | Build the chosen Layer 2 product | Paid after building cand demo launch with announcement to community |
| 7 | Both teams meet. Share what was tested and built. Discuss how AI can help in blockchain. | | No separate pay |

### 8. Resources Required

The request is **9,500 ADA**. At **$0.22 per ADA**, that is **$2,090**.

| | ADA | USD |
| --- | ---: | ---: |
| DeFi pool | 5,400 | $1,188 |
| Layer 2 pool | 3,600 | $792 |
| Project-lead coordination | 500 | $110 |
| **Total** | **9,500** | **$2,090** |

DeFi has three people because the track covers several product types. Layer 2 has two people because the track is one specific infrastructure question. Each of the five people receives the same **1,800 ADA** for the work. The 500 ADA coordination payment is extra, and it is not taken from either pool.

| Pool | People | ADA | Pays |
| --- | ---: | ---: | --- |
| DeFi | 3 | 5,400 | Wednesday tests and the week-6 DeFi product |
| Layer 2 | 2 | 3,600 | Thursday tests and the week-6 Layer 2 prototype |
| Project lead | | 500 | Coordination and supervision |
| **Total** | **5** | **9,500** | |

| Person | Role | ADA |
| --- | --- | ---: |
| Emmanuel | Layer 2 | 1,800 |
| One open nominee | Layer 2 | 1,800 |
| Ahmed | DeFi | 1,800 |
| Jethro | DeFi | 1,800 |
| One open nominee | DeFi | 1,800 |
| Emmanuel | Coordination and supervision | 500 |
| **Paid** | | **9,500** |

Ahmed and Jethro are nominated for DeFi. One DeFi seat is open. Emmanuel is nominated for Layer 2 and is the project lead. One Layer 2 seat is open.

| Week | DeFi | Layer 2 | Both | Why |
| --- | ---: | ---: | ---: | --- |
| 1 | 900 | 600 | 1,500 | First sessions. Medium. |
| 2 | 600 | 400 | 1,000 | Research. |
| 3 | 600 | 400 | 1,000 | Research. |
| 4 | 600 | 400 | 1,000 | Research. |
| 5 | 600 | 400 | 1,000 | Research. |
| 6 onward | 2,100 | 1,400 | 3,500 | Building. Paid from the start of the build through the building work. |
| 7 | 0 | 0 | 0 | Joint AI meeting. |
| **Total** | **5,400** | **3,600** | **9,000** | |

### 9. Responsibilities

**Layer 2** is Emmanuel and one open nominee. Two people, because that track stays on one infrastructure question.

**DeFi** is Ahmed, Jethro, and one open nominee. Three people, because that track tests several kinds of products.

**Emmanuel** is the project lead. responsible for success, coordination and supervision.

Both teams attend week 7. **Gimbalabs** accepts each week’s output before that week’s payment. Attendance is not acceptance.

### 10. Potential Risks and Mitigation Strategies

| Risk | Mitigation |
| --- | --- |
| Sessions skip products and jump to a build. | A category is not built until its listed products are tested. |
| The Catalyst submission is still a generic pitch. | Week 6 must leave a working product, not a research topic. |
| Week 6 and beyond claims a product that cannot run in production. | The highest payment stays unreleased. |
| Tests create security or cost risk. | Keep tests small. No production bridge, liquidity provision, or full audit in this budget. |

### 11. Review and Adaptation Plan

Review each week in Open Spaces. If a listed product cannot be tested, replace it in writing before the next session. Week 7 records what was built, what was dropped, and whether the products are ready to submit to Catalyst.

### 12. Licensing and Intellectual Property

Notes, recordings, and new code from this funding are public. New code uses an open-source license agreed with Gimbalabs before the repository is created. Licenses of products under test still apply.

---

## Consent Process

### Objections Raised

_Record any objections raised during the consent period, along with how they were addressed._

### Resolution Notes

_Document how the proposal was modified to address objections, or why objections were considered invalid._

### Final Decision

_Record the final outcome: Approved, Withdrawn, or Rejected. Include the date and brief reasoning._

---

## Discussion Notes

_Optional: Capture key points from discussions during Open Spaces or Discord._
