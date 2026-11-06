# Printful-to-Shopify recovery notes

These generalized observations come from a single owner-operated release on November 5, 2026. Verify the current interface and tool capabilities before acting. UI labels, available products and field behavior may change.

## Destination and file transport

- Two stores can share a display name but use different integration types. Verify the Shopify-linked destination and matching product evidence before selecting a store.
- An assistant workspace and a connected browser's device may have different filesystems. Use a supported transfer route and an actual device-local path for browser upload controls.
- Start a supported file-chooser wait before clicking a visible upload control. Do not invent paths or target hidden inputs without current evidence and permission.
- Externally hosting an asset is a separate write within the authorized release scope. Do not use public hosting as a general transfer route for private files.
- After an upload or download timeout, inspect existing state before retrying. Apply the production artwork to the new design; never apply a shirt mockup as print art.

## Print preflight

Calculate effective PPI as pixel dimensions divided by physical print dimensions. Image bounds can include empty margins, so inspect visible artwork in the provider preview. Acceptability depends on the selected product and provider checks. No fixed size or PPI in this repository guarantees acceptable output.

If reducing physical dimensions resolves a warning but materially changes the desired design, show the actual alternatives to the operator. Upscaling does not establish recovered detail. Inspect any background-removal result for edge artifacts and unintended changes; obey current image-editing instructions.

## Editor and publish wizard

- Input text can change without committing application state. Check derived dimensions, warnings, earnings or previews. A normal confirmation key or ordinary typing/change event may be needed; inspect after each recovery.
- Actual printed-front mockups should lead the listing. A default selection can put a plain back first.
- Verify final prices for every intended variant and read current cost and shipping treatment. Do not treat old prices as live evidence.
- Confirm the title, description and size guide are committed before publication.
- Treat queued or pending pushes as asynchronous. Reconcile before submitting another write.

## Shared template mismatch

A correct Admin description can coexist with incorrect public copy if a theme uses static text. Compare both views.

When authorized and supported, prefer a verified dynamic product template or an isolated product-specific template. Preserve unrelated products, the shared default and the operator's unsaved work. In the observed repair, existing rich text had to be cleared before binding the current product description; connecting a dynamic source alone appended to the old content.

Verify the final public description and size guide after the assignment. Do not publish an unrelated theme or alter every product to fix one listing.

## Verification and cleanup

Check provider synchronization and fulfillment mappings, Shopify status and online-store publication, prices, title and media. Test one exact visible variant in the cart when practical. Record prior cart contents, add one unit, verify title/size/price, remove only the test addition and restore the prior state. Handle an already-present variant by restoring its original quantity.

A transient empty drawer after adding can be an asynchronous UI state; inspect the settled result. Do not proceed to payment or place an order. Report unavailable checks as unverified and distinguish live image links from successfully completed downloads.
