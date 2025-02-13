---
title: "Challenge Overview"
hide_table_of_contents: true
---

<head>
  <html data-theme="dark" />

  <meta
    name="description"
    content="A $250,000 machine learning and computer vision competition"
  />

  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://scrollprize.org" />
  <meta property="og:title" content="Vesuvius Challenge" />
  <meta
    property="og:description"
    content="A $250,000 machine learning and computer vision competition"
  />
  <meta
    property="og:image"
    content="https://scrollprize.org/img/social/opengraph.jpg"
  />

  <meta property="twitter:card" content="summary_large_image" />
  <meta property="twitter:url" content="https://scrollprize.org" />
  <meta property="twitter:title" content="Vesuvius Challenge" />
  <meta
    property="twitter:description"
    content="A $250,000 machine learning and computer vision competition"
  />
  <meta
    property="twitter:image"
    content="https://scrollprize.org/img/social/opengraph.jpg"
  />
</head>

The objective of the Vesuvius Challenge is to make history by reading an unopened Herculaneum scroll for the very first time. We believe that an open competition will accelerate progress and enable us to achieve this goal in 2023.

<div>We are providing all contestants with the following resources:</div>

- **[Prizes](/overview#grand-prize-150000)**: $250,000 in prizes, including a $150,000 Grand Prize and $100,000 in [Progress Prizes](/overview#progress-prizes-100000). The first progress prize is a [$50,000 ink detection competition on Kaggle](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection).
- **[Data](/data)**: 3D X-ray scans of two unopened scrolls from Herculaneum, and scans and images of three papyrus fragments
- **[Tutorials and tools](/tutorial1)**: the current best tools and techniques for virtually unwrapping papyrus scrolls
- **[Community](/participate)**: a Discord server where you can connect with other contestants and the Vesuvius Challenge team

### Join the community

- Join our [Discord server](https://discord.gg/6FgWYNjb4N) to ask questions, learn about what is going on, hang out with fellow contestants and interested onlookers, and perhaps find teammates.
- Receive updates every 1-2 weeks from our [mailing list on Substack](https://scrollprize.substack.com).
- Follow [@scrollprize](https://twitter.com/scrollprize) on Twitter.

Our team is available for any questions and feedback on Discord. You can also email us at team@scrollprize.org.


### Grand Prize ($150,000)

The Grand Prize will go to the first team to read four passages of text from the inside of the two intact scrolls. More details on the qualifying criteria are available [here](/participate).

Here are the scrolls in question:

<div className="flex w-[100%]">
    <div className="w-[100%] mb-2 mr-2"><img src="/img/overview/scroll1-small.jpg" className="w-[100%]"/><figcaption className="mt-0">Scroll 1</figcaption></div>
    <div className="w-[100%] mb-2"><img src="/img/overview/scroll2-small.jpg" className="w-[100%]"/><figcaption className="mt-0">Scroll 2</figcaption></div>
</div>

We have provided you with 8µm 3D X-ray scans of each of these scrolls, which you can find [here](/data). Your job is to extract the text from these scans.

You can approach this challenge through any means necessary: machine learning, computer vision, or machine-assisted tools operated by humans.

<figure>
  <video autoPlay playsInline loop muted className="w-[100%]" poster="/img/overview/scroll-inside-animation-4.jpg">
    <source src="/img/overview/scroll-inside-animation-4.webm" type="video/webm"/>
    <source src="/img/overview/scroll-inside-animation-4.mp4" type="video/mp4"/>
  </video>
  <figcaption className="mt-0">3D X-ray scan of a scroll <a href="https://www.youtube.com/watch?v=PpNq2cFotyY">(source)</a></figcaption>
</figure>

#### Why is this difficult?

As you will read in the [tutorials](/tutorial1), advanced tools and techniques exist for virtually unwrapping papyrus scrolls. This was demonstrated in 2015 when Dr. Seales's team [unwrapped the En-Gedi scroll](https://www2.cs.uky.edu/dri/the-scroll-from-en-gedi/), and in their recent result [identifying ink from 3D X-ray scans in the Herculaneum scrolls](https://raw.githubusercontent.com/educelab/EduceLab-Scrolls/main/paper/EduceLab-Scrolls.pdf).

<div>But the Herculaneum scrolls have proved more challenging. The remaining challenges include:</div>

- Segmenting the scrolls. The Herculaneum scrolls are especially long, tightly wrapped, damaged, and distorted. To date, no one has successfully done a large-scale segmentation of these scrolls to identify the surfaces of all the rolled layers.
- Finding the ink. The ink used in the Herculaneum scrolls is [radiolucent](https://en.wikipedia.org/wiki/Radiodensity), making it difficult to see in the scans. Recently, Dr. Seales's team has trained a machine learning model which can detect the ink from subtle patterns in the 3D X-rays. This works in the fragments, but these models are not yet perfect and will probably need to be improved to work at the scale of an entire scroll.
- Putting it all together. Applying the ink detection models to the segmented scroll has not yet been successfully demonstrated.

Based on the [landmark results](https://raw.githubusercontent.com/educelab/EduceLab-Scrolls/main/paper/EduceLab-Scrolls.pdf) that Dr. Seales and his team have recently produced, we believe that it is possible to read the Herculaneum scrolls using the [scans](/data) that we already have and the tools and tecniques that they have developed. And that is the Vesuvius Challenge!

The Grand Prize deadline is 11:59pm Pacific, December 31st, 2023.

## Progress prizes ($100,000)

The purpose of progress prizes is to encourage contestants to solve important subproblems and release their work. We also hope that they attract more participants who are interested in starting with a narrower task, and then go on to try to win the Grand Prize.

Progress prizes are optional! You can choose to skip them and work directly on the Grand Prize.

### Ink Detection on Kaggle ($50,000 total)

As you will learn in the [tutorials](/tutorial1), one of the big challenges of reading the Herculaneum Papyri is detecting the ink in the 3D X-ray scans.

<figure>
  <video autoPlay playsInline loop muted className="w-[100%]" poster="/img/tutorials/ink-detection-anim2-dark.jpg">
    <source src="/img/tutorials/ink-detection-anim2-dark.webm" type="video/webm"/>
    <source src="/img/tutorials/ink-detection-anim2-dark.mp4" type="video/mp4"/>
  </video>
</figure>

For this important subproblem, we are offering a $50,000 [Ink Detection Progress Prize](https://www.kaggle.com/competitions/vesuvius-challenge-ink-detection/). This progress prize is hosted on Kaggle, and the final submission deadline is June 14th, 2023.

### Future Progress Prizes ($50,000 total)

We have some ideas of what future progress prizes might best accelerate overall progress on the Vesuvius Challenge, but we’re also keeping an open mind. If you have suggestions, please let us know!

