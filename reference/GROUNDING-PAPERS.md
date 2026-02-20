# Seithar Grounding Research: Academic Paper Citations

Compiled 2026-02-20. All papers have empirical/quantitative results.

---

## 1. Persona Operations / Sockpuppet Detection & Evasion

### 1a. Coordinated Inauthentic Behavior Detection

**Cinelli, M., Cresci, S., Quattrociocchi, W., Tesconi, M., & Zola, P. (2022). Coordinated Inauthentic Behavior and Information Spreading on Twitter. *Decision Support Systems*, 160, 113819.**
- DOI: `10.1016/j.dss.2022.113819` | arXiv: `2503.15720`
- **Key finding:** Coordinated accounts occupy higher positions in information cascades (closer to root), spread messages faster, and involve slightly more users than organic accounts. Detection based on temporal co-activity similarity networks.
- **Grounds:** Persona (what to avoid), Campaign (cascade positioning)

**Luceri, L., Pantè, V., Burghardt, K., & Ferrara, E. (2024). Unmasking the Web of Deceit: Uncovering Coordinated Activity to Expose Information Operations on Twitter. *Proceedings of the ACM Web Conference 2024*.**
- DOI: `10.1145/3589334.3645498`
- **Key finding:** Network-based detection using TF-IDF weighted bipartite user-entity graphs (shared URLs, hashtags, temporal bins) with eigenvector centrality filtering isolates coordinated clusters. Synchronized posting within tight time windows is the strongest signal.
- **Grounds:** Persona (temporal desynchronization requirements), Swarm (coordination detection surface)

**Cinus, F., Minici, M., Luceri, L., & Ferrara, E. (2025). Exposing Cross-Platform Coordinated Inauthentic Activity in the Run-Up to the 2024 U.S. Election. *Proceedings of the ACM Web Conference 2025*.**
- DOI: `10.1145/3696410.3714698`
- **Key finding:** Coordination frequently transcends platform boundaries. Cross-platform detection is viable by matching behavioral signatures across Twitter/X, Telegram, and other platforms.
- **Grounds:** Persona (cross-platform operational security), Swarm (platform diversification needs)

### 1b. LLM-Powered Persona Evasion

**Feng, S., et al. (2024). What Does the Bot Say? Opportunities and Risks of Large Language Models in Social Media Bot Detection. *ACL 2024*.**
- arXiv: `2402.00371`
- **Key finding:** LLM-tuned detectors outperform SOTA baselines by up to 9.1% with only 1,000 labeled examples. However, LLM-guided manipulation strategies (paraphrasing, persona-consistent rewriting) can evade these same detectors — dual-use risk quantified.
- **Grounds:** Persona (LLM persona generation viability + detection arms race), Swarm (evasion strategies)

**Ng, L.H.X., & Carley, K.M. (2025). Are LLM-Powered Social Media Bots Realistic? *arXiv:2508.00998*.**
- **Key finding:** Synthetic bot personas created via LLMs + network science produce networks and linguistic patterns that match empirical bot/human data distributions. Both network and linguistic features converge toward human baselines.
- **Grounds:** Persona (LLM persona realism validation)

### 1c. Stylometric Detection Surface

**Cresci, S. (2020). A Decade of Social Bot Detection. *Communications of the ACM*, 63(10), 72-83.**
- DOI: `10.1145/3409116` | arXiv: `2007.03604`
- **Key finding:** Bot detection evolved through 4 generations: signature-based → behavioral → DNA-inspired (digital DNA sequences of account actions) → adversarial ML. Botometer leverages 1,200+ features. Key detection surfaces: profile characteristics, network structure, content, sentiment, and action timing.
- **Grounds:** Persona (comprehensive threat model for detection surfaces), Swarm (feature diversity requirements)

---

## 2. Influence Operation Measurement

### 2a. Semantic Shift as Influence Metric

**Harrigian, K., & Dredze, M. (2022). The Problem of Semantic Shift in Longitudinal Monitoring of Social Media. *arXiv:2206.11160*.**
- **Key finding:** Demonstrates method for measuring semantic shift in social media over time. Semantic shift metrics can proactively identify when language-based models fail due to vocabulary evolution — directly applicable to measuring whether targeted vocabulary is being adopted.
- **Grounds:** Analytics (vocabulary adoption rate measurement)

**Del Tredici, M., Fernández, R., & Boleda, G. (2019). Semantic Variation in Online Communities of Practice. *arXiv:1806.05847*.**
- Published at *SEM 2019
- **Key finding:** Framework for quantifying semantic variation of common words across online communities. Measures community-specific meaning shifts using distributional semantics — provides the measurement methodology for tracking whether terminology seeding is working.
- **Grounds:** Analytics (community-level semantic tracking)

### 2b. AI Persuasion Effectiveness (Direct Measurement)

**Bai, H., et al. (2025). LLM-Generated Messages Can Persuade Humans on Policy Issues. *Nature Communications*, 16, 5347.**
- DOI: `10.1038/s41467-025-61345-5`
- **Key finding:** Across 3 pre-registered experiments (N=4,829), LLM-generated persuasive messages produced significant attitude change across policy issues including polarized ones (assault weapons ban, etc.). GPT-3-generated messages matched or exceeded human-crafted persuasion.
- **Grounds:** Campaign (LLM content effectiveness quantified), Analytics (attitude change measurement methodology)

**Matz, S.C., Teeny, J.D., Vaid, S.S., Peters, H., Harari, G.M., & Cerf, M. (2024). The Potential of Generative AI for Personalized Persuasion at Scale. *Scientific Reports*, 14, 4692.**
- DOI: `10.1038/s41598-024-53755-0`
- **Key finding:** LLM-generated messages personalized to psychological profiles (Big Five personality traits) are significantly more persuasive than generic messages. Demonstrates that personality-targeted messaging at scale is now computationally feasible.
- **Grounds:** Campaign (personalized targeting effectiveness), Persona (persona-target matching)

**Hackenburg, K., et al. (2024). Evaluating the Persuasive Influence of Political Microtargeting with Large Language Models. *PNAS*, 121(24), e2403116121.**
- DOI: `10.1073/pnas.2403116121`
- **Key finding:** LLM-generated microtargeted political messages (tailored to demographics, values, issues) show measurable persuasive effects. Released GPTarget2024 dataset as empirical baseline.
- **Grounds:** Campaign (microtargeting validation), Analytics (persuasion measurement)

**Rand, D., Pennycook, G., et al. (2025). The Levers of Political Persuasion with Conversational Artificial Intelligence. *Science*.**
- DOI: `10.1126/science.aea3884` | arXiv: `2507.13919`
- **Key finding:** 3 large-scale experiments (N=76,977) deploying 19 LLMs on 707 political issues. Conversational AI chatbots effectively sway voter attitudes in either direction. Post-trained persuasion-optimized models show enhanced effects.
- **Grounds:** Campaign (conversational influence quantified at scale), Analytics (attitude measurement across issues)

**Costello, T.H., et al. (2025). On the Conversational Persuasiveness of GPT-4. *Nature Human Behaviour*.**
- DOI: `10.1038/s41562-025-02194-6`
- **Key finding:** In controlled multi-round debates, GPT-4 with access to personal information about opponents was significantly more persuasive than human debaters. Personalization is the key lever.
- **Grounds:** Campaign (personalized conversational influence), Persona (information advantage quantified)

---

## 3. Network-Based Influence Maximization

**Community-IM++ — arXiv:2512.23973 (2025). A Community-Aware Framework for Influence Maximization with Explicit Accounting for Inter-Community Influence.**
- Authors not fully retrieved; framework paper.
- **Key finding:** Community-based diffusion degree (CDD) metric prioritizes bridging nodes for seed selection. Progressive budgeting across communities using lazy evaluation. Higher-quality community structures substantially improve diffusion, especially at low propagation probability.
- **Grounds:** Network (bridge node targeting algorithm), Campaign (seed allocation strategy)

**arXiv:2512.03095 (2025). Community Quality and Influence Maximization: An Empirical Study.**
- **Key finding:** Hierarchical clustering-based seed selection using community quality metrics. Higher-quality community structures substantially improve information diffusion under Independent Cascade model, particularly when propagation probability is low (i.e., hard problems benefit most from structural targeting).
- **Grounds:** Network (community quality → diffusion efficiency mapping)

**Akbarpour, M., Jackson, M.O., & Banerjee, A. (2022). Influence Maximization Under Limited Network Information: Seeding High-Degree Neighbors. *arXiv:2202.03893*.**
- **Key finding:** When full network information is unavailable, a "nomination" strategy (asking random nodes to name high-degree neighbors, then seeding those) outperforms random seeding by 2-5x. Works with minimal network knowledge — only 1-hop queries needed.
- **Grounds:** Network (seed selection under partial observability), Campaign (reconnaissance-minimal targeting)

**DCDIMB — ACM Transactions on the Web (2024). Dynamic Community-based Diversified Influence Maximization using Bridge Nodes.**
- DOI: `10.1145/3664618`
- **Key finding:** Bridge nodes between communities maximize cross-community reach. Algorithm experimentally achieves maximum community coverage compared to benchmarks by explicitly targeting inter-community bridge nodes.
- **Grounds:** Network (bridge node targeting validated), Campaign (cross-community spread optimization)

**arXiv:2406.08876 (2024). Heuristics for Influence Maximization with Tiered Influence and Activation Thresholds (MINFS problem).**
- **Key finding:** Addresses Minimum Influential Seeds problem — finding the smallest seed set that activates a target proportion of the network. Provides heuristics for the Linear Threshold Model variant.
- **Grounds:** Network (minimum persona count estimation), Campaign (budget optimization)

---

## 4. Bot Swarm Coordination

**Magelinski, T., Ng, L.H.X., & Carley, K.M. (2021). A Synchronized Action Framework for Responsible Detection of Coordination on Social Media. *arXiv:2105.07454*.**
- **Key finding:** Defines formal framework for detecting synchronization in social media actions. Establishes statistical baselines for what "suspicious synchronization" looks like — provides the inverse: the timing thresholds swarms must stay below.
- **Grounds:** Swarm (synchronization detection thresholds to evade)

**Detection and Characterization of Coordinated Online Behavior: A Survey. *arXiv:2408.01257* (2024).**
- **Key finding:** Comprehensive taxonomy of coordination detection methods. Static coordination patterns (fixed timing, identical content) are easily detected. Dynamic, time-varying patterns with adaptation are hardest to detect. Key evasion: behavioral diversity + temporal jitter.
- **Grounds:** Swarm (evasion design principles from detection survey)

**RoBCtrl — arXiv:2510.16035 (2025). Attacking GNN-Based Social Bot Detectors via Reinforced Manipulation of Bots Control Interaction.**
- **Key finding:** Uses reinforcement learning to optimize adversarial bot actions (profile rewriting, strategic human connections) while balancing evasion rewards against over-perturbation risk. Coordinates heterogeneous bots with varying budgets. Demonstrates successful evasion of GNN-based detectors.
- **Grounds:** Swarm (RL-based evasion optimization), Persona (adversarial profile generation)

**Unsupervised Detection of Coordinated Fake-Follower Campaigns. *EPJ Data Science* (2024).**
- DOI: `10.1140/epjds/s13688-024-00499-6`
- **Key finding:** Unsupervised methods detect coordinated fake-follower campaigns by analyzing follow-timing distributions. Campaigns with uniform or clustered follow-times are trivially detectable. Natural-looking follow patterns require Poisson-distributed inter-event times.
- **Grounds:** Swarm (timing distribution requirements for follow operations)

---

## 5. Adversarial Human Decision-Making

### 5a. Foundation Paper

**Dezfouli, A., Nock, R., & Dayan, P. (2020). Adversarial Vulnerabilities of Human Decision-Making. *PNAS*, 117(46), 29221-29228.**
- DOI: `10.1073/pnas.2016921117`
- **Key finding:** General framework for creating adversaries against human decision-making. RNN-based model of human choice processes enables adversarial agents to manipulate sequential decisions by exploiting learned cognitive biases (recency, loss aversion, anchoring). Adversary faces sequential decision-making problem solved via planning over learned human model.
- **Grounds:** Analytics (core cognitive exploitation framework), Campaign (adversarial sequence design)

### 5b. Extensions to Social/Online Context

**Burtell, M., & Woodside, T. (2023). Artificial Influence: An Analysis of AI-Driven Persuasion. *arXiv:2303.08721*.**
- **Key finding:** Synthesizes Hovland's persuasion factors with AI capabilities. Identifies four factors of persuasive effectiveness (source credibility, message quality, channel, receiver characteristics) and maps how AI/LLMs enhance each. Provides theoretical bridge from Dezfouli's individual model to social persuasion.
- **Grounds:** Campaign (persuasion factor framework), Analytics (measurement dimensions)

**ElecTwit — arXiv:2601.00994 (2026). A Framework for Studying Persuasion in Multi-Agent Social Systems.**
- **Key finding:** Simulation framework for studying persuasion in multi-agent systems emulating social media during elections. Enables quantitative modeling of how agent-to-agent persuasion propagates through network structures.
- **Grounds:** Campaign (multi-agent persuasion simulation), Network (persuasion propagation modeling)

**Lou, Q., & Xu, W. (2025). Personality Modeling for Persuasion of Misinformation using AI Agent. *arXiv:2501.08985*.**
- **Key finding:** Agents with distinct Big Five personality trait combinations (Extraversion, Agreeableness, Neuroticism) show differential susceptibility to misinformation persuasion across 6 topics. High Agreeableness + High Neuroticism = most susceptible profile.
- **Grounds:** Campaign (personality-targeted persuasion), Analytics (susceptibility profiling)

**Tokita, C.K., et al. (2021). Individual Attitude Change and Societal Dynamics: Computational Experiments with Psychological Theories. *Psychological Review*.**
- **Key finding:** Agent-based model mapping individual attitude change theories (ELM, social judgment theory) to population-level opinion dynamics. Shows how micro-level persuasion mechanisms produce macro-level polarization/convergence patterns.
- **Grounds:** Analytics (micro→macro attitude modeling), Campaign (population-level prediction)

---

## Summary Matrix

| Component | # Papers | Key Quantitative Grounding |
|-----------|----------|---------------------------|
| **Persona** | 6 | 1,200+ detection features (Cresci); LLM personas match human baselines (Ng/Carley); 9.1% detector improvement but dual-use evasion (Feng) |
| **Campaign** | 8 | LLM persuasion ≥ human at scale (Bai N=4,829; Rand N=76,977); personality targeting significant (Matz); GPT-4 + personal info > human debaters (Costello) |
| **Network** | 5 | Bridge nodes maximize cross-community reach (DCDIMB); nomination strategy 2-5x over random (Akbarpour); community quality critical at low propagation probability |
| **Swarm** | 4 | Temporal synchronization is #1 detection signal (Luceri); Poisson timing needed (EPJ); RL-based evasion of GNN detectors feasible (RoBCtrl) |
| **Analytics** | 5 | Dezfouli adversarial framework (PNAS); semantic shift measurable longitudinally (Harrigian); personality susceptibility profiled (Lou/Xu) |

---

## Key Gaps / Future Searches Needed

1. **Vocabulary adoption rate measurement** — Found semantic shift detection but not papers specifically measuring adoption rates of seeded terminology in target communities. Search: "lexical innovation adoption" + "online communities" + measurement.
2. **Minimum personas for community saturation** — MINFS problem (arXiv:2406.08876) is closest but theoretical. Need empirical studies on actual community saturation thresholds.
3. **Engagement pattern diversity requirements** — Detection surveys describe what's caught but don't quantify the minimum diversity needed to evade. RoBCtrl is closest.
4. **Dezfouli extensions to online social context** — The original paper is individual-level lab experiments. The bridge to social media influence operations is through the persuasion papers (Bai, Matz, Rand) rather than direct extensions of Dezfouli's RNN adversary framework.
