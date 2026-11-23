# TACITUS

Reusable context for teams working with knowledge.

TACITUS helps a team capture its sources, working rules and the decisions behind an analysis. Attach that context as a capsule, use an artefact to guide the output, and give the next teammate the material needed to continue.

[Company website](https://tacitus.me/) · [Explore the App](https://app.tacitus.me/) · [Technology](https://tacitus.me/structures/) · [Research and evaluation](https://tacitus.me/research/)

## Three products, one research family

| TACITUS App | Wind Tunnel | DOXA |
| :--- | :--- | :--- |
| <img src="assets/tacitus-guide.v1.webp" width="59" height="88" alt="TACITUS’s original notebook-carrying guide"> | <img src="assets/wind-tunnel-kite.v1.webp" width="85" height="88" alt="Kite, Wind Tunnel’s teal pixel bird"> | <img src="assets/doxa-analyst.v1.webp" width="85" height="88" alt="DOXA’s pixel owl reading two passages"> |
| Attach and reuse your team’s context, capsules and artefacts. | Explore modeled audience responses and plan research with people. | Compare political framing and evidence in documents and speech. |
| [Open App](https://app.tacitus.me/) · [How it works](https://tacitus.me/product/) | [Open Wind Tunnel](https://windtunnel.tacitus.me/) · [Research and benchmark](https://tacitus.me/research/wind-tunnel/) | [Code and local installation](https://github.com/sargonxg/DOXA-by-TACITUS) |

Each companion identifies its product. Findings, model limitations and human review remain explicit in the working tools.

## Start with working code

The [Knowledge Pipeline](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open) builds source-linked graphs and bounded context from exact passages and authored interpretations. It includes a generic team-knowledge ontology, task layers, BM25 selection, bounded graph expansion and explicit App import.

```sh
git clone https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open.git
cd TACITUS-Knowledge-Pipeline-open/reference-pipeline
PYTHONPATH=src python -m unittest discover -s tests -v
```

[Build and import a complete handoff](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/blob/main/reference-pipeline/docs/app-import.md) · [Organization starter with a pinned implementation](https://github.com/TACITUS-me/Open_Starting_Kpipeline_TACITUS)

## Inspect the approach

- Source editions and exact quotations keep the evidence identifiable.
- Ontologies define record types and relationships. Task layers select relevant context and review questions.
- Capsules and artefacts carry working knowledge and output structure into another task.
- Authored interpretations and model proposals have explicit review states.
- Evaluation covers evidence retention, attribution, qualifications and the total cost of accepted work.

The App uses Google sign-in. Hosted generation is paused. The public compiler and its recorded-response tests run without a model account. Earlier model evaluation produced mixed results. Consistent answer-quality and efficiency gains remain to be measured.

## Related projects

[DOXA](https://github.com/sargonxg/DOXA-by-TACITUS) examines framing and attribution in documents. [Workbench](https://github.com/sargonxg/tacitus-workbench) provides source and output inspection tools. [The research index](https://github.com/sargonxg/TACITUS-Knowledge-Pipeline-open/tree/main/research) links primary papers to engineering questions.

Active code spans this organization and the founder’s account. The repository links above identify the maintained locations. Source material and third-party projects retain their own terms.

[Build a context system with TACITUS](https://tacitus.me/consulting/) · [Contact](mailto:hello@tacitus.me)
