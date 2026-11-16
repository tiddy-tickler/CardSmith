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

Browse the 32-image owner-approved gallery below. These original CardSmith crop outputs show varied source quality, front and back roles, and examples marked for review. The gallery is illustrative material, not a labeled benchmark and not evidence of recognition accuracy.

<table>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/08ff2a617757327a7f5992b3dc4039b47471686e20a138c0cc2827cec61ee438.jpg"><img src="./CardSmith-Public-Gallery/08ff2a617757327a7f5992b3dc4039b47471686e20a138c0cc2827cec61ee438.jpg" alt="Representative image 1" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/1406f57608a049e84051849f9e05eba7d6e0982dbad02cb854d9830a11ac42a1.jpg"><img src="./CardSmith-Public-Gallery/1406f57608a049e84051849f9e05eba7d6e0982dbad02cb854d9830a11ac42a1.jpg" alt="Representative image 2" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/2117f3a2be111fb62949a79fa9ed57196a60fce5de615773c48dc9b59e4175f5.jpg"><img src="./CardSmith-Public-Gallery/2117f3a2be111fb62949a79fa9ed57196a60fce5de615773c48dc9b59e4175f5.jpg" alt="Representative image 3" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/246865722448aad196f9cae081e2fe5604dc466f0c9074edb5f41e9bfe42c239.jpg"><img src="./CardSmith-Public-Gallery/246865722448aad196f9cae081e2fe5604dc466f0c9074edb5f41e9bfe42c239.jpg" alt="Representative image 4" width="180"></a></td>
</tr>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/2669fcda8830e87fa4ca97a7052a049545e226017c18999a694838807a2468d3.jpg"><img src="./CardSmith-Public-Gallery/2669fcda8830e87fa4ca97a7052a049545e226017c18999a694838807a2468d3.jpg" alt="Representative image 5" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/332332f6de819bca13ca271a4bdc4090229072be5370b6021c77c9b8134fb693.jpg"><img src="./CardSmith-Public-Gallery/332332f6de819bca13ca271a4bdc4090229072be5370b6021c77c9b8134fb693.jpg" alt="Representative image 6" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/3e4189482dadf99f9e95c761e950a60c14e7d890fe7d3deefb8b03a4c70a008c.jpg"><img src="./CardSmith-Public-Gallery/3e4189482dadf99f9e95c761e950a60c14e7d890fe7d3deefb8b03a4c70a008c.jpg" alt="Representative image 7" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/42e70e2949f51e0e171557a4cb2e13c5d066fd66a0477b01b5c04132481a63af.jpg"><img src="./CardSmith-Public-Gallery/42e70e2949f51e0e171557a4cb2e13c5d066fd66a0477b01b5c04132481a63af.jpg" alt="Representative image 8" width="180"></a></td>
</tr>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/4967440f15186c059ca35fbd67cc83c90afe82f15026ed5bc35df412121596e4.jpg"><img src="./CardSmith-Public-Gallery/4967440f15186c059ca35fbd67cc83c90afe82f15026ed5bc35df412121596e4.jpg" alt="Representative image 9" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/4a6c5dd732fcc820f729453abf4d015782dbf70e443e3112ce9f5889b265b11d.jpg"><img src="./CardSmith-Public-Gallery/4a6c5dd732fcc820f729453abf4d015782dbf70e443e3112ce9f5889b265b11d.jpg" alt="Representative image 10" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/4b6ab444a25487acc5153ea90014be90bea52e1aaaa777ad7746179e76fce0a0.jpg"><img src="./CardSmith-Public-Gallery/4b6ab444a25487acc5153ea90014be90bea52e1aaaa777ad7746179e76fce0a0.jpg" alt="Representative image 11" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/64a242cefa9f5efe33bd87171f0a97fed0d5e2d74394d1ebd5759a5072514f2e.jpg"><img src="./CardSmith-Public-Gallery/64a242cefa9f5efe33bd87171f0a97fed0d5e2d74394d1ebd5759a5072514f2e.jpg" alt="Representative image 12" width="180"></a></td>
</tr>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/6bfa61b1159fb2469beade65bc744c95f40be9d6b4971965e9c7522815e65e2d.jpg"><img src="./CardSmith-Public-Gallery/6bfa61b1159fb2469beade65bc744c95f40be9d6b4971965e9c7522815e65e2d.jpg" alt="Representative image 13" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/88c25c7796c83bd82c5f7c2d203604e84d670632297ce59c0153fcec77ff5f36.jpg"><img src="./CardSmith-Public-Gallery/88c25c7796c83bd82c5f7c2d203604e84d670632297ce59c0153fcec77ff5f36.jpg" alt="Representative image 14" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/88e2eb4f0df50d27611bfaadf731f8127841b4094b05d1efff06b93114d37326.jpg"><img src="./CardSmith-Public-Gallery/88e2eb4f0df50d27611bfaadf731f8127841b4094b05d1efff06b93114d37326.jpg" alt="Representative image 15" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/8e5504f812a185a08ee779a6ec255135889dcaab895792dcb8b0a776d749d913.jpg"><img src="./CardSmith-Public-Gallery/8e5504f812a185a08ee779a6ec255135889dcaab895792dcb8b0a776d749d913.jpg" alt="Representative image 16" width="180"></a></td>
</tr>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/9c55bd255782e94885a36763e179b623116e7308993a4029f56036648a48789f.jpg"><img src="./CardSmith-Public-Gallery/9c55bd255782e94885a36763e179b623116e7308993a4029f56036648a48789f.jpg" alt="Representative image 17" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/beabdcf7f275a953a010a34ad7167a1cf9d4fe3afbba811029e89d3e93903e5e.jpg"><img src="./CardSmith-Public-Gallery/beabdcf7f275a953a010a34ad7167a1cf9d4fe3afbba811029e89d3e93903e5e.jpg" alt="Representative image 18" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/c1b820e59a1dc00cad5c61e8fb8df61f68192fd60c742aa294ec27520ca1d48c.jpg"><img src="./CardSmith-Public-Gallery/c1b820e59a1dc00cad5c61e8fb8df61f68192fd60c742aa294ec27520ca1d48c.jpg" alt="Representative image 19" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/ca3b697e6211a09da9ca42a2b955cfebc8286819b36dc25e2007f52abb1c7bba.jpg"><img src="./CardSmith-Public-Gallery/ca3b697e6211a09da9ca42a2b955cfebc8286819b36dc25e2007f52abb1c7bba.jpg" alt="Representative image 20" width="180"></a></td>
</tr>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/cb8cfab0ae05230bd2b807698d85668cddc573edbbad21ebfd8ae3982d1def80.jpg"><img src="./CardSmith-Public-Gallery/cb8cfab0ae05230bd2b807698d85668cddc573edbbad21ebfd8ae3982d1def80.jpg" alt="Representative image 21" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/d7ca87497c9b26cc4428092305a315876dbafff71bb69c51f86082415daef94d.jpg"><img src="./CardSmith-Public-Gallery/d7ca87497c9b26cc4428092305a315876dbafff71bb69c51f86082415daef94d.jpg" alt="Representative image 22" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/d7fff56ecd1068d11171ae7c8c896793603739ff190fc4f07b815d5c9d288606.jpg"><img src="./CardSmith-Public-Gallery/d7fff56ecd1068d11171ae7c8c896793603739ff190fc4f07b815d5c9d288606.jpg" alt="Representative image 23" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/d930593e6c055501dcc96cda0aa934064e904259c843f1cef9340d08edef3e41.jpg"><img src="./CardSmith-Public-Gallery/d930593e6c055501dcc96cda0aa934064e904259c843f1cef9340d08edef3e41.jpg" alt="Representative image 24" width="180"></a></td>
</tr>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/e4b640313d168ea55301922061de51f6d619c816c1d40d5e2ec03fa32bcddba7.jpg"><img src="./CardSmith-Public-Gallery/e4b640313d168ea55301922061de51f6d619c816c1d40d5e2ec03fa32bcddba7.jpg" alt="Representative image 25" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/e85748a0f409f5fce87f20a648ddbbef81a2d56f3a2caa5ddf9f42944c8ba0f0.jpg"><img src="./CardSmith-Public-Gallery/e85748a0f409f5fce87f20a648ddbbef81a2d56f3a2caa5ddf9f42944c8ba0f0.jpg" alt="Representative image 26" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/e963b28f45e19a88be91be1c14599a6194f57f932019f9e65f5ddf1fa5bcea0d.jpg"><img src="./CardSmith-Public-Gallery/e963b28f45e19a88be91be1c14599a6194f57f932019f9e65f5ddf1fa5bcea0d.jpg" alt="Representative image 27" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/ea1fa9a30df8959509707940d1a1d92eb86b538f3d1a8ef59297b78a9c5e8b79.jpg"><img src="./CardSmith-Public-Gallery/ea1fa9a30df8959509707940d1a1d92eb86b538f3d1a8ef59297b78a9c5e8b79.jpg" alt="Representative image 28" width="180"></a></td>
</tr>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/eb41d8e60779111b38f6d6fa501c105d6badfc2bc39faec171b377fbfe7d90f1.jpg"><img src="./CardSmith-Public-Gallery/eb41d8e60779111b38f6d6fa501c105d6badfc2bc39faec171b377fbfe7d90f1.jpg" alt="Representative image 29" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/f09c67f06dafb48c872ee7f3d81a909223063376a172f1a1682c6450b7f56409.jpg"><img src="./CardSmith-Public-Gallery/f09c67f06dafb48c872ee7f3d81a909223063376a172f1a1682c6450b7f56409.jpg" alt="Representative image 30" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/f98bd2668407e7d5381712071e8bfff01a0bbcf6e1dded4252241d039bb4dbc3.jpg"><img src="./CardSmith-Public-Gallery/f98bd2668407e7d5381712071e8bfff01a0bbcf6e1dded4252241d039bb4dbc3.jpg" alt="Representative image 31" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/fff0822f5a6efcb08c377b63d6941aa120c72957bb4eae2d14a9e1a5d8df2066.jpg"><img src="./CardSmith-Public-Gallery/fff0822f5a6efcb08c377b63d6941aa120c72957bb4eae2d14a9e1a5d8df2066.jpg" alt="Representative image 32" width="180"></a></td>
</tr>
</table>

The original-quality 289-image sample is distributed separately through the private tester channel. It is not included in this public repository.

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
