# Data Governance in AI, FinTech and LegalTech — Joseph Lee and Aline Darbellay (eds.)
**Format**: Markdown extraction | **Sections**: 8 | **Depth**: study | **Coverage**: prioritized Chapters 1, 2, 4, 5, 6, 9, 10, and 11

## Mental Model (read first)
Financial data is simultaneously an input to decisions, a regulated record, a source of market power, an object of control claims, and critical infrastructure. “Who owns the data?” is usually too crude. Map the data lifecycle and assign lawful basis, access, quality, provenance, decision responsibility, security, sharing, retention, auditability, and redress at each stage.

## Frameworks & Structure

### 1. Financial-data governance foundations
- Build a lifecycle map: collection/generation → classification → validation → storage → combination/inference → access/use → sharing/transfer → automated decision → retention/deletion → incident and redress.
- For each dataset identify data subject/source, controller or equivalent decision-maker, processor/service provider, users, technical custodian, regulator, contractual rights, and affected persons.
- Governance objectives can conflict: privacy, integrity, availability, utility, competition, innovation, explainability, market transparency, security, and property/control.
- **Anti-pattern — compliance silo**: treating privacy notice, cybersecurity, model governance, and commercial licensing as separate projects despite one data flow.

### 2. Cryptocurrency data utility and governance
- Distributed ledgers combine public or shared transaction data, pseudonymous identifiers, protocol rules, analytics, private keys, off-chain services, and governance actors.
- Identify what is on-chain/off-chain, immutable/editable, personal/non-personal, observable/linkable, and controlled by miners/validators, developers, exchanges, wallet providers, analytics firms, and users.
- Immutability can conflict with correction/erasure; pseudonymity does not guarantee anonymity. Analyze re-identification, chain analytics, fork/governance changes, key loss, and jurisdiction.

### 3. Broken informed consent
- In big-data finance, consent may be formally obtained yet substantively weak because information is complex, future uses are unpredictable, bargaining power is unequal, and refusal may exclude the customer.
- Test whether consent is specific, informed, freely given, granular, revocable, and matched to actual downstream processing. Distinguish consent from other lawful bases rather than forcing all processing through a fictional choice.
- Use layered notices, purpose limitation, minimization, defaults, just-in-time explanation, withdrawal operations, and independent accountability to reduce—but not magically cure—the information asymmetry.

### 4. Platform conflicts of interest
- **Algorithm-driven information gatekeepers** influence visibility, matching, pricing, advice, or access while pursuing platform revenue and affiliated interests.
- Map conflict source: payment for placement/order flow, self-preferencing, cross-use of client data, steering, discriminatory access, opaque ranking, bundling, or exploitation of informational advantage.
- Controls include conflict inventory, separation, disclosure that is decision-useful, ranking governance, audit logs, outcome testing, user controls, independent review, and prohibitions where mitigation cannot work.

### 5. Property and data
- Data does not fit a single property category. Separate facts/information, database rights, copyright, confidentiality, trade secrets, privacy/personality interests, contractual access, possession/control, and technical exclusion.
- A claim to “ownership” must specify the entitlement sought: access, use, copy, exclude, transfer, license, monetize, correct, delete, port, or recover on insolvency.
- Contract can allocate rights inter partes but may not override data-protection duties, third-party rights, competition law, regulatory access, or public policy.

### 6. AI-related board duties and liability
- Boards must establish oversight proportionate to AI’s strategic and risk significance: competence, accountability, risk appetite, data/model governance, validation, monitoring, incident escalation, third-party oversight, and records.
- Liability analysis separates company, director/officer, developer/vendor, deployer, employee, and regulated-person conduct; duty, standard of care, delegation, causation, loss, defense, and insurance must be tested under applicable law.
- “Human in the loop” is meaningful only if the person has time, information, competence, authority, and a non-punitive ability to override.

### 7. Market-infrastructure data
- Exchanges, trading venues, CCPs, CSDs, and data vendors produce and commercialize market data while performing regulated functions.
- Analyze data quality, timeliness, consolidation, pricing, access, non-discrimination, intellectual-property/licensing claims, conflicts between commercial revenue and public-market function, and AI use by investors.
- Poor or unequal market data affects price discovery, best execution, surveillance, competition, and model outcomes.

### 8. Cybersecurity certification and compliance
- Certification can evidence conformity but is not security itself. Define scope, assurance level, control baseline, assessor independence, sampling, renewal, change control, supply-chain coverage, and incident implications.
- Operate a cycle: identify assets/data and threats → protect → detect → respond → recover → learn. Connect legal reporting deadlines, customer/regulator communication, evidence preservation, business continuity, and vendor obligations.
- **Anti-pattern — badge reliance**: treating certification or contractual warranty as proof that operational controls work continuously.

### 9. Integrated governance artifacts
- Maintain a data inventory/lineage map, processing and sharing register, legal-basis matrix, access model, retention schedule, model inventory/cards, vendor register, incident playbooks, conflict register, board reporting, and decision logs.
- Use metrics that expose outcomes: data-quality exceptions, overrides, drift, disparate effects, unauthorized access, unresolved vulnerabilities, vendor concentration, complaint themes, and remediation aging.

## Worked Example
A payment platform uses transaction data to train an AI fraud model and offer merchant credit. Trace raw payment data, device/behavioral data, inferred fraud labels, model features, credit outputs, data shared with cloud/model vendors, and market-infrastructure feeds. For each flow record purpose, lawful basis, notice/consent status, access, retention, transfer jurisdiction, security, property/license claims, and regulatory use. Separately assess platform conflicts: the platform may rank merchants, price credit, and favor its own services using privileged data. The board approves risk appetite and accountability; validation tests drift and disparate effects; incident and customer-redress routes are operational before launch.

## Decision Rules & Judgment
- When someone claims to own data, ask which precise entitlement and against whom.
- When relying on consent, test real choice and downstream use, not merely a clicked box.
- When a platform both intermediates and competes, presume a conflict inventory is required.
- When AI affects financial access or markets, require traceable data lineage, validation, monitoring, override, and redress.
- When relying on certification, verify scope and current operational evidence.
- Treat jurisdiction examples as examples; verify current applicable privacy, AI, cyber, financial, and competition law.

## Key Takeaways
1. Govern data across its lifecycle and institutional ecosystem.
2. Privacy, property, competition, fiduciary/governance, and cybersecurity questions overlap but are not interchangeable.
3. AI accountability depends on decision rights and evidence, not generic ethics statements.
4. Financial-market data has both commercial value and public-infrastructure significance.
