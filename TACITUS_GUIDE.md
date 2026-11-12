# TACITUS · House of Evidence: purpose and current stage

Understand how exact sources become task context and reviewable artifacts.

**Stage:** Organization introduction and synthetic teaching game; application readiness is listed separately.

## Play the idea

```sh
python -m http.server 8765 --bind 127.0.0.1 --directory tacitus-demo
```

Open http://127.0.0.1:8765/. In the original 8-bit mansion, recover a source condition, preserve attribution, distinguish event time from publication time, review the synthetic case and export a teaching brief. The game is an original point-and-click lesson inspired by 1980s adventures; it contains no copied game assets. [Credits and research](tacitus-demo/CREDITS.md).

The lesson is separate from application execution. Its teaching JSON is not a native capsule import or a deployment receipt. It makes no model calls and needs no account.

## Why this belongs to TACITUS

TACITUS builds data structures → task-specific context → inspectable artifacts for policy and political AI. A deployer should be able to identify exact source versions, retained conditions, omitted evidence and the review still required. Smaller context is useful only if the distinctions needed for the task survive.

## Research and attribution

- [Lewis et al., 2020, Retrieval-Augmented Generation](https://arxiv.org/abs/2005.11401): retrieval supplies external evidence; our source/version receipts make the handoff inspectable. This is not a reproduction of their benchmark.
- [Liu et al., 2023, Lost in the Middle](https://arxiv.org/abs/2307.03172): a long prompt does not ensure reliable use of evidence; retain exceptions alongside the selected claim. No quality gain is inferred from fewer tokens.
- [Edge et al., 2024, From Local to Global](https://arxiv.org/abs/2404.16130): graph indexing and community summaries address corpus-level questions. Authored TACITUS relations are distinct from that extraction/summarization method.
- [W3C PROV](https://www.w3.org/TR/prov-overview/): distinguish source entities, processing activities and responsible agents. No full standards-conformance claim is made.

[Detailed methods, upstream credit and evaluation limits](https://github.com/sargonxg/sargonxg/blob/main/docs/RESEARCH_AND_DESIGN.md). Existing licenses and third-party source rights remain authoritative. Graph edges, citation matches and hashes do not establish truth, causation or expert approval.

## Profile implementation

GitHub renders `profile/README.md` as the organization home. The public project selector names maintained sources and distinguishes local verification from hosted operation. No private repository inventory is published.
