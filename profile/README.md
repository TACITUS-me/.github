# TACITUS

**A conversation workspace for reusable team context.** Save the instructions, sources and examples that made one conversation useful. Bring them into the next conversation or give a teammate the same starting point.

[Open the App](https://app.tacitus.me/) · [Try a conversation](https://app.tacitus.me/try.html) · [TACITUS website](https://tacitus.me/) · [App availability](https://app.tacitus.me/api/health)

## Keep the context behind the work

- **Capsules** hold the background, working instructions and sources a task needs.
- **Artefacts** show the expected result through a template, a good example or a previous deliverable.
- **Knowledge graphs** connect saved statements to exact passages and source editions. A semantic layer selects the relationships and evidence relevant to a task.

For a new task, attach the team’s working rules, an example of the expected output and the exact source to use. The App keeps the selected versions with the conversation so you can inspect them later. Its experimental public practice uses local previews and template-based outlines. See the availability endpoint for hosted generation.

## Run the public reference

The open Python compiler shows how exact sources become a provenance graph, a bounded capsule and a proposed review sheet. In the pinned example, NIST kept its citation-checking guidance and changed its reference number between the April draft and July final. Checking both editions also shows that the final identifier pointed to a different action in the draft.

Use Python 3.11 or newer. The command needs no API key and makes zero model calls.

```sh
git clone https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open.git
cd TACITUS-Knowledge-Pipeline-open
git checkout --detach be8640a6a2b5ff2755c884e9e7eae981bb98e62e
cd reference-pipeline
PYTHONPATH=src python3 examples/citation-guidance/compile.py --output build/citation-guidance
cmp examples/citation-guidance/proof.json build/citation-guidance/proof.json
diff -r examples/citation-guidance/compiled build/citation-guidance/compiled
```

Open `build/citation-guidance/proof.json` for the proposed judgment and `build/citation-guidance/compiled/brief.md` for the source passages and reviewer checks. The companion export provides PROV-O provenance and SKOS concepts with optional SHACL validation. The build verifies evidence assembly. Research on answer quality and review time remains in progress.

[Exact-source example and outputs](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/tree/be8640a6a2b5ff2755c884e9e7eae981bb98e62e/reference-pipeline/examples/citation-guidance) · [Evaluation protocol](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/blob/be8640a6a2b5ff2755c884e9e7eae981bb98e62e/reference-pipeline/benchmarks/model-evaluation-plan.json)

## Public projects

| Project | What you can inspect |
| --- | --- |
| [Knowledge Pipeline](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open) | The standard-library reference compiler, source pins, ontology and semantic-layer examples. |
| [Workbench](https://github.com/sargonxg/tacitus-workbench) | Local readers for source-linked material, graphs and recorded drafts. |
| [DIALECTICA](https://github.com/sargonxg/A3_DIALECTICAbyTACITUS_v3) | Experimental capsule contracts and graph projections. |
| [KAIROS](https://github.com/sargonxg/KAIROS-temporal-vision-TACITUS) | Experimental temporal relationships for knowledge graphs. |

Each project documents its own license, formats and verification. The public compiler, hosted App and local Workbench use separate contracts. Review format compatibility before moving an output between them.

[Format guide](https://github.com/sargonxg/tacitus-workbench/blob/main/docs/FORMAT_COMPATIBILITY.md) · [Research and credits](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/tree/main/research) · [Public project map](https://github.com/sargonxg/sargonxg/blob/main/docs/PUBLIC_PROJECT_MAP.md) · [Teaching demo](https://github.com/TACITUS-me/.github/blob/main/TACITUS_GUIDE.md)

<details>
<summary>Earlier roadmap and research projects</summary>

- [Research and design notes](https://github.com/sargonxg/sargonxg/blob/main/docs/RESEARCH_AND_DESIGN.md), [earlier roadmap](https://github.com/sargonxg/sargonxg/blob/main/docs/GROWTH_PLAN.md) and [validation protocol](https://github.com/sargonxg/sargonxg/blob/main/docs/VALIDATION_PROTOCOL.md).
- [Organization starter pipeline](https://github.com/TACITUS-me/Open_Starting_Kpipeline_TACITUS) and [DIALECTICA A2](https://github.com/TACITUS-me/DIALECTICA_by_TACITUS_A2).
- [Historical Syria and Middle East toolkit](https://github.com/sargonxg/Syria-political-analysis), [AGON evidence-span tools](https://github.com/sargonxg/AGON) and [TCGC alpha benchmark](https://github.com/sargonxg/TCGC_TACITUS-Conflict-Grammar-Corpus_BENCHMARK).

</details>
