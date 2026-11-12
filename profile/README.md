# TACITUS

**Data infrastructure for Policy / Political AI.**

We build explicit knowledge structures, task-specific context capsules and reviewable artifacts. The aim is better saliency and efficiency in AI generation: preserve the distinctions that change an answer, then measure the full cost of producing it.

[Explore tacitus.me](https://tacitus.me/) · [Build guide](https://tacitus.me/developers/) · [LinkedIn](https://www.linkedin.com/company/tacitus-me) · [Public project map](https://github.com/sargonxg/sargonxg/blob/main/docs/PUBLIC_PROJECT_MAP.md)


## Enter the House of Evidence

![Original TACITUS Source Workshop: saved sources, typed structure, bounded context and human review](https://raw.githubusercontent.com/sargonxg/sargonxg/a91027079c8ff8ebbd3623898a5e03a13cd80df5/assets/tacitus-source-workshop-8bit.png)

*Original concept illustration; the scene and documents are fictional. [Artwork and reuse](https://github.com/sargonxg/sargonxg/blob/a91027079c8ff8ebbd3623898a5e03a13cd80df5/docs/VISUAL_IDENTITY.md).*

A small lesson with a real purpose: recover the missing condition, preserve who said what, place events in time, and review before exporting. **[Clone and play the original adventure](https://github.com/TACITUS-me/.github/blob/main/TACITUS_GUIDE.md)**. The lesson needs no API key or account and uses fictional dispatches; it is separate from the working policy tools below.

## Choose the smallest useful starting point

| You need to… | Start here | What is ready |
| --- | --- | --- |
| Prepare evidence-backed policy context | [Pinned organization pipeline](https://github.com/TACITUS-me/Open_Starting_Kpipeline_TACITUS) | Offline graph/capsule/review-sheet build; Python standard library. |
| Inspect a draft against its source | [Workbench](https://github.com/sargonxg/tacitus-workbench) | Local/static source, graph and artifact views; model execution is separate. |
| Study historical political evidence | [Middle East toolkit](https://github.com/sargonxg/Syria-political-analysis) | Dated snapshots, exact document spans and bounded research exports. |
| Understand the design and limits | [Methods and credit](https://github.com/sargonxg/sargonxg/blob/main/docs/RESEARCH_AND_DESIGN.md) | Papers, upstream contributions, implemented differences and evaluation still needed. |

We are building reusable infrastructure, not a new authority over the sources. Our testable contribution is making selection, structure, evidence dependencies and review state explicit. Whether that improves an analyst’s decisions or a model’s answers must be established by matched human evaluation.

## Start with a working policy task

Prepare a historical Syria negotiation-policy note from exact source passages. Build the ontology and semantic layer, run an evidence-inspection agent, and inspect the cited draft beside its source wording.

```sh
git clone https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open.git
cd TACITUS-Knowledge-Pipeline-open/reference-pipeline
PYTHONPATH=src python -m unittest discover -s tests -v
```

[Run the complete workflow](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/blob/main/reference-pipeline/docs/model-workflows.md) · [Inspect the actual cloud run](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/tree/main/reference-pipeline/examples/syria-negotiation/agent-step-2) · [Open the workbench guide](https://github.com/sargonxg/tacitus-workbench/blob/main/apps/workbench/docs/policy-workflow.md)

![Actual model-assisted policy draft inspected beside historical evidence](https://raw.githubusercontent.com/sargonxg/TACITUS-Knowledge-Pipeline-open/main/assets/showcase/policy-workflow-desktop.png)

The recording was produced with Cloudflare on 10 November 2026. The model inspected selected evidence before drafting; code retained exact quotations and qualifications. The result remains a draft for human review. It is a historical source exercise, not a current Syria assessment.

## What you can build

| Layer | Working reference |
| --- | --- |
| Data structures | [Exact sources](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/blob/main/reference-pipeline/docs/sources.md), [ontology rules](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/blob/main/reference-pipeline/docs/ontology.md), [semantic layers](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/blob/main/reference-pipeline/docs/semantic-layers.md), qualified graph records and source versions. |
| Context capsules | Bounded task context with entity and relation definitions, exact evidence, conditions, review checks and explicit omissions. |
| Artifacts | Populated evidence review sheets and model-assisted cited desk notes, with source wording kept alongside the draft. |
| Agent workflows | [Finite evidence-inspection agent](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/blob/main/reference-pipeline/src/tacitus_pipeline/agent.py): selected evidence lookup, then a draft. No arbitrary browsing, code execution, publication or approval tool. |
| Evaluation | [Real request/response recordings](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/tree/main/reference-pipeline/examples/syria-negotiation), local tests and a separate held-out model-evaluation plan. |

## Public code and current scope

Active research code currently spans this organization and the founder's `sargonxg` account. These links identify the actual maintained locations; the repositories have not been transferred.

| Repository | Useful work | Scope |
| --- | --- | --- |
| [Knowledge Pipeline](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open) | Source → graph → capsule → cited model draft; cloud/local HTTP adapters and bounded agent | Runnable reference; 42 reference tests checked at the accepted pin on 11 November 2026. Apache-2.0 code. |
| [Workbench](https://github.com/sargonxg/tacitus-workbench) | Inspect source-linked objects, exact evidence, qualifications and recorded agent steps | Local/static tools; separate from hosted PRAXIS. |
| [Syria / Middle East toolkit](https://github.com/sargonxg/Syria-political-analysis) | Historical research atlas, source records and a source-preserving pipeline exporter | Reconciled research toolkit: 203 local tests pass; two service-dependent checks skipped. Dated evidence, not a live feed. |
| [AGON](https://github.com/sargonxg/AGON) | Conflict-analysis research and exact evidence-span verification | Experimental modules; existing all-rights-reserved license applies. |
| [KAIROS](https://github.com/sargonxg/KAIROS-temporal-vision-TACITUS) | Temporal relationships and graph experiments | Local prototype; live-model acceptance is separate. Apache-2.0. |
| [DIALECTICA v3](https://github.com/sargonxg/A3_DIALECTICAbyTACITUS_v3) | Native capsule contracts, review records, graph projections and CLI experiments | Experimental core; not a complete hosted ingestion product. Apache-2.0. |
| [TCGC](https://github.com/sargonxg/TCGC_TACITUS-Conflict-Grammar-Corpus_BENCHMARK) | Conflict-grammar corpus and structural scorer; separate workflow-recording inspector | Alpha benchmark. **CC BY-NC-SA 4.0**; commercial reuse requires separate review. |
| [PRAXIS](https://github.com/sargonxg/A4_PRAXIS_CLOUD_Work) | Agentic policy workspace source | Invitation-only hosted application. Generation and paid upgrades remain paused. |

## Evidence and research

The one-task model smoke test does not establish a general quality or efficiency gain. Both flat and structured drafts resolve their citations; structured context used more total tokens in this example. Citation identity, semantic entailment and expert approval are separate checks.

[12-paper research index](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/tree/main/research) · [Verified workflows and limits](https://github.com/sargonxg/sargonxg/blob/main/docs/VERIFIED_WORKFLOWS_2026-11-10.md)

The current pipeline format is separate from native Context and DIALECTICA capsules. A verified hosted PRAXIS attachment bridge remains in development.

## Historical organization repositories

[Open_Starting_Kpipeline_TACITUS](https://github.com/TACITUS-me/Open_Starting_Kpipeline_TACITUS) pins the maintained runnable pipeline and retains the early notebooks as historical material. [DIALECTICA A2](https://github.com/TACITUS-me/DIALECTICA_by_TACITUS_A2) is the historical Python predecessor of v3.

The archived [Semantica](https://github.com/TACITUS-me/semantica4tacitus), [Cozo](https://github.com/TACITUS-me/cozo4TACITUS) and [regulatory assistant](https://github.com/TACITUS-me/regulatory-intelligence-assistant-4TACITUS) repositories are upstream reference forks, not original TACITUS products. The [early AGON fork](https://github.com/TACITUS-me/AGON-humanfriction-detection-TACITUS) is archived. Original attribution and licenses apply.

[Discuss a pilot](https://tacitus.me/pricing/) · [hello@tacitus.me](mailto:hello@tacitus.me)

## Current readiness and what comes next

[Public repository readiness and 20 concrete refinements](https://github.com/sargonxg/sargonxg/blob/main/docs/FRESH_START.md) records local checks, historical/experimental boundaries and the next useful gate. The accepted source improvements are on the default branches. Current PRAXIS source passes its verification, audit and five-scenario authenticated emulator lane; hosted generation and paid upgrades remain paused.
