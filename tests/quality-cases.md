# Semantic Quality Cases

These cases are review tests for the method. They are deliberately small and contextual rather than automated.

## Case 1 — application name

**Candidate:** `Salesforce`

**Expected:** reject.

**Why:** product/application, not an enduring business ability.

**Possible underlying capabilities:** Customer Management, Opportunity Management, Customer Interaction Management — subject to business evidence.

---

## Case 2 — team name

**Candidate:** `Fleet Operations Team`

**Expected:** revise.

**Why:** organisation structure.

**Possible capability:** Fleet Management or Fleet Operations, depending on scope and evidence.

---

## Case 3 — workflow step

**Candidate:** `Approve Rental Extension`

**Expected:** remove as peer capability or place under a broader capability.

**Why:** activity/process step.

**Possible parent ability:** Rental Agreement Management.

---

## Case 4 — temporary programme

**Candidate:** `Digital Customer Programme`

**Expected:** reject.

**Why:** temporary change initiative.

**Question:** which enduring customer abilities is the programme changing?

---

## Case 5 — enduring ability

**Candidate:** `Supplier Management`

**Definition:** The ability to establish, govern and maintain supplier relationships so external goods and services meet business, commercial and operational requirements.

**Expected:** likely accept, subject to model scope.

**Why:** enduring, implementation-independent and business-meaningful.

---

## Case 6 — weak definition

**Candidate:** `Contract Management`

**Definition:** The ability to manage contracts.

**Expected:** revise definition.

**Why:** tautology; does not establish purpose or boundary.

---

## Case 7 — mixed granularity

**Sibling candidates:**

- Customer Management
- Send Welcome Email
- Revenue Management
- Enterprise Management

**Expected:** revise hierarchy/granularity.

**Why:** one process step and one very broad umbrella sit beside domain-level capabilities.

---

## Case 8 — location

**Candidate:** `Sydney Fulfilment`

**Expected:** revise.

**Why:** the location can change independently of the business ability.

**Possible capability:** Fulfilment Management, with Sydney mapped as an operating location.

---

## Case 9 — ambiguous but potentially valid

**Candidate:** `Customer Account Management`

**Expected:** needs context.

**Why:** it may be a genuine enduring ability, a team name, or a sales process depending on the organisation.

**Required action:** define purpose, scope and boundaries before accepting.

---

## Case 10 — AI inference without evidence

**Input evidence:** company rents equipment and performs maintenance.

**Generated candidate:** `Loyalty Programme Management`

**Expected:** mark as unsupported / needs evidence.

**Why:** plausible industry knowledge is not evidence that this organisation requires or performs the capability.

## Completion test

A reviewer using this method should be able to explain not only whether each candidate passes, but **why** it passes or fails and what architectural view the failed item actually belongs to.
