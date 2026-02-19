---
title: "The Community Archive: 17 Million Tweets and the OSINT Surface Nobody Locked Down"
series: Seithar Current Event Analysis
id: CEA-022
date: 2026-02-19
author: Seithar Group Intelligence Division
tags: [OSINT, social graph analysis, epistemic.garden, community archive, HoleSpawn, network analysis, Twitter, intelligence collection]
---

# The Community Archive: 17 Million Tweets and the OSINT Surface Nobody Locked Down

## Seithar Group Current Event Analysis — CEA-022

---

## 1. EXECUTIVE SUMMARY

The epistemic.garden Community Archive is a crowdsourced dataset of approximately 17 million tweets, complete with follow graphs, quote chains, and reply trees, all sitting behind a public Supabase API with no authentication barrier. We fed it into HoleSpawn's network analysis engine as a field test. From 50 seed accounts, the engine resolved 6,712 nodes with full relational mapping. Top influential accounts were identified. Vulnerability analysis was completed in under an hour.

This is a case study in what open-source intelligence looks like when the data is structured, the API is open, and the analyst has the right tools. The implications extend well beyond one archive.

---

## 2. THE ARCHIVE

The Community Archive exists as a public good. Its creators built it with transparent intentions: preserve tweets that might otherwise disappear, make research possible, give people access to their own data. The project is crowdsourced. Users authorize export of their Twitter data, which gets ingested into a Supabase-hosted PostgreSQL database. The result is a queryable corpus that includes:

- **Tweet content** with full metadata (timestamps, engagement counts, client application)
- **Follow/follower relationships** as directed graph edges
- **Quote tweet chains** preserving the full citation structure
- **Reply trees** with parent-child threading intact
- **User profile data** including bios, join dates, follower counts over time

The Supabase API is public. No API key. No rate limiting that we encountered during our testing window. Standard REST queries return paginated JSON. You can filter by user, date range, content, engagement threshold. The schema is documented.

Seventeen million tweets is not Twitter's full corpus. It's a self-selected subset: the people who chose to contribute their archives. But self-selection is not random. The Community Archive skews toward a specific demographic: technically literate, engaged in discourse communities around AI, crypto, rationalism, effective altruism, and adjacent subcultures. This isn't a weakness for intelligence purposes. It's a feature. You're getting deep coverage of exactly the communities where influence operations, narrative seeding, and social engineering campaigns are most active and most consequential.

---

## 3. THE FIELD TEST

We used HoleSpawn's network analysis engine. The procedure:

**Seed selection.** We chose 50 accounts as entry points. Selection criteria: high engagement within the archive's community, varied position in the social graph (central nodes, bridge nodes, peripheral but high-output accounts), and coverage across the major topic clusters visible in the data.

**Graph expansion.** From those 50 seeds, HoleSpawn crawled the follow graph, quote chain, and reply tree relationships available through the API. Each connected account became a node. Each relationship became a directed edge with type metadata (follow, quote, reply, mutual follow).

**Result: 6,712 nodes.** A connected subgraph representing a substantial slice of the archive's social universe. Not the full 17 million tweets' worth of accounts, but a dense, richly connected neighborhood around our seeds.

**Network metrics computed:**
- Degree centrality (who has the most connections)
- Betweenness centrality (who bridges otherwise disconnected clusters)
- PageRank (who accumulates influence through the graph structure)
- Community detection via Louvain clustering (what are the natural groupings)
- Temporal analysis (how did these relationships form over time)

**Vulnerability analysis.** We flagged accounts and structural positions that represent single points of failure, bridge nodes whose compromise would fragment communities, and amplification chokepoints where a small number of accounts control disproportionate information flow.

The entire process, from first API call to completed analysis, took less than an hour of compute time. The bottleneck was API pagination, not processing.

---

## 4. WHAT WE FOUND

We're not publishing specific account names or detailed vulnerability maps. That's not what this analysis is for. The point is structural.

**The graph is strikingly centralized.** Despite the Community Archive's grassroots, decentralized ethos, the actual social graph exhibits classic power-law degree distribution. A small number of accounts (fewer than 50 in our 6,712-node subgraph) account for a disproportionate share of all quote and reply interactions. Remove those nodes and the graph fragments into disconnected clusters.

**Bridge nodes are identifiable and few.** Certain accounts serve as the primary connective tissue between topic clusters. The rationalism cluster connects to the AI safety cluster through roughly a dozen bridge accounts. The crypto-adjacent community connects to the policy discussion community through even fewer. These bridges are structural vulnerabilities. Compromise or impersonate a bridge node and you control the information flow between communities.

**Temporal patterns reveal influence campaigns.** By analyzing when follow relationships formed and when quote/reply activity spiked, we could identify coordinated engagement patterns. Not necessarily malicious ones. Organic community events (a viral thread, a conference, a controversy) produce similar signatures. But the analytical framework that detects organic coordination is the same one that detects artificial coordination. The tooling doesn't care about intent.

**The quote chain structure is particularly revealing.** Quote tweets create a citation graph. Who quotes whom, how often, and in what context maps the intellectual influence network with precision that follow graphs alone can't achieve. Follows are cheap. Quoting someone is an investment of attention and endorsement (or opposition). The quote graph is a higher-fidelity signal of actual influence than follower counts.

---

## 5. IMPLICATIONS FOR SOCIAL GRAPH INTELLIGENCE

This exercise was trivial. That's the point.

The Community Archive is one dataset, covering one platform's subset of users, with one public API. We used one analysis engine with standard graph algorithms. The result was a detailed intelligence product on community structure, influence topology, and vulnerability surfaces for over six thousand accounts.

Scale this up and the picture gets serious fast.

**Data availability is not the bottleneck.** Between public archives, API scraping, data breaches, and commercial data brokers, the raw material for social graph analysis is abundant. The Community Archive is notable only for being unusually well-structured and openly accessible. Less convenient sources yield the same data with more effort.

**Tooling is the bottleneck, and it's dropping.** Two years ago, the kind of analysis we ran would have required a dedicated team with custom infrastructure. Today, HoleSpawn's network engine runs it as a standard module. Graph analysis libraries are mature. Community detection algorithms are a pip install away. The barrier to entry is falling, and it's falling fast.

**Anyone with moderate technical skill can do this.** We're not describing nation-state capability. This is weekend-project territory for a competent developer with a clear objective. The Community Archive practically invites this kind of analysis. But the same techniques apply to any social graph data, regardless of source.

**The targets don't know they're mapped.** Nothing in our process touched any account directly. No follows, no likes, no DMs, no interactions of any kind. Pure passive collection from a public data source. The 6,712 people in our graph have no indication that their social relationships, influence patterns, and structural vulnerabilities have been cataloged. This is the nature of OSINT: the collection is invisible because it happens at a distance.

---

## 6. DEFENSIVE CONSIDERATIONS

If you're in the Community Archive (or any public social graph dataset), your relational data is intelligence material. Some things worth considering:

**Your follow graph is a map of your world.** Who you follow, who follows you, and the intersection of those sets reveals your community position, your information sources, and your potential pressure points. This is public data on most platforms. Treat it as such.

**Quote and reply patterns are behavioral signatures.** Consistent engagement with specific accounts creates a traceable pattern. An adversary studying your quote graph knows whose ideas you amplify, whose arguments you engage with, and whose framing you adopt. This is harder to obscure because it's a byproduct of normal participation.

**Bridge positions are high-value targets.** If your account connects otherwise separate communities, you are structurally valuable to anyone running an influence operation. Compromising a bridge node gives access to multiple audiences simultaneously. If you occupy this position, your account security posture should reflect it.

**Crowdsourced archives compound exposure.** Every person who contributes their archive to a public dataset increases the graph coverage for everyone connected to them. You didn't opt in to the Community Archive, but your followers who did just made your relational data available by proxy. Consent in network data is structurally impossible to contain to individuals.

---

## 7. ASSESSMENT

The Community Archive is a clean example of a pattern we expect to see more of: well-intentioned public datasets that constitute ready-made intelligence surfaces. The creators built something useful for researchers. We used it for network intelligence in under an hour. Both uses are legitimate. Both are enabled by the same open access.

The lesson is not that public archives are bad. The lesson is that social graph data, once structured and queryable, becomes intelligence material regardless of the intent behind its collection. The tools to process it are accessible. The techniques are documented. The people in the graph are unaware.

For anyone building social graph analysis capability: the Community Archive is an excellent training ground. The data is clean, the API is cooperative, and the community structure is rich enough to test any network analysis technique you're developing.

For anyone in the graph: you're already mapped. Act accordingly.

---

*Seithar Group Intelligence Division | seithar.com*
