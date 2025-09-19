# Blockora Technical Design Blueprint

## 1. Overview
Blockora is a next-generation blockchain protocol designed for scalability, security, and community-driven growth. Unlike existing solutions that rely on energy-intensive Proof of Work or wealth-concentrated Proof of Stake, Blockora introduces **Proof of Contribution (PoC)** – a consensus mechanism that rewards users for meaningful participation in the network.

This document describes the **technical architecture**, **consensus mechanism**, **tokenomics**, **security model**, and **future upgrades** in detail, serving as a reference for developers and contributors.

---

## 2. Network Architecture

### 2.1 Layers
- **Application Layer:** dApps, smart contracts, token factory, NFT marketplace.
- **Consensus Layer:** Proof of Contribution consensus engine, validator selection, block production.
- **Network Layer:** P2P gossip protocol, transaction propagation, validator discovery.
- **Execution Layer:** WASM-based smart contract engine for fast, secure computation.
- **Storage Layer:** Merkle-tree-based state storage with pruning support for lightweight nodes.

### 2.2 Node Types
- **Validator Nodes:** Produce blocks, validate transactions, secure the chain.
- **Contributor Nodes:** Participate in PoC, run light clients, submit transactions.
- **Observer Nodes:** Read-only access, used by explorers, analytics, and auditors.

---

## 3. Consensus – Proof of Contribution (PoC)

PoC is a hybrid reputation-based consensus mechanism that uses a **Contribution Score** for each participant. Rewards are distributed proportionally to scores.

**Formula:**
