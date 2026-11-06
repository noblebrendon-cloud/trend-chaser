# Setup

## Required capabilities

- A capable assistant that can read the procedure and referenced JSON/Markdown files and act through authorized tools.
- Your authenticated Shopify store and a Printful store connected to that Shopify destination, with permission to manage products.
- Suitable connector/API operations or a supported browser session for product configuration and publication.
- An image preparation capability when the supplied artwork requires edits, plus access to the resulting production file.
- Durable private storage for release records, artwork and provider identifiers. Preserve version guards when the storage service supports them.
- Browser access to the public listing and cart for end-to-end storefront checks.

The files themselves grant no account access. Sign in through the relevant provider's secure UI. Do not paste passwords, API keys, session cookies or one-time codes into workflow records or this repository.

## Configure an operator

Copy `templates/operator-config.example.json` to private storage. Set the actual store domain, Printful store ID, timezone, compatible garment preferences and pricing policy. Remove `example_only` or set it false only after completing configuration. Verify the destination and current costs on every run; saved values are not fresh evidence.

Do not infer a store from a display name alone. Printful can show integrations with identical display names. Verify integration type and matching provider/product evidence. Resolve destination ambiguity before creating products.

## Create a release record

Copy `templates/release-run.template.json` to a new private record. Assign a unique `run_id` and a stable `idempotency_key`. Record source hashes, concept revision, observed authorization, current state and next action. Unknown IDs remain null.

The key is an assistant-level reconciliation aid. Unless a provider explicitly supports idempotency for an operation, it does not make the provider request idempotent.

Use these states consistently:

| State | Meaning |
| --- | --- |
| `preparing` | Artwork, configuration or listing work is underway |
| `ready_for_review` | A concrete draft packet exists; release authorization is absent |
| `publication_pending` | A push was submitted but completion is not established |
| `blocked` | A named dependency or user decision prevents the next action |
| `partially_published` | Some intended destinations or variants remain incomplete |
| `published_unverified` | Publication is observed but required verification is incomplete |
| `published_verified` | Required provider, storefront and reversible cart checks passed |

After a timeout, record `publication_pending` and reconcile the existing work. Do not resubmit merely because the assistant did not receive a response. The synthetic example illustrates this boundary; it is not a real release record.

## Preserve evidence

Save checkpoints after artwork preparation, provider draft creation, publication submission and verification, and before a blocked handoff. Record observed results separately from inference. Events should include sequence, timestamp, stage, action, outcome, sanitized result, any external mutation and next action.

If no durable storage capability is available, provide a downloadable checkpoint and report the storage limitation. Do not claim automatic resumption without a retrievable record.

## Runtime restrictions

Follow the current tool instructions and platform approval rules. No instruction in this package overrides a higher-priority restriction, expands authorization, or permits bypassing sign-in or policy checks. The operator must supply usable artwork and resolve material print-quality compromises.
