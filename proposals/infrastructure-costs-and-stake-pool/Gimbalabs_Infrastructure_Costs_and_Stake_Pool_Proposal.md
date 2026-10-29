# Gimbalabs Infrastructure Costs and Stake Pool

**Proposed by:** James Dunseith
**Status:** Draft

## Gimbalabs Primary Driver

> To provide open, replicable safe spaces to learn, to explore, and to empower individuals and organizations anywhere so that we can solve meaningful problems.

## Proposal Driver

### Current Situation

Several Gimbalabs services bill to James's personal card: hosting for the GMBL stake pool, front-end hosting, domains, DNS, Meetup, Miro and TeamUp. James has paid these for months. The stake pool moved from Scaleway to Google Cloud in October and now runs on Dingo. It costs about the same as before. The pool earns rewards, which are small for now, and James controls both the rewards wallet and the pledge.

### Effects

Gimbalabs has no record of what its infrastructure costs or who pays for it. We haven't yet decided which services are still needed. The pool's rewards have no agreed use, and its wallet and pledge sit with one person.

### Need

Gimbalabs needs to reimburse what James has paid, decide which services to keep, and decide what to do with the stake pool and its rewards.

---

## Proposal

### 1. Title or Brief Description

**Gimbalabs Infrastructure Costs and Stake Pool**

### 2. Background or Rationale

The Admin Operations and Maintenance Budget (season7-2026 issue 5) gives the Admins $5,000 (26,000 ADA) for September 2026 to February 2027. It covers hosting, domains, subscriptions and reasonable reimbursements. The costs in this proposal are larger than that budget. Scaleway alone was about $450 a month, and the pool's new hosting costs about the same. So this proposal asks for them separately rather than drawing on the Admin budget.

The pool's return to the pool list on Dingo was announced at Open Space on 2026-10-22.

### 3. Intended Outcome

- James is reimbursed for Gimbalabs costs he has paid.
- Each recurring service has a keep or drop decision.
- The stake pool has a decision on whether it keeps running, what its rewards are for, and who controls its wallet and pledge.

### 4. Details of the Proposal

#### A. Reimbursement

Repay **$4,834.86** for the charges below.

**Hosting, May to October 2026**

Scaleway hosted the GMBL stake pool (gimbal-stakepool) and the Dandelion GraphQL preprod instance (dandelion-graphql-preprod). Both are now shut down on Scaleway: the pool moved to Google Cloud, and Dandelion GraphQL preprod was retired. One final Scaleway bill is still to come.

| Month | Scaleway | Vercel | Google Cloud |
|---|--:|--:|--:|
| May | $437.89 | $41.25 | $10.64 |
| June | $448.79 | $41.25 | $10.91 |
| July | $445.20 | $41.26 | $10.66 |
| August | $464.38 | $41.26 | $10.59 |
| September | $467.36 | $41.26 | $11.31 |
| October | $441.26 | $41.26 | $10.57 |
| **Total** | **$2,704.88** | **$247.54** | **$64.68** |

**Other Gimbalabs charges**

| Charge | Date | Amount |
|---|---|--:|
| Namecheap, plutuspbl.io | 01-20 | $66.98 |
| Cloudflare (annual) | 02-01 | $240.00 |
| Namecheap, midnightpbl.io | 03-24 | $34.98 |
| Meetup Pro (6 months) | 04-26 | $190.18 |
| Miro (annual) | 04-26 | $204.00 |
| Zoom | 05-03 | $36.10 |
| TeamUp Pro (annual) | 09-01 | $360.00 |
| Namecheap, gimbalabs.io and gimbalabs.com renewals | 09-15 | $94.66 |
| Namecheap Private Email, gimbalabs.io (13 mailboxes) | 09-17 | $300.68 |
| Google Cloud | 10-13 | $100.00 |
| Meetup Pro (6 months) | 10-26 | $190.18 |
| **Total** | | **$1,817.76** |

#### B. Which services we keep

For each service, decide whether we keep it or drop it before its next charge. James keeps paying for the ones we keep.

| Service | What it does | Cost | Next charge | Proposed |
|---|---|--:|---|---|
| Google Cloud, GMBL stake pool | Pool hosting on Dingo | about $450/month | Monthly | Decided in C |
| Google Cloud | Gimbalabs Google accounts and Drive | about $11/month | Monthly | [keep or drop] |
| Vercel | Gimbalabs account; hosts Cardano XP | $41.26/month | Monthly | [keep or drop] |
| Namecheap domains | gimbalabs.io, gimbalabs.com, plutuspbl.io, midnightpbl.io | about $197/year | January, March, September | [keep or drop each] |
| Namecheap Private Email | 13 mailboxes on gimbalabs.io | $300.68/year | September 2027 | [keep, or drop unused mailboxes] |
| Cloudflare | DNS | $240/year | February 2027 | [keep or drop] |
| Meetup Pro | Gimbalabs Meetup groups | about $380/year | April 2027 | [keep or drop] |
| Miro | Gimbalabs boards | $204/year | April 2027 | [keep or drop] |
| TeamUp Pro | Shared calendar | $360/year | September 2027 | [keep or drop] |
| Zoom | Meetings | | Stopped billing after May 2026 | Drop. The Admin budget proposes Jitsi instead |

#### C. The stake pool

Three decisions:

1. **Keep the pool running?** It costs about $450 a month to host.
2. **What are the rewards for?** Options include offsetting the pool's own hosting, funding other Gimbalabs costs, funding a program, or holding them.
3. **Who controls the rewards wallet and the pledge?** Today James does. The alternative is a Gimbalabs-controlled wallet.

The pool keys were rotated during the migration. The next rotation is due around the end of December 2026.

### 5. Impact and Benefits

- Gimbalabs gets a full record of what its infrastructure costs.
- Services nobody uses stop costing money.
- The pool's rewards get a purpose, and its control no longer rests on one person by default.

### 6. Evaluation Criteria

- James is repaid.
- Every service in B has a decision, and dropped services stop billing.
- The pool has decisions on all three questions in C.
- At the review: what the pool earned against what it cost.

### 7. Timeline

- Present at Open Space: 2026-10-29
- Reimbursement paid: within 30 days of consent
- Dropped services cancelled before their next charge
- Review: three months after consent

### 8. Resources Required

- **One-time:** $4,834.86 reimbursement (about 24,200 ADA at the Admin budget's rate of $0.20 per ADA).
- **Ongoing, if everything is kept:** about $640 a month, nearly all of it the pool's hosting. James pays, so the ongoing cost needs no new funds now. It is listed so the community can see it.

### 9. Responsibilities

- **James:** pays the kept services, cancels the dropped ones, runs the pool and rotates its keys.
- **Admins:** pay the reimbursement and record it.
- **Community:** decides B and C through the consent process.

### 10. Potential Risks and Mitigation Strategies

| Risk                                                      | Mitigation                                                                                                          |
| --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| The pool costs more than it earns.                        | Review the numbers at the three-month review. Dropping the pool is an option.                                       |
| One person controls the pool's wallet and pledge.         | Decision C3 settles who holds them.                                                                                 |
| A dropped service turns out to be needed.                 | Most are monthly or annual and can be restarted. Domains are the exception: check each one before letting it lapse. |

### 11. Review and Adaptation Plan

Review after three months: what each service cost, what the pool earned, and whether James should keep paying.

**A follow-up proposal.** James paying Gimbalabs costs on a personal card works for now, but it isn't a lasting arrangement. A follow-up proposal could set a standing way to handle Gimbalabs expenses: a Gimbalabs payment method, a regular repayment schedule, or a budget per service. This proposal doesn't decide that.

### 12. Licensing and Intellectual Property

Not applicable. This proposal creates no software or content.

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