---
metaLinks:
  alternates:
    - /broken/spaces/mzd6xx2kCQ8dn7PxnBoD/pages/6Bd48tPzkNXHvUISVbgt
---

# ☄️ Reproducible Science

Many of us are in science because we want to drive progress. The goals of driving scientific progress are undoubtedly enhanced by greater sharing, and modern technology gives us the mechanisms to share our science better, and for the computational analyses we do, even precisely share every step. As the public mostly contributes to an academic scientist's salary with their taxes, you as a scientist might therefore feel a duty to use that money to give back to the community by sharing (and communicating) what you've done as freely (and clearly) as possible.

Unfortunately, sometimes in science we are pulled in one direction that is better for our careers, and another that is better for science. If the scientific system were better structured, these two goals would be perfectly aligned. However, practicing open science is one area where it helps both science and your own career. People value high-quality science, and sharing your science increases its impact:

1. Your work is marked as higher quality if it is reproducible. Quality matters in a scientific literature drowning in quantity. And a reputation for quality gets you noticed in your field.
2. You drive more attention to your science as people come across your work through the other resources you are freely making available to the world (e.g., data and code).
3. Others may build on your data/code, or use parts of it in their work, putting you a direct chain in aiding the progress of others (this is a great feeling).

If you choose not to share your work, you are simply putting on a show:

> An article about computational science in a scientific publication is not the scholarship itself, it is merely advertising of the scholarship. The actual scholarship is the complete software development environment and the complete set of instructions which generated the figures. — David Donaho ([reproducibleresearch.net](https://reproducibleresearch.net/))

Academia is special in that it is funded with the ideal goal of being impartial with respect to commercial or other interests. As such, trust is crucial---if we don't trust each other, then the public should not trust us. And if the public doesn't trust its scientists (the people who have spent decades training to be impartial, honest, and trustworthy), then, well, humanity is in trouble in a world in which rhetoric beats reason. The first step is trusting yourself and adopting reproducible science gives you greater trust in what you produce.

* The mindset of working reproducibly forces you to work to a much higher standard that pushes your science forward.
* It also allows you to go back to your analyses later down the track and be able to very quickly understand what you did when you want to do something new based on your past work (or direct someone else to).

There is a tendency to go all or nothing (in many causes, from veganism to dieting), but to make meaningful, lasting change we have to encourage small changes in the right direction. That is, any move in the direction towards open and reproducible science (the two go hand-in-hand) is a good way to build better habits and over time the practice will become second-nature. For example, it is optimal to move from a closed coding language like Matlab to python or R or Julia (where anyone can run your code without relying on a proprietary licence and all underlying code can be verified and improved over time by the community). But if you code in Matlab, making your code available and reproducible is a very valuable first step.

### Talk

:thought\_balloon: :thought\_balloon: :thought\_balloon: I gave a short overview talk on implementing reproducible science practices. The video is on [Youtube](https://youtu.be/fUGIKuXwFFc?t=2847) and the slides from this talk are [here](https://figshare.com/articles/OHBM_Australia_A_practical_guide_to_working_reproducibly/12367667). :thought\_balloon: :thought\_balloon: :thought\_balloon:

### Making scientific writing accessible

On submission to a journal, you should make it part of your workflow to submit to a preprint server, such as [arXiv](https://arxiv.org/), [bioRxiv](https://www.biorxiv.org/), or on the [Open Science Framework](https://osf.io/). These give you a DOI for your work (a unique key that allows others to cite it), and allow more rapid and wide sharing of science, as there is no barrier to others reading your work. Make sure you update the text if there are any edits involved in the review process. This is important to ensure that these open versions of closed papers accurately reflect the journal version (in content if not formatting).

For extra impact, you should cross-reference your work on [papers with code](https://portal.paperswithcode.com/).

#### Unpaywall

* Services like [unpaywall](https://unpaywall.org/) will automatically point people to these open versions of scientific articles.
* It's a good idea to install the unpaywall browser add-on.
* You need the [`biblatex-ext`](https://ctan.org/pkg/biblatex-ext) package and the extra functionality of the open access options: `biblatex-ext-oa.sty`.
* Actually this looks like a cool way to add these OA stamps automatically to you bibliography using the [unpaywall](https://unpaywall.org/) API.

#### Displaying your contributions in your CV

You can acknowledge your efforts to make your work accessible by marking your openly accessible outputs in your CV.

### Reproducible Coding

When coding, you’re often changing bits of code incrementally, or producing results that rely on a particular version of code. Version control, the most popular implementation of which is a system called 'git', is a way of keeping track of changes to a code repository over time. These repositories can also be uploaded to a server to allow collaboration on code, when working together with other researchers.

Details are on the [coding-and-computation.md](coding-and-computation.md "mention") page.

### Registered report

A registered report, where planned analysis steps are published and peer-reviewed prior to collecting the data and reporting the results, have the benefit of limiting researcher degrees of freedom and thus providing another level of transparency and reliability. Details are here [https://help.osf.io/article/330-welcome-to-registrations#Select-a-Registration-Template-1g4YO](https://help.osf.io/article/330-welcome-to-registrations#Select-a-Registration-Template-1g4YO)

### Sharing data

* [Zenodo](https://zenodo.org/signup/) is a good way to upload scientific datasets, providing a citable DOI to your data.
* [figshare](https://figshare.com) is a poorly designed alternative, but also provides a citable DOI to your data.
* Another option is [Dryad](https://datadryad.org/stash).
* To pick the right data repository for your paper, you can use the registry of research data repositories: [re3data](https://www.re3data.org/) or [FAIRsharing](https://fairsharing.org/).

### Getting involved

* Join the [Australia/New Zealand Open Research Network](https://www.anzopenresearch.org/), including the [Sydney chapter](https://sydneyopenresearch.org/).
* Join a [Reproducibilitea](https://reproducibilitea.org/) journal club.
* Follow some open science twitter accounts, e.g., this [open access Aus/NZ advocacy](https://twitter.com/openaccess_anz).
