# Trend Chaser

A checkpointed AI-assisted workflow for Printful-to-Shopify merchandise releases.

**Version:** 1.0.0 · **Creator:** Brendon R. Coleman · **License:** CC BY 4.0

**Archived release:** [10.5281/zenodo.23993469](https://doi.org/10.5281/zenodo.23993469) · [Download v1.0.0 ZIP](https://zenodo.org/records/23993469/files/noblebrendon-cloud/trend-chaser-v1.0.0.zip?download=1)

Trend Chaser takes a supplied concept or graphic through artwork preparation, print checks, product configuration, authorized publication and storefront verification. A private release record preserves completed work so an interrupted session can resume without blindly creating duplicate products.

This repository publishes the portable procedure and templates. Execution requires an active assistant session, authenticated Printful and Shopify accounts, and supported tools. No executable publishing service, API credentials, automatic trend monitor or payment automation is included.

## Use

1. Read [setup requirements](docs/SETUP.md) and configure a private copy of [operator-config.example.json](templates/operator-config.example.json).
2. Give a capable assistant [WORKFLOW.md](WORKFLOW.md), its referenced files, your configuration and the source artwork or concept.
3. Specify whether to prepare a draft or publish. The instruction below authorizes publication to your verified configured store.

**Publish invocation**

```text
Follow WORKFLOW.md. Trend Chaser: turn this image or idea into a shirt and publish it to my configured Shopify store. Save a private release record and verify the public listing before reporting completion.
```

**Draft invocation**

```text
Follow WORKFLOW.md. Trend Chaser: prepare this shirt and a review packet. Do not publish it.
```

**Resume invocation**

```text
Follow WORKFLOW.md. Resume this Trend Chaser release from its saved record. Reconcile provider and Shopify state before retrying any uncertain write.
```

Publishing a listing does not authorize purchases, social announcements or access beyond the specified accounts and concept. An installed personal adaptation may support a shorter invocation; this public package does not automatically install one.

## Files

| File | Purpose |
| --- | --- |
| [WORKFLOW.md](WORKFLOW.md) | Execution procedure and approval boundaries |
| [docs/SETUP.md](docs/SETUP.md) | Required capabilities and operator configuration |
| [templates/release-run.template.json](templates/release-run.template.json) | Blank private release record |
| [templates/operator-config.example.json](templates/operator-config.example.json) | Unconfigured operator settings |
| [references/printful-shopify.md](references/printful-shopify.md) | Generalized provider recovery observations |
| [examples/pending-publication.synthetic.json](examples/pending-publication.synthetic.json) | Explicitly synthetic retry example |
| [docs/VALIDATION.md](docs/VALIDATION.md) | Evidence, limits and acceptance checks |
| [docs/PUBLISHING.md](docs/PUBLISHING.md) | GitHub and Zenodo versioning procedure |
| [CITATION.cff](CITATION.cff) | Citation metadata |
| [LICENSE](LICENSE) | Reuse terms |

## Evidence and limits

The source workflow was derived from one owner-operated Printful-to-Shopify release completed on November 5, 2026, followed by an offline pending-publication exercise. The underlying release verified product synchronization, storefront details and a reversible cart addition. It did not test payment, physical printing or delivery. The public adaptation has not been executed against another store. See [validation notes](docs/VALIDATION.md).

Provider interfaces, product availability and prices change. Inspect current state; the reference notes are observations, not stable UI selectors or guarantees. Persistent run IDs support reconciliation but do not establish provider-enforced exactly-once execution.

The package excludes the owner's store identifiers, private file references, artwork, credentials, session data and full operational history. Keep your own release receipts and artwork outside this public repository.

## Citation and attribution

Coleman, Brendon R. (2026). *Trend Chaser: A Checkpointed AI-Assisted Workflow for Printful-to-Shopify Merchandise Releases* (Version 1.0.0). Zenodo. https://doi.org/10.5281/zenodo.23993469

The workflow and documentation were developed with assistance from ChatGPT/Codex. Brendon R. Coleman supplied the goals, release direction and publication instructions. AI assistance is disclosed without assigning it authorship or claiming independent peer review.

This workflow documentation and its templates are licensed under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). Provider names identify dependencies and imply no affiliation or endorsement. The license does not grant rights to separately supplied shirt artwork, trademarks or third-party services.
