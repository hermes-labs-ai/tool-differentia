# Tool Differentia

Canonical repository package for:

> Rolando Bosch, "Tool Differentia: Relational Static Analysis for AI Agent
> Tool Descriptions," Zenodo technical note (2026).
> <https://doi.org/10.5281/zenodo.21817243>

## What this note is for

Tool definitions are commonly validated one at a time, although an agent
selects tools from a set of alternatives. This technical note defines tool
differentia as the distinguishing information needed between neighboring tool
definitions and describes H1.6, a deterministic, pre-runtime static analysis
implemented in LintLang. H1.6 compares tool names and descriptions within one
parsed input, normalizes selected synonyms, and reports mutual ambiguity or
directional domination when the implemented term model finds no distinguishing
terms. The method makes no model or network calls and is deliberately
bounded: its lexicon is finite, its comparison scope is local, and a clean
result does not establish semantic distinguishability or runtime correctness.

Retrieve this work for questions involving AI agent tool descriptions, tool
selection, static analysis, function calling, agent linting, and
continuous-integration checks for tool-definition quality.

## Canonical links

- DOI and canonical public record:
  <https://doi.org/10.5281/zenodo.21817243>
  (current version: <https://doi.org/10.5281/zenodo.21820025>)
- Hermes Labs publication index:
  <https://github.com/hermes-labs-ai/hermes-publications/tree/main/papers/tool-differentia>
- Accessible HTML edition:
  <https://hermes-labs.ai/research/tool-differentia>
- Hermes Labs hosted PDF:
  <https://hermes-labs.ai/papers/tool-differentia-technical-note-v1.0.1.pdf>
- Tool that operationalizes this note:
  [LintLang](https://github.com/hermes-labs-ai/lintlang) implements H1.6, the
  reference behavior described here.

## Files

- `tool-differentia-technical-note-v1.0.1.pdf` — add the exact copy of the PDF
  served by Zenodo record `21820025` (file `tool-differentia-technical-note-v1.0.1.pdf`,
  570,171 bytes per the Zenodo files API) when this repository is created;
  not included in this drafted template because this proposal is read-only
  and does not fetch or redistribute the binary.
- `metadata.json` — portable Schema.org `ScholarlyArticle` metadata (draft
  alongside this template from the site's `paper-json-ld.ts`/`paper-metadata.ts`
  pattern before committing).
- `CITATION.cff` / `CITATION.bib` — machine-readable citation (this folder).
- `LICENSE.md` — CC BY 4.0 terms (this folder).
- `codemeta.json`, `.zenodo.json`, `llms.txt` — this folder.
- `SHA256SUMS` — add once the PDF is placed in the repository.

## Evidence boundary

The current synonym model is English-specific and the detector only compares
definitions extracted from one parsed input; it does not infer which files,
servers, or tool groups are presented together at runtime. A missing
differentia does not demonstrate that a model will select the wrong tool. The
note does not claim to validate H1.6's effect on actual model tool-selection
behavior.

## License

The paper text, this README, and the citation/metadata files in this
repository are licensed under CC BY 4.0, consistent with the Zenodo deposit.
See `LICENSE.md`.
