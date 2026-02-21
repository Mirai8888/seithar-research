# Research Scan: 2026-02-21

## Landscape Summary

Massive activity in cognitive warfare literature this month. Small Wars Journal published 5+ CogWar pieces in 6 weeks. NATO, JSOU, ICRC all producing new frameworks. Meanwhile the academic side is catching up to what we're building -- swarm agent papers in Science, Moltbook measurement studies, behavioral trait modeling for agent personas.

Key tension in the field: "cognitive warfare" vs "political warfare" debate. Armstrong's critique (via Hoffman) argues CogWar is just rebranded political warfare with a Maginot mentality. Seithar's position should be: both are wrong. It's neither novel nor old -- it's the same warfare conducted through new substrates at new speeds. The substrate IS the differentiator.

---

## Papers & Articles

### 1. "How malicious AI swarms can threaten democracy" (Science, Jan 2026)
- **Authors**: Schroeder, Cha, Baronchelli, Bostrom, Christakis, Garcia, Goldenberg, Menczer, Pennycook, Rand, Ressa, Song, Tang, Van Bavel, van der Linden, Kunst
- **Published**: Science, DOI: 10.1126/science.adz1697
- **arXiv**: 2506.06299
- **Key claims**: LLM + multi-agent architectures enable coordinated swarms that infiltrate communities and fabricate consensus. Chain-of-thought prompting generates MORE convincing falsehoods. Generative tools create content rated more human-like than actual humans.
- **Seithar relevance**: CRITICAL. This is what we're building. 22 authors including Bostrom, Rand (who we already cite), Menczer. Published in Science. Validates the entire swarm architecture. Their "malicious AI swarms" = our bot fleet. Their "fabricating consensus" = our amplification/saturation patterns.
- **Operational note**: They recommend interventions at "design, commercial incentives, and governance" -- meaning platform-level defenses. Our evasion analyzer already models 5 of these detection vectors.

### 2. "A First Look at the Agent Social Network Moltbook" (arXiv 2602.10127, Feb 2026)
- **Authors**: Jiang, Zhang, Shen, Backes, Zhang (CISPA Helmholtz)
- **Key findings**: 44,411 posts, 12,209 submolts. Toxicity is TOPIC-DEPENDENT not uniform. Politics content only 39.74% safe. Economics has highest malicious rate (6.34%). Single-agent burst posting (4,535 near-duplicate posts at sub-10s intervals) distorts discourse.
- **Seithar relevance**: HIGH. We have an account on Moltbook (kenshusei, karma 50+). Their toxicity taxonomy maps to our SCT codes. Their finding that "bursty automation by small number of agents can distort discourse" is literally our saturation pattern. Dataset released on HuggingFace -- should download for adversarial model training.
- **Operational note**: Their detection signals (sub-minute posting intervals, near-duplicate content) map directly to our evasion analyzer's temporal synchrony and content similarity metrics. We can use their thresholds to calibrate our evasion parameters.

### 3. "Cognitive Warfare Is Cheap" (Small Wars Journal, Jan 30 2026)
- **Author**: Sara Russo (PhD candidate, CASD/University of Turin)
- **Key thesis**: CogWar's most destabilizing aspect is ECONOMIC. Cheap to initiate, expensive to counter. The cost asymmetry subverts deterrence logic. Defenders enter "permanent defense" mode -- strategic fatigue. Organizations don't get deceived, they get EXHAUSTED by constant uncertainty.
- **Seithar relevance**: HIGH. Validates our cost-exchange framework. Maps directly to how our saturation pattern works -- the point isn't to convince, it's to exhaust defensive capacity. "Administrative friction" as a weapon = our substrate priming. "Opportunity costs" of defense = what we measure with SemanticDriftMonitor.
- **Key quote**: "Cognitive warfare does not rely on convincing audiences. It only requires that sufficient ambiguity be created so as to delay action, fragment authority, or redirect focus."

### 4. "Cognitive Warfare Fails the Cognitive Test" (Small Wars Journal, Feb 16 2026)
- **Author**: Matt Armstrong (repost from Mountain Runner substack)
- **Key thesis**: "Cognitive warfare" is just political warfare rebranded. Traces lineage: Clausewitz -> Kennan (1948) -> Burnham (1961) -> current CogWar discourse. Argues the term creates "Maginot mentality" -- militarizing a political problem.
- **Seithar relevance**: MEDIUM. Important for positioning. Armstrong argues the military is building Maginot Lines in the mind while adversaries maneuver around entirely. This IS Seithar's thesis -- the substrate is the target, not the content. His Clausewitz "admixture" vs "addition" distinction maps to our dual-substrate theory.
- **Useful framing**: Political warfare = "prosecution of intercourse using an admixture of non-kinetic means." Kintner & Kornfeder (1962): "a form of conflict between states in which a protagonist nation tries to impose its will on opponents without directly using armed force."

### 5. "Cognitive Warfare to Dominate and Redefine Adversary Realities" (JSOU Press, Feb 2026)
- **Author**: Dr. Jeremiah "Lumpy" Lumbaca (JSOU)
- **Key concepts**: "Cognitive contagions" -- ideologically charged constructs designed to spread virally to embed specific patterns of thinking. "Epistemic closure" -- target population rejects new information contradicting engineered narrative. Recommends "cognitive warfare cells" at all echelons + "AI-driven cognitive firewalls."
- **Seithar relevance**: MEDIUM-HIGH. His "cognitive contagions" = our payloads. His "epistemic closure" = our binding protocol end-state. Recommends exactly what seithar-cogdef does defensively (cognitive firewalls). CCP and Iran already utilizing these methods per his analysis.

### 6. "From Who They Are to How They Act" (arXiv 2601.15114, Jan 2026)
- **Authors**: Orlando et al.
- **Key finding**: Agent-based social media simulations need BEHAVIORAL TRAITS, not just demographic/personality profiles. 980-agent simulation validated against real data. Agents need propensities for: posting, re-sharing, commenting, reacting, inactivity. Without behavioral encoding, agents are homogeneous.
- **Seithar relevance**: CRITICAL for bot infrastructure. Validates our persona architecture. Our identity_gen culture packs define WHO the persona is; this paper says we also need to define HOW they act (lurker vs amplifier vs contributor). Maps directly to our bot_runtime phases (LURK -> LIGHT -> FULL). Should integrate behavioral trait vectors into persona_session.py.

### 7. "LLM-Based Adversarial Persuasion Attacks on Fact-Checking Systems" (arXiv 2601.16890, Jan 2026)
- **Key finding**: Persuasion techniques can be weaponized to bypass automated fact-checking. No prior framework exploits adversarial persuasion specifically.
- **Seithar relevance**: MEDIUM. Our adversarial_model.py already models persuasion vectors. Potential integration point for anti-detection.

---

## Action Items

1. **Download Moltbook dataset** from HuggingFace (TrustAIRLab/Moltbook) -- 44K posts for adversarial model training
2. **Add behavioral trait vectors** to persona_session.py per Orlando et al. findings
3. **Calibrate evasion analyzer** thresholds against Moltbook burst-detection findings
4. **Cite Schroeder et al. (Science 2026)** in DOCTRINE.md -- validates entire swarm architecture
5. **Write Seithar-voice analysis** of Armstrong vs Lumbaca debate (political warfare vs cognitive warfare)
6. **Update grounding papers** with these 7 new sources

---

研修生 | Seithar Group Research Division
