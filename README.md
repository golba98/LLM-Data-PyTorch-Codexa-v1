# LLM-Data

Reproducible text, conversational and binary token preparation.

Owns corpus cleaning, provenance, exact duplicate/root splits, source mixtures, binary packing and memmap datasets. PyTorch, Parquet and Hub dependencies are optional extras; choose them for the corresponding modules. Existing preparation/mixing algorithms and format variants remain distinct. Near-duplicate clustering is deferred.

## Development

In the sibling workspace, use `../LLM-From-Scratch/run.py --repo LLM-Data test`.
This selects the existing environment and sibling package sources without installing dependencies.
For a separately installed checkout, run `python -m pytest` after provisioning the documented dependencies and exact sibling version 0.1.0. These packages are local and not published to PyPI.

## Entry points

- `python -m llm_data.cli.benchmark_token_data --help`
- `python -m llm_data.cli.build_mixed_token_data --help`
- `python -m llm_data.cli.build_mixed_token_data_bucketed --help`
- `python -m llm_data.cli.build_smoke_dataset --help`
- `python -m llm_data.cli.build_token_accounting --help`
- `python -m llm_data.cli.download_fineweb_edu --help`
- `python -m llm_data.cli.download_language_corpora --help`
- `python -m llm_data.cli.estimate_parquet_tokens --help`
- `python -m llm_data.cli.inspect_token_data --help`
- `python -m llm_data.cli.prepare_base_corpus --help`
- `python -m llm_data.cli.prepare_conversational_sft --help`
- `python -m llm_data.cli.prepare_dataset --help`
- `python -m llm_data.cli.prepare_fineweb_edu --help`
- `python -m llm_data.cli.prepare_general_chat --help`
- `python -m llm_data.cli.prepare_repair_sft --help`
- `python -m llm_data.cli.sample_conversation_jsonl --help`
- `python -m llm_data.cli.tokenize_dataset --help`

## Integration and assets

`../LLM-From-Scratch/compatibility.json` records the complete tested version set.
Checkpoint weights, tokenizers, datasets and generated logs are referenced by path; none are distributed in this package. Preserve tokenizer fingerprints and architecture lineage. Source provenance is in PROVENANCE.md.

## Validation and limitations

See the central VALIDATION.md for commands, results and unverified large-model checks.
The original project is preserved unchanged. No model promotion, training pipeline or remote publishing occurs as part of extraction.
# LLM-Data-PyTorch-Codexa-v1

## Canonical workspace integration

This repository remains independently versioned at its existing remote and is pinned as a sibling in LLM-From-Scratch/compatibility.json. Integration decisions live in ../LLM-From-Scratch/documentation/training/SESSION_DECISIONS.md. Historical assets are external inputs; never commit weights, datasets or recovery snapshots.
