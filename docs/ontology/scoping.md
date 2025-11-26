# Active Animals Ontology (AAO)

Welcome! We're all about classifying animal behaviour and cataloguing observations.

## Scoping

On our [Introduction](ontology/index) page, you can find out more about our use case, model, and how to participate. Here we will outline our situation assessment.

### Why is it needed?

What amateur behaviour watchers (and students beginning a life of ethology) crave, is an open access place to find labels and definitions for behaviours and categories of behaviour, with which to help them understand and record any behaviour they might encounter. For a price, paper glossaries might be bought such as the [Animal Behavior Desk Reference](https://doi.org/10.1201/b10864). But this and its ilk are an exhausting resource to bring to a five second video clip for a label, and have limited internal cross-references, let alone in a hierarchical set of categories.

Elephants currently probably have the most comprehensively categorised set of publicly accessible behaviour labels (see [Elephant Voices](https://www.elephantvoices.org/studies-a-projects/the-elephant-ethogram.html)). A handful of other taxon-specific glossaries and ethograms exist in scattered, patchy, often basic, and somewhat incompatible forms.

In 2011, a comprehensive, new ontology was launched. Called the [Neuro-Behavioural Ontology](https://www.ebi.ac.uk/ols4/ontologies/nbo) (NBO) and with a huge amount of goodwill, it scattered a vast range of behavioural shotgun pellets out into the behaviour-scape. Sadly, it rapidly ran aground on the shifting sands of its multiple use cases, and just couldn't be reconciled to the needs of all key stakeholders. It was for most purposes abandoned, never having come close to achieving its vision. Unfortunately, the way ontologies often crosslink to each other meant that a number of them had quickly become dependant on its continuing existence. And so it languished, effectively in limbo, with only minor attempts at what one correspondent called 'hacking'. A sage in the ontology world wrote of the NBO in January 2023:
> This ontology is functionally inactive, and I think it should be declared as such... to be fully transparent.

<p style="text-align: right">
  <a href="https://github.com/obo-behavior/behavior-ontology/issues/126#issuecomment-1397651952">Chris Mungall</a>
</p>

The AAO takes in a large scope, but with a more focused use case, not dependant on funding, and able to move forward without so many restrictions. It will undoubtedly have its gaps and failings. But unless it is replaced by something more water tight, it should provide at least a raft for those of us otherwise left to flounder.

By taking a public domain approach, we hope it will also provide leads to promising new avenues of ethological research. We hope this can then lead to highly collaborative forms of citizan science.

And as an incidental, we want to enable the principles of [FAIR data](https://en.wikipedia.org/wiki/FAIR_data) (findability, accessibility, interoperability, reusability).

### How did the project start?

By May 2016, Ditch Townsend had taken thousands of fish photos and dozens of hours of video footage of them in his spare time, whilst diving and snorkelling around the world over the preceding 29 years. Having published several peer-reviewed articles, including a checklist of fish species found on the reefs off northwest Borneo, he decided it was time to catalogue (i.e. 'collect') some of the fish behaviours encountered along the way.

The "ah-ha!" moment came in December 2021, when stumbling across a reference to The Elephant Ethogram, a comprehensive catalogue of African savannah elephant behaviours. Made available in April 2021 and reported in a journal in November 2021, it was not only comprehensive and catalogued, but appended artefacts (videos and recordings) of each one. And so a search began for a fish analogue.

This led a few days later to discovering the [Zebrafish behavior catalog (ZBC)](https://doi.org/10.1089/zeb.2012.0861)[^1]: a large fish behaviour glossary originally published in 2013.  References there to the NBO drew Ditch to attempt to use the NBO to label the behaviours in short underwater video clips in mid-2022. This increasingly revealed the sorry state of what had looked a promising resource.

No sign of the promised ZBC 2.0, let alone an ethogram, was forthcoming ten years on from the original ZBC 1.0. So a method for synthesising the NBO with a ZBC 2.0 was proposed and pre-printed in December 2022, but abandoned as it was clear that the Zebrafish research community had given up on the NBO.

From this point, a year-long attempt was made to ressurect the NBO, trying to tackle its multiple methodological and content shortcomings. Sadly, no significant progress was made to achieve consensus in the scientific community for its revamp, although a handful of edits were made, and new structural models described, to illustrate possible ways forward. Efforts ceased in February 2024 (see [Issue 127](https://github.com/obo-behavior/behavior-ontology/issues/127#issuecomment-1925736023)). (By 25th November 2025, nothing more had been done either to edit or end it.)

So yet another new chapter was opened in early 2024. Using open source data mapping and ontology software ([Gephi](https://gephi.org) and [Protégé](https://protege.stanford.edu)), a fresh start was made to create a comprehensive, open, participatory, citizen science-led ontology of animal behaviour. Just under a year later, working alone in his spare time, Ditch was ready to open up a collaborative improvement and implementation process, to build on a starting line-up of 361 behaviours and 374 non-behaviours.

Drawing some inspiration from Bill Eshmeyer (see [Eschmeyer's Catalog of Fishes](https://www.calacademy.org/scientists/projects/catalog-of-fishes)), it is hoped that unless others can pick up and run with the ball in a timely and useful way, this ontology can gradually become a core resource for all kinds of scientist, 'citizen' or otherwise. Using only openly accessible sources, we hope one day to reference all animal behaviours, their label and synonym origins, definitions and earliest uses, and their hierarchical relations.

[^1]: If you can't access this article, try searching for its title in Google Scholar to see if there are alternative sources.
