# CardSmith

**Turn your physical card collection into a digital collection without doing everything by hand.**

I'm building CardSmith because organizing a large collection of trading cards shouldn't mean spending days photographing, cropping, looking up and typing in information for every single card.

The idea is pretty simple. Take pictures of your cards, even entire binder pages, and let the software do as much of the work as possible. You should be able to go through the results, fix anything it got wrong and get on with your day.

CardSmith is still in development. I'm testing it on real collections, and there's plenty of work left before I'm comfortable calling it a finished product. This is the public page where I'm sharing the progress, not a download for the application or its source code.

## What I'm building it to do

| Feature | What it means for you |
| --- | --- |
| Bulk import | Add pictures, scans or entire binder pages, with backs if you have them. |
| Automatic cropping | Find individual cards, straighten them and get them ready to read. |
| Front/back pairing | Keep both sides of the same card together without guessing when a match is unclear. |
| Local OCR | Read visible names, years, card numbers, manufacturers and other details. |
| Identification | Look up possible matches using permitted reference data and flag anything it can't confidently identify. |
| Inventory | Keep your collection, images, search, corrections and source information in one place. |
| Optional appraisal | Look up values when you ask for them, using the identity and available market evidence. |
| Reporting | Export your collection and appraisal information. |

The goal is to get the clear, straightforward cards through automatically and leave you with the ones that actually need attention. Your original pictures and confirmed corrections should stay intact.

## Why local-first?

I don't want people to need an internet connection, an AI subscription, an API key or a paid service just to scan and organize the cards they already own.

The plan is to handle the core work locally using image processing, OCR and smaller, purpose-built models where they actually help. General-purpose generative AI isn't supposed to be a requirement.

Online research and valuation are separate and optional. Importing a card shouldn't automatically send it to an online service. If you want values, you can ask for them after reviewing the cards.

## What cards will it support?

I'm starting with baseball cards because they're a particularly difficult place to start. The plan is to expand to other sports cards, Pokémon, Yu-Gi-Oh! and Magic: The Gathering as the recognition, reference data and licensing are sorted out. Those are future goals, not categories I'm claiming are ready today.

## Where things stand

Bulk importing, local OCR, inventory, cropping, pairing and reporting are already being worked on and exercised. I'm also training and testing local specialist models. If a new model doesn't improve the results, it doesn't get added just for the sake of using AI.

One offline test processed 23 real source images into 135 processing records without recorded source or record failures. None of those records had a confirmed ID or a numeric value; they still needed review. The pipeline ran, but that doesn't mean the recognition is where I want it yet.

The biggest priorities right now are getting the crops and identification right on actual collection photos.

## Real CardSmith output

Here are a few examples of what CardSmith actually produces. Some are good, some need work. I'm showing real results, not just perfect ones.

<table>
<tr>
  <td align="center"><a href="./CardSmith-Public-Gallery/08ff2a617757327a7f5992b3dc4039b47471686e20a138c0cc2827cec61ee438.jpg"><img src="./CardSmith-Public-Gallery/08ff2a617757327a7f5992b3dc4039b47471686e20a138c0cc2827cec61ee438.jpg" alt="Representative image 1" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/1406f57608a049e84051849f9e05eba7d6e0982dbad02cb854d9830a11ac42a1.jpg"><img src="./CardSmith-Public-Gallery/1406f57608a049e84051849f9e05eba7d6e0982dbad02cb854d9830a11ac42a1.jpg" alt="Representative image 2" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/2117f3a2be111fb62949a79fa9ed57196a60fce5de615773c48dc9b59e4175f5.jpg"><img src="./CardSmith-Public-Gallery/2117f3a2be111fb62949a79fa9ed57196a60fce5de615773c48dc9b59e4175f5.jpg" alt="Representative image 3" width="180"></a></td>
  <td align="center"><a href="./CardSmith-Public-Gallery/246865722448aad196f9cae081e2fe5604dc466f0c9074edb5f41e9bfe42c239.jpg"><img src="./CardSmith-Public-Gallery/246865722448aad196f9cae081e2fe5604dc466f0c9074edb5f41e9bfe42c239.jpg" alt="Representative image 4" width="180"></a></td>
</tr>
</table>

**[Browse all 32 images](./CardSmith-Public-Gallery/README.md)** — click any picture to see it larger. These are examples, not confirmed card IDs or an accuracy benchmark.

The larger 289-image sample is separate from this gallery. I'm keeping it off the main page so you don't have to scroll through hundreds of pictures.

## What I'm working toward

| Priority | Goal |
| --- | --- |
| 1 | Better card detection, cropping and orientation on real photos. |
| 2 | More accurate front/back pairing, OCR and exact card identification. |
| 3 | Faster processing with less manual work on large collections. |
| 4 | Better inventory editing, recovery, exports and installation. |
| 5 | Get a Windows beta properly tested and expand hardware and platform testing. |
| 6 | Support more card categories and permitted reference and pricing services. |

My long-term speed target is around 10,000 cards in eight hours on suitable hardware. For accuracy, the minimum goals are at least 90% of representative crop tests reaching 90% overlap and 95% correct exact-printing identification among automatically confirmed cards, with at least 90% coverage. I haven't reached those targets on independent representative tests yet.

I'd rather have the app leave a price blank than make up a number. Zero incorrect numeric valuations is the goal.

## Get involved

If you collect, buy or sell cards, I'd like to hear what would actually make this useful for you. Suggestions, feedback and interest in testing are welcome.

- [Leave feedback or suggest a feature](https://github.com/tiddy-tickler/CardSmith/issues/new)
- [Follow the project](https://github.com/tiddy-tickler/CardSmith)

Please keep private collection information, credentials, unredacted logs and copyrighted datasets out of public issues. Test builds will be shared separately with approved testers; I don't have a public download or release date to announce yet.

## Supporting the project

I'm developing CardSmith independently. If you like the idea and want to help, sharing it, giving feedback or offering technical help all count. Financial support is entirely optional.

**[Support CardSmith on GoFundMe](https://gofund.me/729fbb185)**

## A quick note

I'm keeping the application source, internal development material and private test data separate from this showcase. This page doesn't grant a software license or permission to distribute the application.

CardSmith is meant to help identify and appraise cards, not replace professional grading or guarantee what a card will sell for. It's an independent project and isn't affiliated with or endorsed by the card brands or publishers mentioned here.
