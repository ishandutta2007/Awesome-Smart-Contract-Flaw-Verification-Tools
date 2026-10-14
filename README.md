# Awesome-Smart-Contract-Flaw-Verification-Tools

## Top Smart Contract Flaw Verification Tools Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Static Analysis, Formal Verification & Runtime Monitoring*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Smart Contract Flaw Verification**. These tools analyze Web3 and digital contract logic dynamically and statically — finding vulnerabilities, proving correctness, and monitoring deployed contracts before attackers can exploit them.



**Examples** include CertiK, OpenZeppelin, ConsenSys Diligence, Trail of Bits, Quantstamp, Halborn, Hacken, PeckShield, and Immunefi (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom analysis pipelines, and transparent verification — ideal for security researchers, developers building DeFi protocols, and teams avoiding per-audit pricing.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CertiK](https://www.certik.com/)**  

  High-volume audit firm with thousands of completed audits and the Skynet on-chain monitoring system that watches deployed contracts post-launch. Common on exchange listing checklists, though breadth is the model rather than depth .



- **[OpenZeppelin](https://www.openzeppelin.com/)**  

  Maintains the most widely used open-source contract library for Solidity development. Auditors review code built on patterns they authored, typically pairing multiple senior reviewers with static analysis and fuzzing. The reference-standard choice for EVM protocols .



- **[ConsenSys Diligence](https://diligence.security/)**  

  Audit arm of ConsenSys (MetaMask, Infura pedigree), giving deep native Ethereum expertise. Client list includes Aave, Balancer, and 1inch. Pairs manual review with in-house tooling built specifically for Ethereum mainnet protocols .



- **[Trail of Bits](https://www.trailofbits.com/)**  

  Top name for hard problems — cryptography, zero-knowledge circuits, and low-level infrastructure. Maintains open-source security tools the industry relies on, including **Slither** and **Echidna**. Trade-off is price and availability: among the most expensive firms with long queues .



- **[Quantstamp](https://quantstamp.com/)**  

  One of the earliest dedicated audit firms (since 2017), offering **formal verification** — mathematically proving code behaves as specified — alongside standard manual audits. Premium pricing reflects the highest assurance level for critical logic .



- **[Halborn](https://www.halborn.com/)**  

  Leans into offensive security: red-teaming, penetration testing, and infrastructure review alongside contract audits. Works with larger exchanges, institutions, and high-value protocols where risk surface extends beyond contracts to servers, keys, and staff .



- **[Hacken](https://hacken.io/)**  

  Full security stack: code review, penetration testing, bug-bounty platform, and on-chain monitoring across 30+ chains. Operating since 2017, publishes widely cited Web3 security reports. One partner across the entire security lifecycle .



- **[PeckShield](https://peckshield.com/)**  

  Blockchain security firm specializing in smart contract auditing, threat intelligence, and incident response. Known for rapid post-exploit analysis and public disclosure of attack vectors.



- **[Immunefi](https://immunefi.com/)**  

  Largest Web3 bug bounty marketplace: 45,000+ researchers, 650+ active programs, and $110M+ paid out. Uses **Vulnerability Severity Classification System V2.2** (impact × privilege × likelihood). Most programs require a working PoC — no PoC means rejection or downgrade .



## Open-Source GitHub Projects



- **[MIESC (Multi-layer Intelligent Evaluation for Smart Contracts)](https://pypi.org/project/miesc/)**  

  **The most comprehensive open-source smart contract analysis framework.** Orchestrates **31 security tools across 9 defense layers** — Static, Dynamic, Symbolic, Formal, AI, ML, Threat Modeling, Cross-Chain, and AI Ensemble. Integrates Slither, Aderyn, Mythril, Echidna, Foundry, Certora, Halmos, and SmartLLM. On the SmartBugs-curated dataset (50 contracts), achieves **100% precision, 70% recall, 82.35% F1-score** with zero false positives. AI correlation via local LLM (Ollama) reduces false positives. Compliance mapping for ISO 27001, NIST, OWASP, and SWC. Multiple interfaces: CLI, REST API, WebSocket, MCP, and Web UI. Docker-ready with named profiles (defi, token, security, thorough) .



- **[Slither](https://github.com/crytic/slither)**  

  Trail of Bits' static analysis framework for Solidity — the industry-standard first-pass detector. Finds reentrancy, access control issues, and dangerous patterns. Underlies many commercial audit workflows .



- **[Echidna](https://github.com/crytic/echidna)**  

  Trail of Bits' property-based fuzzer for Ethereum contracts. You define invariants and it attempts to falsify them through smart mutation. Standard tool in professional audit pipelines .



- **[Medusa](https://github.com/crytic/medusa)**  

  Cross-platform, Go-ethereum-based fuzzer inspired by Echidna. **Parallelized fuzz testing** across multiple workers with coverage-guided mutation. Provides CLI and Go API for custom testing methodology. Successor lineage to Echidna .



- **[Halmos](https://github.com/a16z/halmos)**  

  a16z's symbolic testing tool that **reuses existing Foundry tests** as formal specifications. Makes symbolic execution accessible to developers already writing Foundry tests .



- **[Kontrol](https://github.com/runtimeverification/kontrol)**  

  Runtime Verification's formal verification tool that integrates with Foundry, allowing developers to write formal specifications as Foundry tests in Solidity. Built on **KEVM** (validated formal semantics of EVM bytecode), providing mathematical guarantees that verified contracts behave identically when executed. Open source under BSD-3 Clause. CI integration and Kontrol as a Service (KaaS) for cloud verification .



- **[hevm](https://github.com/dapphub/dapptools/tree/master/src/hevm)**  

  State-of-the-art symbolic and concrete EVM execution engine. Performs symbolic execution and **equivalence checking** between contracts. CLI tool for security researchers .



- **[Aderyn](https://github.com/Cyfrin/aderyn)**  

  Cyfrin's **Rust-based Solidity static analyzer** designed to help protocol engineers and security researchers find vulnerabilities. Community-driven with VSCode extension .



- **[ESBMC](https://esbmc.github.io/)**  

  Mature, permissively licensed SMT-based bounded model checker supporting Solidity alongside C, C++, CUDA, Python, and Rust. **Automatically detects or proves absence of runtime errors** (bounds checks, pointer safety, overflow) and verifies user-defined assertions. Used to verify Solidity smart contracts handling millions of dollars .



- **[Isabelle/Solidity](https://zenodo.org/records/15121526)**  

  Academic formal verification tool implemented as a definitional extension for the Isabelle proof assistant. Complements axiomatic approaches by providing a foundational framework. Funded by UK Research and Innovation (EP/X027619/1) .



- **[AI Smart Contract Auditor](https://pypi.org/project/ai-smart-contract-auditor/)**  

  AI-powered audit system with a **vulnerability database of 47,294 findings** and **305,943 PoCs** aggregated from Sherlock, Solodit, DeFiHackLabs, and Web3Bugs. ChromaDB vector search with 14,291 semantic embeddings. **17.7x parallel speedup**, 97.5% audit success rate, 2–5 minute average audit per contract. Generates PoCs 15x faster than manual. 621 tests with 100% pass rate. MIT licensed .



- **[AW3SS (Automated Web3 Security Scanner)](https://pypi.org/project/aw3ss/)**  

  Enterprise-grade autonomous security framework with **1,015 indexed exploit templates** in a vector RAG knowledge base. Multi-chain native RPC routing with deterministic mainnet forking (Ethereum, Arbitrum, Base, Polygon, BSC, Optimism, Cronos, Flare). **8 formal invariant assertions** covering CRITICAL to LOW severity. Self-healing PoC engine with 3 retries and temperature-controlled adjustments. Docker Foundry sandbox with `--cap-drop=ALL` hardening. Outputs SARIF v2.1.0 and Markdown audit reports ready for Code4rena, Sherlock, and Immunefi submission .



### Additional Strong Open-Source Options



- **[SmartBugs](https://github.com/smartbugs/smartbugs)** — Execution framework for analyzing Solidity contracts with multiple analysis tools. Foundation dataset used by MIESC validation .

- **[Solodit](https://solodit.xyz/)** — Aggregates audit findings across firms, searchable by vulnerability class. Essential pattern-mining resource .

- **[Trail of Bits building-secure-contracts](https://github.com/crytic/building-secure-contracts)** — Educational resource with vulnerability patterns, checklists, and development guidelines.

- **[EVM Fuzz (spamoor)](https://pkg.go.dev/github.com/ethpandaops/spamoor)** — Deploys randomly generated bytecode to find consensus bugs and stress-test EVM implementations. Stack-aware bytecode generation, weighted opcode selection, and precompile testing .

- **[kevm](https://github.com/runtimeverification/evm-semantics)** — K framework formal semantics of EVM bytecode, the foundation for Kontrol's verification guarantees .



**Frameworks for building custom systems**: Combine **MIESC** for multi-layer orchestration across 31 tools, **Slither** and **Aderyn** for static analysis, **Echidna** or **Medusa** for property-based fuzzing, **Halmos** or **Kontrol** for formal verification, and **AW3SS** for autonomous PoC generation to build a complete self-hosted smart contract verification stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Smart contract verification tools must comply with applicable laws, exchange listing requirements, and security best practices. **No tool or audit guarantees complete safety** — defense in depth, bug bounties, and runtime monitoring are essential complements.

- Self-hosted open-source solutions require proper security hardening, regular updates, and validation against known vulnerability datasets.



---



**Made for smart contract auditors, DeFi developers, security researchers, and teams building Web3 verification platforms.**  

Let's make smart contract flaw verification more open, rigorous, and accessible.
