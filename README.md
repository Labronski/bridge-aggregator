# Bridge Aggregator

A tool for tracking cross-chain bridge transactions across multiple providers and networks in one place. Built to solve one of the most frustrating investigation problems in Web3 support: figuring out where a bridged transaction actually is.

---

## The Problem

Bridge transactions are hard to support. A single bridge operation touches two separate blockchains, goes through a third-party bridge provider, and each provider has its own status schema, terminology, and data format. When something goes wrong, you're switching between multiple provider dashboards, cross-referencing transaction hashes, and trying to reconcile inconsistent status labels.

The Bridge Aggregator pulls data from MetaMask's bridge API and the underlying provider APIs, normalizes it into a single consistent view, and surfaces everything you need to diagnose an issue in one place.

---

## Features

- Aggregates bridge transaction data across multiple providers (e.g. LI.FI, Socket, Squid)
- Normalizes status labels, amounts, and timestamps across providers
- Shows source chain, destination chain, token, amount, and current status at a glance
- Surfaces intermediate transaction hashes for both the source and destination legs
- Reduces diagnosis time for stuck, pending, or failed bridge transactions

---

## Stack

- **JavaScript** — core logic and API integration
- **HTML / CSS** — frontend interface
- **MetaMask Bridge API** — primary transaction data source
- **Bridge Provider APIs** — LI.FI, Socket, Squid, and others for status resolution

---

## Notes

This is an internal tool and the live environment is not publicly accessible. Source code is not included as it contains environment-specific API configurations. This README documents the project's purpose, design, and impact.
