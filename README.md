# 🛡️ SafeBite

<p align="center">
  <img src="assets/safebite-logo.svg" alt="SafeBite logo" width="480">
</p>

**Scan products. Understand ingredients. Make more informed allergy-safety decisions.**

> **Public showcase repository**  
> This repository documents SafeBite’s purpose, product direction, progress, and lessons learned. The active application source remains private while reliability, security, and data integrations are being tested.

## Why SafeBite Exists

SafeBite began as a personal solution for my family.

My daughter lives with serious allergies and eczema. Product labels can be unclear, incomplete, or changed without warning, and families often have to compare multiple sources before deciding whether a food, beauty, or household product may be appropriate.

SafeBite is being built to reduce that uncertainty by combining product lookup, ingredient visibility, personalized profiles, source transparency, and user verification guidance.

## Current Product Direction

SafeBite is evolving beyond a basic barcode scanner into a personalized product-safety assistant that can support:

- Barcode and manual product lookup
- Food, beauty, and household product categories
- Multiple family profiles and individual allergen needs
- Ingredient and allergen review
- Product-source attribution and freshness indicators
- Scan history and cached results
- Recall awareness
- Confidence and incomplete-data warnings
- Safer fallback behavior when sources disagree

## Latest Progress — July 2026

Recent work has focused on **lookup reliability, source transparency, and safer infrastructure**.

### Completed or improved

- Consolidated product-evaluation logic to reduce conflicting results
- Reduced dependence on low-value or unreliable product sources
- Improved product lookup speed through parallel requests and caching
- Added stronger handling for duplicate scans and repeated lookups
- Continued family-profile, scan-history, and product-cache workflows
- Fixed a LiveData auto-sync render loop
- Strengthened Supabase configuration and removed project-specific credentials from public documentation
- Completed a Phase 1 recovery effort centered on product lookup reliability and visible source information

### Current focus

- Improving ingredient and allergen data coverage
- Distinguishing direct allergen matches from uncertain or incomplete information
- Adding clearer confidence, source, and freshness labels
- Expanding manual search and fallback behavior
- Continuing security review and backend separation
- Preparing for broader controlled testing

## Product Challenges

SafeBite works with data that may be incomplete, inconsistent, outdated, or different across providers.

The product therefore must not treat a successful scan as proof that an item is safe. Important design requirements include:

- Showing where information came from
- Identifying missing or conflicting data
- Encouraging users to verify the physical label
- Avoiding medical guarantees
- Defaulting to caution when confidence is low

## Technology

- React Native / Expo
- TypeScript
- Supabase
- Node.js and API integrations
- Product databases and recall sources
- Local caching and structured fallback logic

## Status

**Active build and reliability phase.**

The public repository is a portfolio and progress record. It is not the current production source repository and should not be interpreted as a released medical or safety product.

## Safety Notice

SafeBite is an informational tool under development. It does not replace medical advice, emergency guidance, manufacturer confirmation, or careful review of the physical product label.

## Related Links

- [Eazy Peezy Technologies Portfolio](https://github.com/eazypeezytechnologies-ctrl/Portfolio)
- [Eazy Peezy Technologies](https://eazypeezytech.com)

## Builder

**Babatunde Jegede**  
Founder, Eazy Peezy Technologies LLC

---

**Last updated: July 8, 2026**
