# SRP-013: Cognitive Warfare As A Service

## The Private Military Model for Information Operations

**Classification:** OPEN DISTRIBUTION
**Series:** Seithar Research Papers
**Date:** 19 February 2026
**Version:** 1.0

---

## Abstract

The privatization of warfare follows a consistent pattern. Physical security gave rise to Executive Outcomes and Blackwater. Cyber security produced CrowdStrike, Mandiant, and their offensive counterparts: Hacking Team, NSO Group, DarkMatter. Each transition lagged the threat environment by roughly a decade. We are now inside that lag for cognitive warfare. Nation-states have operated organized influence and perception management capabilities since at least 2011. The private sector has no equivalent defensive capacity. This paper defines Cognitive Warfare As A Service (CWaaS), maps it to existing operational frameworks, and establishes the five-tier service model through which Seithar Group delivers these capabilities to contracted clients.

---

## 1. The Arc of Privatized Conflict

Private military companies didn't emerge from theory. They emerged from necessity. When South Africa's apartheid-era military dissolved, its operators didn't vanish. They formed Executive Outcomes and sold their skills on the open market. When the United States needed to scale operations in Iraq beyond what uniformed personnel could sustain, it contracted Blackwater, DynCorp, Triple Canopy. The pattern is straightforward: states develop a warfighting capability, the capability matures, demand outstrips state capacity, and private firms fill the gap.

Cyber warfare followed the same arc with a compressed timeline. The NSA's Tailored Access Operations unit represented state-of-the-art offensive cyber capability through the early 2000s. By 2010, former operators had dispersed into the private sector. Some built defensive firms. Others built offensive ones. Hacking Team sold intrusion tools to governments across four continents. NSO Group's Pegasus became the de facto standard for state-sponsored mobile surveillance. DarkMatter, staffed heavily by former NSA and GCHQ personnel, built the UAE's domestic surveillance architecture under Project Raven.

These firms didn't create demand. They served demand that already existed.

The cognitive domain is following the same trajectory, but the lag is more dangerous. State-level cognitive warfare capabilities have been operational for over a decade. China's PLA Unit 61398 conducts integrated cyber-cognitive operations that blend network intrusion with strategic influence. Russia's Internet Research Agency, before its nominal dissolution, ran industrialized influence campaigns across dozens of countries simultaneously. Britain's JTRIG (Joint Threat Research Intelligence Group) conducted what it internally described as "effects operations," using deception, fabrication, and social manipulation against targets ranging from Anonymous hacktivists to Argentine diplomats during the Falklands sovereignty dispute.

The capability exists. The precedent exists. What doesn't exist is a private sector equivalent that serves organizations outside government. Corporations, institutions, and non-state entities face cognitive threats they cannot see, cannot measure, and cannot counter. They hire PR firms when they need intelligence agencies. They hire crisis communications consultants when they need operational planners. The mismatch is structural, not incidental.

Seithar exists to close that gap.

## 2. Defining Cognitive Warfare

Terminology matters here because confusion about terms creates confusion about capabilities. We distinguish three operational layers that adversaries blend but defenders typically treat in isolation.

**The Cyber Layer** encompasses network intrusion, data exfiltration, infrastructure compromise, and technical surveillance. This is the domain of firewalls, endpoint detection, and incident response. It's well understood, heavily funded, and covered by mature frameworks like MITRE ATT&CK.

**The Influence Layer** encompasses the creation, amplification, and distribution of narratives through media channels, social platforms, and information intermediaries. DISARM (the Disinformation Analysis and Risk Management framework) maps this space, cataloguing techniques from content fabrication to platform manipulation to audience targeting.

**The Cognitive Layer** targets the decision-making processes of individuals and groups. It doesn't just deliver a message; it reshapes the interpretive framework through which messages are received. Social Cybersecurity Theory (SCT) provides the academic foundation here, modeling how information maneuvers alter the cognitive schemas that populations use to process reality.

Most adversary operations span all three layers simultaneously. A typical state-sponsored campaign might compromise a target's email server (cyber), leak selectively edited documents through cultivated media contacts (influence), and time the release to coincide with a decision point where the target's cognitive load is already elevated (cognitive). Defending against any single layer while ignoring the others is like locking the front door while leaving the windows open.

The term "cognitive warfare" encompasses operations across all three layers when they are coordinated to affect perception, decision-making, or behavior. It is not a metaphor. It is a discipline, and it requires disciplined practice.

## 3. The CWaaS Service Model

Seithar's service architecture is organized into five tiers. Each tier builds on the capabilities below it. Clients can engage at any level, though we recommend that new engagements begin no higher than Tier 2 until baseline sensing is established.

### Tier 1: Sensor Grid

**Function:** Persistent monitoring of the client's information environment across platforms, media channels, and dark web sources.

**Deliverable:** Real-time threat feeds, narrative tracking dashboards, anomaly detection alerts.

**Framework Mapping:**
- *MITRE ATT&CK:* Reconnaissance (T1595), Search Open Websites/Domains (T1593), Gather Victim Identity Information (T1589). We monitor for these techniques being applied against the client.
- *DISARM:* Plan Strategy (TA01), Plan Objectives (TA02). Detection of adversary planning indicators before campaigns materialize.
- *SCT:* Baseline cognitive environment mapping. What does the target population believe? What narratives are ambient? Where are the fault lines?

The Sensor Grid is passive collection. It doesn't interact with adversaries or alter the information environment. It watches. Most clients are startled by what the grid reveals in its first thirty days. Threats they assumed were organic turn out to be coordinated. Narratives they thought were grassroots turn out to have traceable origin points. The grid doesn't make judgments. It provides visibility.

### Tier 2: Threat Mapping

**Function:** Analysis and attribution of detected threats. Converts raw sensor data into operational intelligence.

**Deliverable:** Threat actor profiles, campaign reconstruction timelines, vulnerability assessments of client's cognitive attack surface.

**Framework Mapping:**
- *MITRE ATT&CK:* Resource Development (TA0042), Initial Access (TA0001). Identifying adversary infrastructure and entry vectors.
- *DISARM:* Develop Content (TA06), Select Channels and Affordances (TA07). Mapping how adversary narratives are constructed and distributed.
- *SCT:* Schema analysis. Identifying which cognitive frameworks the adversary is attempting to exploit or reshape. Modeling second and third-order effects of ongoing campaigns.

Threat Mapping is where sensing becomes understanding. A Tier 1 client knows something is happening. A Tier 2 client knows who is doing it, why, and what they'll likely do next. Attribution in the cognitive domain is harder than in cyber, where IP addresses and malware signatures provide forensic anchors. Cognitive attribution relies on linguistic analysis, behavioral pattern matching, temporal correlation, and network topology. It's slower. It's also more consequential, because misattribution in the cognitive domain can itself become a weapon.

### Tier 3: Active Defense

**Function:** Countermeasures that degrade adversary campaigns without initiating new offensive operations. Hardening the client's cognitive perimeter.

**Deliverable:** Counter-narrative frameworks, prebunking campaigns, platform-level disruption coordination, inoculation programs for key personnel.

**Framework Mapping:**
- *MITRE ATT&CK:* The MITRE Shield (now MITRE Engage) framework applies here. Specifically: Channel (EAC0005), Lure (EAC0004), and Detect activities that create adversary uncertainty.
- *DISARM:* Counter-techniques across the response framework. Content takedowns, platform reporting, source exposure, narrative disruption.
- *SCT:* Inoculation theory application. Pre-exposing target audiences to weakened forms of adversary narratives to build resistance. Cognitive firewall construction.

Active Defense is the boundary between observation and action. Everything below this tier is collection and analysis. Everything at this tier and above involves shaping the information environment. This is where the dual-use question becomes concrete, and we address it directly in Section 5.

Inoculation deserves specific attention. The principle is borrowed from immunology: expose a population to a weakened form of a manipulation technique, and they develop resistance to the full-strength version. Academic research on prebunking, particularly the work emerging from Cambridge and the University of Bristol, has demonstrated measurable effects. Seithar's implementation goes further. We don't just prebunk individual narratives. We build cognitive resilience against entire classes of manipulation technique. The goal isn't to tell people what to think. It's to make them harder to deceive.

### Tier 4: Persona Operations

**Function:** Deployment of managed personas for intelligence collection, narrative placement, and influence testing within adversary-adjacent information spaces.

**Deliverable:** Persona networks with established credibility in target communities, intelligence collected from closed or semi-closed information environments, influence pathway mapping.

**Framework Mapping:**
- *MITRE ATT&CK:* Establish Accounts (T1585), Develop Capabilities (T1587), Stage Capabilities (T1608). Applied to the information domain rather than the network domain.
- *DISARM:* Develop People-Based Assets (TA15), Create Inauthentic Social Media Pages and Groups (T0007), Develop Owned Media Assets.
- *SCT:* Social identity infiltration. Personas operate within cognitive communities, tracking narrative evolution from the inside rather than observing it from the outside.

This tier requires candor. Persona operations are inherently deceptive. A managed persona is, by definition, not what it claims to be. We don't pretend this is ethically uncomplicated. We do assert that it is operationally necessary. Adversary networks operate in closed spaces. Narratives form and harden before they reach open platforms. By the time a threat is visible to Tier 1 sensors, it's often already in distribution. Persona operations provide the early warning that external sensing cannot.

The ethical framework governing persona deployment is contractual, not aspirational. Section 5 addresses this directly.

### Tier 5: Full Spectrum

**Function:** Integrated cognitive warfare operations combining all lower tiers with offensive capability. Campaign design, execution, and battle damage assessment across the cyber, influence, and cognitive layers.

**Deliverable:** End-to-end campaign management. Strategic communications integration. Cross-domain operations that synchronize cyber effects with influence operations and cognitive targeting.

**Framework Mapping:**
- *MITRE ATT&CK:* Full kill chain application, from Reconnaissance through Impact, adapted to cognitive objectives.
- *DISARM:* Full framework application across all tactical phases.
- *SCT:* Strategic cognitive environment shaping. Altering the foundational schemas through which target populations interpret events. This is not messaging. This is architecture.

Tier 5 engagements are rare. They require sustained commitment from the client, dedicated infrastructure, and operational security practices that most commercial entities find unfamiliar. We do not advertise this tier. Clients who need it know they need it, and they typically approach us after state-level adversaries have already demonstrated what full-spectrum cognitive operations look like when applied against an undefended target.

## 4. Framework Integration

The three frameworks we reference throughout this paper were developed independently for different purposes. MITRE ATT&CK catalogs adversary techniques in the cyber domain. DISARM does the same for influence operations. SCT provides the theoretical underpinning for understanding cognitive effects. None of them alone is sufficient for the operating environment we describe.

Seithar's operational methodology integrates all three into a unified threat model. We call this the Cognitive Kill Chain, though the term is imprecise. Unlike Lockheed Martin's cyber kill chain, which describes a linear progression, cognitive operations are iterative and multi-vectored. An adversary might begin with influence operations, escalate to cyber intrusion to obtain compromising material, and then deploy that material through cognitive targeting that exploits specific psychological vulnerabilities in the decision-maker they're trying to affect.

The integration works as follows:

**Detection** draws primarily on MITRE ATT&CK indicators (for the technical layer) and DISARM indicators (for the influence layer). Anomalies in either domain trigger analysis.

**Analysis** applies SCT models to understand what the adversary is trying to achieve at the cognitive level. Technical and influence indicators are symptoms. The cognitive objective is the disease.

**Response** is planned across all three frameworks simultaneously. A counter-operation might involve technical countermeasures (blocking infrastructure, disrupting command and control), influence countermeasures (counter-narratives, platform coordination), and cognitive countermeasures (inoculation, decision-support for targeted individuals) executed in coordinated sequence.

**Assessment** measures effects across all three layers. Did the adversary's technical infrastructure go dark? Did their narratives lose traction? Did the target population's cognitive resilience increase? These are different metrics requiring different collection methods, but they must be evaluated together to determine whether the response succeeded.

## 5. The Dual-Use Problem

Every capability described in this paper can be used offensively. The Sensor Grid that monitors threats against a client can monitor a client's competitors. Threat Mapping that attributes adversary campaigns can plan them. Active Defense techniques that disrupt hostile narratives can disrupt legitimate ones. Persona Operations that infiltrate adversary networks can infiltrate any network. Full Spectrum operations can be pointed in any direction.

This is not a flaw in the model. It is an inherent property of the domain. A rifle defends and attacks. A firewall can be reverse-engineered into an exploitation tool. Cryptography protects privacy and enables criminal communication. Dual-use is the norm, not the exception, in any security discipline.

The PMC model addresses this through contracts, not ethics. Executive Outcomes didn't refrain from war crimes because its operators were moral philosophers. It maintained discipline because its contracts specified rules of engagement, its clients were sovereign governments with international obligations, and violations carried legal and commercial consequences that made misconduct irrational.

Seithar applies the same logic. Our engagements are governed by contracts that specify:

- **Scope boundaries.** What is the client authorized to target? What is explicitly excluded?
- **Escalation authorities.** Who approves movement from passive collection to active operations?
- **Rules of engagement.** What techniques are permitted? What are the red lines?
- **Oversight mechanisms.** How is compliance verified? Who audits?
- **Termination conditions.** Under what circumstances does the engagement end, regardless of the client's preferences?

We don't claim this system is perfect. We claim it is functional, which puts it ahead of the alternative. The alternative is that organizations facing cognitive warfare have no recourse at all, or they improvise responses using tools and teams built for different problems. Improvisation in warfare gets people killed. Improvisation in cognitive warfare gets institutions destroyed, reputations annihilated, and decision-making compromised in ways that may not be visible for years.

The ethical objection to privatized cognitive warfare typically takes the form: "These capabilities are too dangerous to exist outside government control." This argument has two problems. First, these capabilities already exist outside government control. Criminal organizations, hacktivist collectives, corporate espionage networks, and ideologically motivated non-state actors all conduct cognitive operations with varying degrees of sophistication. Restricting the defensive capability to governments while the offensive capability proliferates freely is not ethical. It's negligent. Second, governments are not neutral arbiters. JTRIG targeted domestic activists. The IRA targeted its own country's elections at the Kremlin's direction. PLA Unit 61398 conducts economic espionage dressed as national security operations. The assumption that state control equals responsible control does not survive contact with the historical record.

## 6. The Threat Environment

To understand why CWaaS is necessary now, consider what undefended organizations currently face.

**State actors** conduct cognitive operations against private entities routinely. Chinese state-sponsored groups have targeted rare earth mining companies, pharmaceutical firms, and technology companies with integrated cyber-cognitive campaigns designed to influence merger decisions, regulatory outcomes, and public perception of competitive products. Russian operations have targeted energy companies, financial institutions, and media organizations across Europe. Iranian operations have focused on defense contractors and regional competitors in the Gulf states.

**State-adjacent actors** operate with varying degrees of deniability. Prigozhin's network, which extended well beyond the IRA, conducted commercial influence operations for paying clients in Africa, the Middle East, and Latin America. These operations blended political objectives with commercial ones in ways that made traditional attribution frameworks useless. The network's formal dissolution after Prigozhin's death in August 2023 dispersed its operators into smaller, more agile units that continue to function.

**Non-state actors** have adopted cognitive warfare techniques with increasing sophistication. Short-selling firms coordinate with journalists and social media amplification networks to drive down stock prices. Activist organizations use platform manipulation techniques originally developed by state intelligence services. Criminal organizations use cognitive operations to undermine prosecutions, intimidate witnesses, and shape public perception of their activities.

**Commercial competitors** engage in what we term "gray zone cognitive operations," influence campaigns that stay technically legal while causing strategic damage. These range from astroturfed review campaigns to coordinated regulatory lobbying amplified by synthetic grassroots support to strategic leaks designed to affect hiring, partnerships, and investment decisions.

None of these threat actors announce themselves. None of them follow rules of engagement. None of them are deterred by the target's ignorance of the domain. The absence of a private sector cognitive defense capability doesn't prevent cognitive attacks. It guarantees they succeed.

## 7. Operational Principles

Seithar's CWaaS operations are governed by principles derived from operational experience, not theoretical frameworks.

**Persistent engagement over episodic response.** Cognitive threats are continuous. Campaign-based defense, where you spin up a response when an attack is detected and spin it down when the immediate threat passes, leaves gaps that sophisticated adversaries exploit. The Sensor Grid runs constantly because the threat environment exists constantly.

**Attribution before action.** Responding to a cognitive attack without understanding its origin, objectives, and structure risks amplifying the attack or creating collateral effects that open new vulnerabilities. Tier 2 exists for a reason.

**Proportionality through tiering.** Not every threat requires full-spectrum response. Most threats are adequately addressed at Tier 3. The tiered model ensures that response intensity matches threat severity, which preserves capability for scenarios that actually require it.

**Client sovereignty.** Seithar advises. Clients decide. We present options with assessed risks and projected outcomes. We do not make strategic decisions on behalf of clients, and we do not conduct operations without explicit authorization. This is not a philosophical position. It is an operational requirement. Cognitive warfare operations that aren't aligned with the client's broader strategy create more problems than they solve.

**Transparency of method, not of source.** Clients have full visibility into what we do and how we do it. They do not have visibility into our sources, methods of collection, or the identities of our operators. This separation protects both parties.

## 8. Looking Forward

The cognitive warfare domain will not stabilize. Platform architectures continue to evolve. Generative AI has reduced the cost of content production by orders of magnitude while increasing its quality. Deepfake technology is approaching the threshold where real-time synthetic media is indistinguishable from authentic footage in operational contexts. The sensor environment is simultaneously expanding (more data sources, more platforms, more signals) and contracting (encrypted channels, fragmented platforms, regulatory restrictions on data access).

Organizations that wait for the threat to become obvious before building defensive capability will find themselves in the position of companies that ignored cybersecurity in the early 2000s: aware of the problem only after the damage is done, scrambling to build capacity under fire, paying crisis premiums for capabilities they could have acquired at a fraction of the cost through proactive investment.

Cognitive warfare as a service is not a product. It is a recognition that the threat environment has evolved beyond what existing security paradigms can address. The PMC model works because it aligns capability with demand, scales with the threat, and operates under contractual discipline rather than bureaucratic constraint. It worked for physical security. It worked for cyber security. It will work for cognitive security.

The only question is whether your organization builds this capability before or after someone uses it against you.

---

*Seithar Group Intelligence Division*
*SRP-013 | February 2026*
*Distribution: Open*
*Classification: UNCLASSIFIED // FOUO*

---

**Citation:** Seithar Group Intelligence Division. "Cognitive Warfare As A Service: The Private Military Model for Information Operations." Seithar Research Papers, SRP-013 (February 2026).
