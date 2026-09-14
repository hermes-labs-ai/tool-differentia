# Security Policy

## Scope

This repository is an archival package for a published Hermes Labs Zenodo
technical note, "Tool Differentia: Relational Static Analysis for AI Agent
Tool Descriptions" (DOI: [10.5281/zenodo.21817243](https://doi.org/10.5281/zenodo.21817243)).
It ships no runtime code, no service, and no dependency tree to have
vulnerabilities in: the contents are a PDF of the paper, citation and
discovery metadata (`CITATION.cff`, `CITATION.bib`, `codemeta.json`,
`.zenodo.json`, `llms.txt`, `metadata.json`), `SOURCES.md`, and this policy.
There is nothing here to execute, deploy, or exploit.

The deterministic static analysis this note describes (H1.6) is implemented
separately in [LintLang](https://github.com/hermes-labs-ai/lintlang).
Security reports about that implementation belong in that repository, not
this one.

## Reporting a problem

If you find a problem with the archived materials themselves — a citation or
metadata error, a broken canonical link, a factual or attribution error, or a
mismatch between this repository and the Zenodo record of record
(<https://doi.org/10.5281/zenodo.21817243>) — please open an issue in this
repository, or contact Hermes Labs via <https://hermes-labs.ai>.

## What this is not

This is not a software project with a release cycle. There is no
supported-versions table, no SLA, and no bug bounty. Reports are read and
handled on a best-effort basis by a solo maintainer.
