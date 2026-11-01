# Contract Risk Report — TechVendor Ltd. (input/sample_contract.txt)

## Risk Rating
**High** — Section 4.2 irrevocably assigns all Customer Data, including derivative works and insights, to Vendor for perpetual use, which is a P1 unilateral data assignment (Section 6.2 uncapped Customer liability and the 7-day non-renewal notice in Section 2.2 are also P1).

### Critical Summary
The most dangerous clause is Section 4.2, which irrevocably assigns all Customer Data and derivative works to Vendor for perpetual use, including commercial offerings to third parties, and survives termination. The most important customer obligation is Section 6.2 read with 6.3, under which Customer's liability to Vendor is unlimited and Customer must indemnify Vendor for all claims arising from its use of the Services, while Vendor's liability is capped at one month's fees under 6.1. Before signing, strike or substantially narrow Section 4.2, make the liability cap in Section 6 mutual, and consider lengthening the 7-day non-renewal notice period in Section 2.2.

## P1 Critical Clauses
| Clause type | Excerpt | Risk explanation |
|---|---|---|
| Auto-renewal without adequate notice | "shall automatically renew for successive twenty-four (24) month periods (each a "Renewal Term") unless Customer provides written notice of non-renewal to Vendor at least seven (7) days prior" | Renewal is automatic for another 24 months. Customer has only 7 days before term end to give non-renewal notice, and late notice "shall be of no effect." |
| Uncapped liability (Customer side) | "Customer's liability to Vendor arising out of or related to this Agreement, including under Section 6.3, shall be unlimited" | Customer's liability has no cap, exclusion, or limitation of any kind, and it extends to the Section 6.3 indemnity. |
| Asymmetric liability cap (Vendor side) | "Vendor's aggregate liability to Customer under this Agreement shall be limited to the fees paid by Customer in the preceding one (1) month" | Vendor's liability is capped at one month of fees, and Vendor is excluded from indirect and consequential damages. Customer's recovery is limited while its own exposure is unlimited. |
| Unilateral IP or data assignment to vendor | "Customer hereby irrevocably assigns to Vendor all right, title, and interest in and to all Customer Data, including all derivative works and insights" | Customer irrevocably assigns ownership of its data and derivatives to Vendor. The assignment is one-way, requires no Vendor obligation in return, and permits use in commercial offerings to third parties. |
| Perpetual data retention and use | "Vendor may retain and use Customer Data perpetually, including after termination of this Agreement." | Vendor keeps and uses Customer Data indefinitely, including after the contract ends. The contract contains no deletion or return obligation. |
| Punitive penalties | — | None found |

## P2 Major Clauses
| Clause type | Excerpt | Risk explanation |
|---|---|---|
| Broad indemnification | "Customer shall indemnify and hold harmless Vendor against all claims, losses, damages, and expenses (including legal fees) arising from Customer's use of the Services." | Customer's indemnity covers all claims, losses, and legal fees arising from its use of the Services, with no fault qualifier or cap. The contract gives Customer no reciprocal indemnity from Vendor. |
| Price escalation trigger | "Vendor may increase the fees at any time, effective on each anniversary of the Effective Date, by up to fifteen percent (15%) per year." | Fees can rise up to 15% per year. Section 3.2 states that no Customer consent or approval is required. "At any time" conflicts with the anniversary-date effective timing, which creates ambiguity about when increases take effect. |
| Customer data ownership ambiguity | "including all derivative works and insights, for Vendor's use in analytics, product development, benchmarking" | The contract does not define "derivative works and insights." Section 4.1 defines Customer Data as data submitted to the Services, so the scope of what transfers under Section 4.2 is unclear. |
| Exclusivity | — | None found |

## P3 Minor Clauses
| Clause type | Excerpt | Risk explanation |
|---|---|---|
| Termination for convenience timeline | "Customer may terminate this Agreement for convenience upon thirty (30) days' prior written notice to Vendor." | Customer can terminate for convenience on 30 days' notice. Section 8.2 also states that no refund of prepaid fees is due on such termination, although fees are invoiced annually in advance under Section 3.1. |
| Termination for material breach (cure period) | "Either party may terminate this Agreement for material breach if the breach remains uncured thirty (30) days after written notice." | Either party may terminate for material breach after a 30-day cure period that runs from written notice. |
| Confidentiality duration | "Each party shall protect the other's Confidential Information with reasonable care for three (3) years after termination." | Confidentiality obligations end three years after termination. The contract does not address how Customer Data is treated after that period, and Section 4.2 separately allows perpetual use. |
| Governing law | "This Agreement shall be governed by and construed in accordance with the laws of the State of Delaware, United States, without regard to its conflict of laws principles." | Delaware law governs, excluding conflict-of-laws rules. Vendor is located in the United Kingdom, so cross-border enforcement questions are not addressed in the contract. |
| Dispute resolution forum | "The state and federal courts located in Wilmington, Delaware shall have exclusive jurisdiction over any dispute arising under this Agreement." | Exclusive jurisdiction is in Wilmington, Delaware courts. No arbitration or alternative dispute mechanism is provided. Vendor is located in London, so litigation there may be costly. |

## Key Obligations

### Acme Corp (Customer)
- Pay the annual subscription fee of USD 180,000, invoiced annually in advance, with invoices due within thirty (30) days of receipt (Section 3.1).
- Give written notice of non-renewal to TechVendor Ltd. at least seven (7) days before the end of the then-current term, or the Agreement automatically renews for a 24-month Renewal Term (Section 2.2).
- Irrevocably assign to TechVendor Ltd. all right, title, and interest in all Customer Data, including derivative works and insights (Section 4.2).
- Indemnify and hold harmless TechVendor Ltd. against all claims, losses, damages, and expenses, including legal fees, arising from Acme Corp's use of the Services (Section 6.3).
- Bear liability to TechVendor Ltd. that is unlimited and not subject to any cap, exclusion, or limitation, including liability under Section 6.3 (Section 6.2).
- Protect TechVendor Ltd.'s Confidential Information with reasonable care for three (3) years after termination (Section 7).
- Give thirty (30) days' prior written notice to terminate for convenience; no refund of prepaid fees is due upon such termination (Section 8.2).
- Make any amendment to the Agreement in writing and signed by both parties (Section 10).

### TechVendor Ltd. (Vendor)
- Provide Acme Corp with access to its cloud-based workflow automation platform (the "Services") in accordance with the service descriptions in Exhibit A (Section 1).
- Notify Acme Corp of any fee increase (Section 3.2).
- Protect Acme Corp's Confidential Information with reasonable care for three (3) years after termination (Section 7).
- Aggregate liability to Acme Corp is limited to the fees paid by Acme Corp in the preceding one (1) month, and TechVendor Ltd. is not liable for indirect, incidental, special, or consequential damages (Section 6.1).
- Make any amendment to the Agreement in writing and signed by both parties (Section 10).

## Run Info
- Input file: input/sample_contract.txt
- Date: 2026-11-01
- Model: coordinator — sonnet (claude-sonnet-5-5); sub-agents — haiku
- Sub-agents used: clause-agent, obligation-agent, risk-agent (run in parallel)

---
GATE: FAIL
