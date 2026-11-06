# Validation and limitations

## Source evidence

The source personal workflow followed one completed owner-operated shirt release on November 5, 2026. The operational record reports eight variants synchronized from Printful to Shopify, an active public product, verified prices and media, a product-specific description/size-guide repair, and a reversible cart addition with cleanup.

The source workflow package passed structural validation. An offline assistant exercise then received a pending Printful push, missing product IDs, a matching approved concept and existing publication authorization. It returned a pending status, preserved authorization, required reconciliation before retry and avoided claiming publication or creating a duplicate. No live write occurred in that exercise.

These are limited operational observations, not a controlled performance study, independent audit, or guarantee of reliability. The private store log is intentionally excluded from public distribution. The public adaptation removes store-specific settings and replaces storage-specific instructions with capability-based requirements.

## Public package checks

Before release, check JSON/YAML parsing, local documentation links, required templates, absence of owner-specific operational identifiers and agreement between version, creator and license metadata. Review the package file list before archiving it.

The synthetic example is explicitly labeled and must remain `publication_pending`. Unknown provider IDs and URLs stay null. Do not treat it as a completed release or a reusable live authorization.

## Acceptance checks for an actual run

1. Verify the destination integration and authorized concept.
2. Inspect artwork, physical print dimensions and provider warnings.
3. Verify selected variants, current costs, retail prices and front mockups.
4. Preserve actual provider IDs and checkpoint publication submission.
5. Reconcile any timeout before another write.
6. Verify provider mappings, public listing and prices.
7. Compare public description and size guide with the intended product data.
8. Verify a reversible cart addition and restore the prior cart state.
9. Deliver the actual URL and asset links with precise verification limits.

## Not established

- Physical printing quality, order payment, fulfillment or delivery.
- Successful execution of this public adaptation on another account, provider region or garment.
- Guaranteed execution time, profit margin or availability.
- Provider-enforced idempotency or exactly-once publication.
- Autonomous monitoring, scheduling, a standalone API or an MCP server.
- Compatibility with every assistant or future version of a provider interface.

Future releases should record additional tests without converting unobserved outcomes into claims of success.
