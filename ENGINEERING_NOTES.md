# promptfoo — engineering notes

LLM evaluation · Source review: 6 November 2026

## Purpose

A candidate for repeatable quality checks on prompts and RAG answers before changing a model or prompt version.

## Architecture reviewed

A TypeScript CLI/library with evaluation configs, providers, examples and a dedicated test suite.

Repository areas inspected: `src, test, examples, vitest.config.ts` (root inventory and linked README documentation).

## Decision and trade-off

Evaluation quality depends on the fixtures and assertions. A green result on a narrow dataset is not a production guarantee.

## Verification to perform

Include normal, unsupported, malformed and conflicting inputs; keep provider calls and costs explicit; run tests only on owned fixtures.

This is a source review and a proposed verification plan. No upstream runtime suite, deployment, provider benchmark or paid API evaluation was run for these notes.

## Attribution and scope

- Original project: [promptfoo/promptfoo](https://github.com/promptfoo/promptfoo).
- Original license: MIT; retained without replacement.
- Original README and source history remain part of the fork.
- This portfolio layer adds documentation; it does not claim authorship of the upstream project or an accepted upstream contribution.
- Dependency licenses, model weights, hosted services and any existing NOTICE files remain subject to their own terms.

## Start from the maintained instructions

Read the [upstream README](https://github.com/promptfoo/promptfoo/blob/main/README.md) and its contribution guidance for current installation and development commands.
