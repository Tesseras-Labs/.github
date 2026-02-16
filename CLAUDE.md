# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is the GitHub organization repository for **Tesseras Labs S.A.**, a Panama-based company building **RWADEX.ai** — infrastructure for compliant real-world asset (RWA) tokenization and market access. The `profile/README.md` serves as the public GitHub organization profile.

Currently this repo contains organizational documentation only. No source code, build system, or tests exist yet.

## Key Documents

- `CORPORATION.md` — Corporate definition: what the company builds, who it serves, architectural posture, compliance position
- `FOUNDER.md` — Founder decision-making principles and non-negotiables (guides ambiguity resolution)
- `README.md` — Public-facing organization overview
- `profile/README.md` — GitHub organization profile page

## Domain Context

RWADEX.ai uses a **multi-token market model**:
- **Ownership tokens** encode rights and enforce transfer policies (compliance-constrained)
- **Market tokens** and routing layers handle liquidity, price discovery, and interoperability
- Cross-ecosystem support (EVM and NEAR) where it strengthens access without compromising regulatory posture

Three stakeholder groups drive all product decisions: **Issuers**, **Investors/Market Participants**, and **Liquidity/Execution Partners**.

## Decision Principles

When making any contribution or resolving ambiguity, apply these in order:
1. Safety over speed
2. Clarity over cleverness
3. Durable architecture over temporary growth hacks
4. Institutional trust over speculative excitement

Compliance is foundational, not bolted on. Self-custody is the default. If something cannot be clearly explained to an issuer, investor, or regulator, it should not be in the system.

## Compliance Guardrails

- Tesseras Labs does **not** operate funds, provide investment advice, or act as a broker-dealer
- Systems must enforce eligibility and transfer constraints at token and application layers
- Auditability and traceability of state changes must be preserved
- Jurisdiction-aware deployment patterns are required
