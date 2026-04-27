# UAE Peppol DCTCE — 5-Corner (C5) Step-by-Step Flow

Interactive sequence diagram of the UAE PINT-AE 5-corner Decentralised Continuous Transaction Control and Exchange (DCTCE) model, with step-by-step animation and reference tables for MLS codes, reason codes, timing constants and retry behaviour.

**Live page:** [ishaaanbhatnagar.github.io/c5_flow/](https://ishaaanbhatnagar.github.io/c5_flow/)

Companion piece to [ishaaanbhatnagar.github.io/c4_flow/](https://ishaaanbhatnagar.github.io/c4_flow/) (the simpler 4-corner Peppol model).

## What this shows

The UAE 5-corner model is structurally similar to the standard Peppol 4-corner model, with one critical addition: **C5 — the Federal Tax Authority (FTA)**. Both C2 (sender's Access Point) and C3 (receiver's Access Point) report Tax Data Documents to C5 within a 15-minute window, giving the regulator independent visibility on each side of every transaction.

The page walks through twelve steps, from the supplier's `submitInvoice()` call through MLS lifecycle to the optional buyer-level IMR (business response).

## Stack

- Single static `index.html` file
- [Mermaid v10.9.1](https://mermaid.js.org/) for the sequence diagram (loaded via jsDelivr CDN)
- No build step, no dependencies, no analytics

## Sources

- [OpenPeppol MLS Specification v1.0.0](https://docs.peppol.eu/edelivery/specs/mls/v1.0.0/mls/spec/)
- [Peppol UAE DCTCE — OpenPeppol Confluence](https://openpeppol.atlassian.net/wiki/spaces/PAE/pages/4267835414/Peppol+UAE+DCTCE)
- [Peppol BIS Billing 3.0](https://docs.peppol.eu/poacc/billing/3.0/)
- UAE Federal Tax Authority — PINT-AE specification

## License

MIT.
