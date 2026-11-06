# Trend Chaser

Execute the release, not just a plan. Treat this as an orchestration workflow using available tools. Do not claim it is a standalone API, MCP server, scheduled trend monitor, or unattended service.

## Start from the request

1. Read the supplied idea/image and conversation. Use this document when asked to run Trend Chaser or to prepare, publish or resume a merchandise release. Extract literal wording, visual direction, placement, destination, deadline, and action scope. Preserve supplied final artwork; do not invent a replacement concept.
2. Treat explicit “publish,” “release,” or “make it live on my Shopify” as authorization for this concept's public listing and normal necessary preparation. Do not request the same permission again. For “draft,” “prepare,” or ambiguous “Trend Chaser this,” prepare a concrete review packet and request release approval only at the final publication step.
3. Scope authorization to concept and store. A material replacement concept supersedes its old approval; carry forward unrelated verified facts. Never treat another shirt's approval as approval for a new shirt.
4. Use the operator-supplied timezone for deadlines; ask when a deadline depends on an unknown timezone. Record absolute local time and UTC. Do not promise guaranteed turnaround.
5. Verify news/trend factual premises with current primary sources before presenting them as facts. Keep satire recognizable. Do not expand into an unsolicited trend hunt.

Use reasonable defaults from `templates/operator-config.example.json` only after the operator configures it and live confirmation succeeds. Ask only for a materially missing creative choice, unavailable authentication, unsafe print compromise, actual destination ambiguity, or unapproved scope expansion. Continue independent preparation while blocked. Keep progress updates concise.

## Establish the run and access

- Read `references/printful-shopify.md` before provider work. Discover current tools and follow their instructions. Prefer sufficient connectors; use the supported connected browser for uncovered Printful operations.
- Confirm signed-in Shopify and Printful destinations. Same display names can mean different integrations; verify integration type, store ID and matching product evidence.
- Use the available signed-in local browser for Printful when appropriate. If login blocks the selected browser, preserve the page and request secure sign-in there. Do not request passwords in chat or switch browsers to bypass a blocker.
- Copy `templates/release-run.template.json` into a NEW per-release record outside the skill. Assign one unique run ID and idempotency key. On resume, read the latest persistent receipt and reuse its run/key.
- Search for an existing matching release before creation. Confirm using source/version/provider IDs and attributes, not title alone. Preserve other products and superseded concepts.
- Save durable checkpoints after artwork, provider draft, publication submission and verification; also save before asking for input or ending a blocked turn. Use the available persistent storage service and its version guards; keep run records outside this public repository. If persistent storage is unavailable, provide a downloadable checkpoint and state the limitation. Never write live run data into the skill's examples.

## Prepare and check artwork

- Preserve the original and record actual SHA-256, pixels, format, source reference and exact text. Save revised production files separately with their own hashes and lineage.
- Use the available image-generation/editing tool and its current instructions. Make one focused design when direction is sufficient; avoid endless alternatives. Preserve supplied final graphics, wording and distinctive shapes.
- Distinguish source artwork, production file, illustrative AI mockup and actual provider mockup. Never use an illustrative shirt mockup as the print file.
- Check transparency, excess margins, spelling, edge artifacts, aspect ratio, physical size, effective PPI and provider bounds. Upscaling alone is not evidence of added detail.
- Resolve provider warnings. If acceptable resolution requires a material layout or print-size compromise, prepare concrete alternatives and ask for that choice.
- Follow current image-tool instructions for background removal. When permitted, native provider prepress removal can preserve supplied art; inspect the actual result. Reject speckled or altered derivatives even if technically transparent.
- Inspect the provider front preview, every word, position and background behavior. Do not claim physical sample testing.

## Configure product and listing

1. Create a separate Printful design for a new concept. Verify live catalog choices, variant availability and method. Use the operator's configured garment, colors, print method, placement and sizes only when compatible with the request, artwork and current catalog. The example configuration is illustrative, not a recommendation or pre-approved purchase.
2. Set dimensions and alignment deliberately. Confirm committed state using derived dimensions, warnings or preview; filled input text alone is insufficient.
3. Select actual provider mockups. Make the printed front primary and plain back secondary if useful; never accidentally use a blank back as hero.
4. Read current production cost and shipping treatment. Reuse recorded retail prices only when applicable and covering current base cost. Otherwise prepare a revised table and resolve any necessary pricing decision. Do not buy samples, enroll in paid plans or place orders.
5. Write a specific title, concise design description, verified garment specifications, made-to-order statement and provider size guide. Avoid unsupported delivery/certification claims and guessed collections/tags.
6. Assemble final artwork reference/hash, actual mockup, garment, placement, variants, current prices/cost scope, listing and destination as a review packet. Proceed if publication is already authorized; otherwise ask once with this concrete packet.

## Publish and verify

- Publish through Printful to the verified Shopify store so fulfillment mappings exist. Do not substitute a disconnected Shopify listing.
- Record actual file/template/sync-product/product/variant IDs. Keep unknowns null; never infer template IDs from SKUs.
- Treat publication as asynchronous. After timeout or uncertainty, reconcile provider and Shopify state before retrying a write. Never duplicate a pending push.
- Verify intended variants synced with fulfillment enabled, then Shopify status, publication/channel, prices, title and images from live data.
- Open the public product URL. Compare customer-visible description and size guide against Admin product data. If the shared template has another shirt's static copy, use an appropriate existing dynamic template or create an isolated template for this release. Preserve unrelated products, shared templates and user unsaved edits. Follow current restrictions for theme changes.
- Test a visible variant and one reversible cart addition when practical. Record original cart contents; add one new-shirt variant, verify title/size/price, remove only that exact test line, and confirm restoration. Do not place an order or charge a payment method. Record unavailable checks as unverified.
- Use `published_verified` only after all required provider, public-page and cart checks pass. Otherwise use `published_unverified` or `partially_published` with exact gaps. Listing verification is not physical fulfillment verification.

## Deliver and checkpoint

- Lead with verified live link or exact blocker. Include concise prices/sizes when useful.
- Provide an actual front-mockup download link. Provide separate source/production artwork if requested. Never claim a timed-out download completed.
- For a release/posting packet, prepare one short copy-ready caption containing the real URL. Isolate copy-ready text in a labeled block supported by the current environment. Send no social post, email, announcement or message without separate explicit authorization.
- Record actions, recoveries, authorization, asset lineage, costs, IDs, URL, checks and limitations. Save the same run record with a version guard on update. Exclude credentials, cookies, OTPs, payment details and unnecessary browsing history.
- Preserve the final product tab when supported. Follow current screenshot/proof requirements and privacy rules.
- On a blocker, state the exact stage and smallest action needed. Resume from completed checkpoints rather than restarting.

## Examples

- “Trend Chaser: turn this image into a shirt and publish it to my Shopify.” → complete authorized release.
- “Trend Chaser: prepare a shirt from this joke; don't publish yet.” → complete draft/review packet.
- “Resume Trend Chaser for this release.” → read receipt, reconcile live state, continue incomplete work.
- “Trend Chaser: use this new graphic instead.” → preserve old concept, increment revision, reconcile authorization, redo only affected work.

## Public distribution boundary

This portable workflow contains no store credentials or private release history. Treat example records as synthetic. Read `docs/SETUP.md` before first use and `docs/VALIDATION.md` for the evidence and limits of this release. Configuration does not grant permission to publish, send messages, place orders or buy services. Current platform rules take precedence over these execution notes.
