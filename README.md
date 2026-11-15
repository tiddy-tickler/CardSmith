# CardSmith

**From physical trading cards to an organized digital collection.**

CardSmith is a local-first trading card identification, automated image processing, collection management and evidence-based appraisal application currently in active development.

The idea is simple: photograph your collection, including entire binder pages, and let CardSmith do as much of the repetitive work as possible. Instead of manually photographing, cropping, researching and entering every individual card, collectors should be able to build a digital inventory and spend their time reviewing genuine exceptions.

> **Development status:** Commercial beta in development. Selected workflows have been exercised on real collections, but automatic crop and identification accuracy, performance and release readiness are still being qualified. This repository is a public project showcase, not a software download or source-code release.

## What CardSmith is being built to do

| Capability | Intended experience |
| --- | --- |
| Bulk import | Import individual card photographs, scans or entire binder pages, including optional back images. |
| Automatic card isolation | Detect individual cards, crop them, correct perspective and orient them for reading. |
| Front/back pairing | Associate both views of the same physical card without silently merging ambiguous cards. |
| Local recognition | Extract visible names, numbers, dates, manufacturers and other identifying information using local OCR and image analysis. |
| Card identification | Compare visible evidence with permitted reference data and distinguish confirmed, provisional and unresolved identities. |
| Collection management | Maintain a persistent inventory with card images, provenance, search, review and corrections. |
| Optional appraisal | Research value only when explicitly requested, with sufficient identity and market evidence. |
| Reporting | Export collection information and appropriate appraisal reports. |

The goal is to process routine clear cards with minimal manual intervention, while giving collectors practical tools to review and correct uncertain results. Original photographs and verified corrections are intended to remain preserved across processing runs.

## Local-first by design

CardSmith is intended to operate without a mandatory internet connection, cloud AI account, API key or paid service for core image processing, recognition using local evidence, and inventory management.

Online market research and other optional connected services are separate from normal offline processing. Nothing should be automatically sent to an online valuation service simply because a card has been scanned.

CardSmith is being developed to use efficient conventional image processing, local OCR and appropriately qualified task-specific models. General-purpose generative AI is not intended to be a required runtime component.

## Cards and collections

Baseball cards are the initial development and testing focus. The broader goal is support for other sports cards and trading card games, including Pokémon, Yu-Gi-Oh! and Magic: The Gathering.

Expansion depends on appropriate recognition accuracy, reference data, licensing and independent qualification. These additional categories are planned scope, not currently verified support.

## Development progress

Current development includes working bulk-ingestion, local OCR, persistent inventory, crop and pairing workflows, reporting, and experimental local specialist training.

A documented offline development replay processed 23 real source images into 135 processing records without recorded source or record failures. All records remained review-gated; none had a confirmed identification or numeric valuation. This demonstrates pipeline execution, not crop or identification accuracy. Real-world isolation and recognition remain the main development priorities.

Experimental models are compared against existing methods before adoption. Candidates that make results worse or fail to provide useful coverage are not promoted into the default processing path.

## Representative development images

A 289-image representative sample has been reviewed for archive integrity. It contains real photographs of binder pages and individual card images, including clearer examples, card backs, glare, rotation, incomplete crops and other genuine processing difficulties.

The sample contains 289 distinct JPEG files, approximately 497 MB in total. It is illustrative development evidence, not a labeled benchmark or a demonstrated recognition-accuracy result.

A smaller browsable gallery and the original-quality sample archive are being prepared for publication. The archive is not currently available as a public download.

## Roadmap

| Priority | Goal |
| --- | --- |
| 1 | Improve real-world card boundary detection, isolation and orientation. |
| 2 | Improve front/back association, local text recognition and exact card identification. |
| 3 | Reduce processing time and unnecessary manual review for large collections. |
| 4 | Strengthen inventory correction, recovery, export and installation workflows. |
| 5 | Qualify a controlled Windows beta and expand hardware and platform testing. |
| 6 | Extend card-category coverage and permitted reference and valuation integrations. |

The engineering target is approximately 10,000 cards in an eight-hour work period on suitable hardware. This is a development objective, not an achieved benchmark.

The minimum release accuracy objectives include at least 90% of independently evaluated crop cases meeting a 90% overlap floor, and at least 95% exact-printing identification accuracy among automatically confirmed cases with at least 90% coverage of representative evaluated cases. Numeric valuations must abstain when identity or market evidence is insufficient. These objectives have not yet been achieved on representative independent evidence.

## Get involved

Collectors, card dealers and hobbyists are welcome to share feedback on the workflows they would find useful.

- [Suggest a feature or share feedback](https://github.com/tiddy-tickler/CardSmith/issues/new)
- [Follow project updates](https://github.com/tiddy-tickler/CardSmith) by watching this repository.

Please do not post private collection data, unredacted diagnostics, credentials, personal information or copyrighted datasets in public issues.

Controlled test builds will be distributed separately to approved testers. Public downloads and release dates are not being promised at this stage.

## Support CardSmith development

CardSmith is an independently developed project. Community involvement helps improve its recognition accuracy, usability and compatibility with real collections.

Financial support is entirely optional. Sharing the project, offering constructive feedback, volunteering relevant technical expertise, or expressing interest in controlled beta testing are also valuable ways to help.

If you would like to support the ongoing development effort financially, the project's fundraiser is available here:

**[Support CardSmith on GoFundMe](https://gofund.me/729fbb185)**

## About this repository

This public repository is for project information, progress updates and approved demonstrations. The application source code, internal development history, private fixtures and experimental artifacts are maintained separately. No software license or distribution permission is granted by this showcase.

CardSmith provides evidence-based identification and appraisal assistance, not professional card grading or guaranteed market values.

CardSmith is an independent project and is not affiliated with or endorsed by the card brands or publishers mentioned above.
