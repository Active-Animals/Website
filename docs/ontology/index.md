# Active Animals Ontology (AAO)

Welcome! We're all about classifying animal behaviour and cataloguing observations.

## Introduction

The study of the mechanisms, development, evolution and function of behaviour is called [Ethology](https://doi.org/10.3389/fetho.2023.1270913). Behaviour classification is generally [a typological ordering system](https://doi.org/10.1046/j.1439-0469.2002.00211.x)[^1]. In this project, we are attempting to tease out some order from the, "almost chaotic diversity,"  of behaviour, by classifying its mechanisms (the more observable component of ethology, such as *swimming*) and their functional-context (the tip of the function iceberg wherein context may allow reasonable inferences, such as *escaping*).

Having undergone a closed, primordial development phase, the AAO project is now open for Alpha testing and redesign. Those interested in animal behaviour, and who are willing to contribute directly, are invited to collaborate. [Sister projects](#what-about-observations-and-examples) are also being developed to test the use of labelling developed here, for annotating searchable repositories of animal behaviour records, most notably at [iNaturalist](https://www.inaturalist.org). Collaborators are also being sought, who are able to test and extend these sister projects to their own records in various repositories, such as [xeno-canto](https://xeno-canto.org).

***If you would like to collaborate, check out the section: [Can I contribute?](#can-i-contribute)***

### Who is this for?

This ontology is a tool designed and maintained by and for amateur animal behaviour watchers. It provides us with a system for classifying what could potentially be seen, heard, felt, or otherwise tangibly discerned by us. It can also help us to share knowledge with each other. For some of us, it could extend the scope of natural observation beyond taxonomy. For others, it may even replace taxonomy as our main observational paradigm, with taxonomy having the supplementary role. In other words, 'collecting' behaviours.

A secondary use case is that of professional researchers into animal behaviour. Even if this ontology is not always consistent with the most current academic thinking, it can be used to build bridges between different interpretations or labels, as well as between 'citizens' and 'scientists'. If behaviour watchers use the labels to annotate publicly accessible artefacts as Instances of behaviour, it may assist professionals in searching for examples of unusual behaviour, or extensions of known behaviour to new animal taxa.

### Why is it needed?

What amateur behaviour watchers (and students beginning a life of ethology) crave, is an open access place to find labels and definitions for behaviours and categories of behaviour, with which to help them understand and record any behaviour they might encounter. For a price, paper glossaries might be bought such as the [Animal Behavior Desk Reference](https://doi.org/10.1201/b10864). But this and its ilk are an exhausting resource to bring to a five second video clip for a label, and have limited internal cross-references, let alone in a hierarchical set of categories.

Elephants currently probably have the most comprehensively categorised set of publicly accessible behaviour labels (see [Elephant Voices](https://www.elephantvoices.org/studies-a-projects/the-elephant-ethogram.html)). A handful of other taxon-specific glossaries and ethograms exist in scattered, patchy, often basic, and somewhat incompatible forms.

In 2011, a comprehensive, new ontology was launched. Called the [Neuro-Behavioural Ontology](https://www.ebi.ac.uk/ols4/ontologies/nbo) (NBO) and with a huge amount of goodwill, it scattered a vast range of behavioural shotgun pellets out into the behaviour-scape. Sadly, it rapidly ran aground on the shifting sands of its multiple use cases, and just couldn't be reconciled to the needs of all key stakeholders. It was for most purposes abandoned, never having come close to achieving its vision. Unfortunately, the way ontologies often crosslink to each other meant that a number of them had quickly become dependant on its continuing existence. And so it languished, effectively in limbo, with only minor attempts at what one correspondent called 'hacking'. A sage in the ontology world wrote of the NBO in January 2023:
> This ontology is functionally inactive, and I think it should be declared as such... to be fully transparent.

<p style="text-align: right">
  <a href="https://github.com/obo-behavior/behavior-ontology/issues/126#issuecomment-1397651952">Chris Mungall</a>
</p>

The AAO takes in a large scope, but with a more focused use case, not dependant on funding, and able to move forward without so many restrictions. It will undoubtedly have its gaps and failings. But unless it is replaced by something more water tight, it should provide at least a raft for those of us otherwise left to flounder.

By taking a public domain approach, we hope it will also provide leads to promising new avenues of ethological research. We hope this can then lead to highly collaborative forms of Citizan Science.

And as an incidental, we want to enable the principles of [FAIR data](https://en.wikipedia.org/wiki/FAIR_data) (findability, accessibility, interoperability, reusability).

### What's an ontology?

> An ontology contains a formal classification of terminology in a domain that provides textual and machine readable definitions, and defines the relationships between terms. An ontology is a terminology, but a terminology is not (necessarily) an ontology.

<p style="text-align: right">
  <a href="https://oboacademy.github.io/obook/lesson/ontology-term-use">Nicole Vasilevsky</a>
</p>

> A reference ontology is meant to serve a general purpose, providing terms for some domain of science. We can compare it to a textbook. An application ontology is meant to serve a specific purpose, limited to a particular project or institution, but often crossing several domains. An application ontology is likely to include terms from several reference ontologies. Reference ontologies focus almost exclusively on universals, while application ontologies are more likely to include terms for particulars.

<p style="text-align: right">
  <a href="https://github.com/jamesaoverton/obo-tutorial/blob/master/docs/obo.md">James A Overton</a>
</p>

#### What is the AAO?

This is an editable reference ontology for animal behaviours. It defines, labels, and interconnects potentially discernible actions and functional contexts. Using scientific references, it attempts to provide an internally consistent framework for classifying assertions which have been made about these behaviours.

In addition, it offers a range of non-behavioural classes (e.g. qualities), mainly imported from other ontologies, which can help situate certain behaviours.

#### What isn't the AAO?

This is not a reference for potentially maladaptive behaviours, and excludes so-called abnormal, aberrant, deficient, pathological, diseased, or impaired behaviour. We acknowledge that some acute stress-related behaviours are adaptive and so include them, but that chronic stress leads to maladaptive or compensatory behaviours, which we therefore do not include.

However, damage, variability, phenotype, and physiological state are referenced in the non-behaviour part of this ontology, alongside personality. These are all possible modulators of what could otherwise be adaptive behaviours.

NB: We are not describing specific individuals, except as Instances for illustration and typing.

### How does it work?

You use the ontology's labels to annotate a behaviour observation (sometimes called artefacts, e.g. one of your photos, sound recordings, or video clips). To find the right label, you need to look in the behavior branch hierarchy. You might be able to work your own way through a particular sub-branch to what you are looking for. Or you might want to try searching for a word you think is in the ontology somewhere. Bear in mind that some behaviours are listed with more than one parent class, or as part of another, so you might come at what you are looking for from different routes.

It might also be, that you want to add one or more non-behaviour (descriptive) classes to your annotation, relating to issues such as habitat or morphology. A range of these are appended to our ontology. The taxonomic characteristics (e.g. species) will be managed by your observation's host platform, if you are using a depository like iNaturalist to save your observations.

Only in exceptional cases do we label composite behaviours (usually if they have a unique term, or if they are synergistic and not merely additive). In other words, if you wish to label a co-occurent set of behaviours, label each one of them. The same goes for non-behaviours.

Remember that much is missing from the ontology and you may need to offer edits to existing entries, or new terms.

If you want to improve the ontology, make sure you understand the section, [Can I contribute?](#can-i-contribute) Then tuck into the page about [Editing](ontology/editing).

NB: You may offer edits to this Introduction or the Editing page too, although anything but typos in the Editing page may need some debate before being adopted by us all.

### Where is it?

The Active Animal's ontology structure and edit history is saved as a project in Stanford University's [WebProtégé](https://webprotege.stanford.edu) server. In this Alpha development phase, it is only visible to shared users who are accredited as collaborators. 

WebProtégé allows collaborators to mutually edit the ontology (even simultaneously if needed). A download of the current WebProtégé AAO project file (owl/rdf/xml), including all edits but no history, can also be viewed in more detail using the standalone desktop [Protégé](https://protege.stanford.edu) or other ontology software, but offline edits do not presently have a merging process.

In the Beta phase, we hope to provide an easier tool for users to locate appropriate labels for applying to their own observation records. By the end of the Alpha phase, we will regularly upload versions to [Bioportal](https://bioportal.bioontology.org) and this will provide an interim search solution to users without access to the WebProtégé project.

Unless the NBO is resurrected or a better replacement is created, we hope that our ontology will one day be accepted as a reference ontology in the [OBO Foundry](https://obofoundry.org) ontology community.

### What about observations and examples?

This project does not provide any storage for artefacts. Behavioural records are located in repositories in the form of example observations (ontologically referred to as Instances). iNaturalist provides the world's largest open data source of animal observations. Alongside this are a number of other open access online repositories for behavioural artefacts, such as xeno-canto. Most of these allow users to annotate or tag their uploads, and providing good labels for these annotations is our goal.

The [Active Animals (AA)](https://www.inaturalist.org/projects/active-animals-aa) project at iNaturalist is a way for animal behavioural records to be aggregated systematically there. Our ontology here provides the systematic source labels for the project's basic Observation Fields there. The AA project is also in its Alpha stage and interested collaborators are encouraged to message the project's own administration there.

Restricted access resources are unlikely to be referenced by the ontology, except in justifiable cases involving affordable entry or membership fees (e.g. behavioural artefacts like tools, nests, or fossils in museums, or videos which may be sourced in libraries, such as natural history documentaries on DVD). Some public animal behaviour resources also store accessible behavioural artefacts, such as Elephant Voices.

### Can I contribute?

We very much hope so!

This ontology aims to be participatory, transparent and accountable. In practice, this means first of all that a wide range of people can freely use, contribute ideas, edit, and even manage the ontology. Secondly, we use openly accessible software including the free WebProtégé platform. Thirdly, visible comments and an accessible change history allow users to review changes to the ontology.

Collaborators are expected to make active contributions, either in the ontology's engineering/software support, or in its database/editing curation, or stress-testing against their own observations. Consultants who only offer advice could play a key role, and will be directly recruited by a manager. Impromptu consultants will be thanked but invited to directly implement their own advice.

If advice about an issue is solicited by an active collaborator, advisory comments (without further commitment) are welcome. This may even be preferred to diving straight into an edit, particularly for big changes. Big changes may be reverted by a manager if inadequate prior community discussion has occured.

During the Alpha development phase, there will be a single manager (Ditch Townsend). Collaborators may be invited by a manager, or recommended to a manager by an editor. Known collaborators may be invited by a manager to be editors. Unknown collaborators may be invited to be commenters until they become sufficiently known to be invited to be an editor. The collaboration team will be limited in size.

During the Beta development phase, a significant number of positions will be available for new editors. Also for more commenters, provided they test the ontology against their own observations. During this phase, a mutually acceptable participatory organisational structure will be set up and tested, but will remain advisory to the manager, who will arrange for a deputy to also have management privileges.

Only in the open, final phase will the ontology be fully open. This stage will also mark an accountable and participatory organisation and management structure, including a mechanism for changing leadership.

Feel free to look over our [Editing](ontology/editing) guidelines.


***If you would like to collaborate, feel free to contact [Ditch Townsend](https://orcid.org/0000-0002-4277-2151)***

### How did the project start?

By May 2016, Ditch Townsend had taken thousands of fish photos and dozens of hours of video footage of them in his spare time, whilst diving and snorkelling around the world over the preceding 29 years. Having published several peer-reviewed articles, including a checklist of fish species found on the reefs off northwest Borneo, he decided it was time to catalogue (i.e. 'collect') some of the fish behaviours encountered along the way.

The "ah-ha!" moment came in December 2021, when stumbling across a reference to The Elephant Ethogram, a comprehensive catalogue of African savannah elephant behaviours. Made available in April 2021 and reported in a journal in November 2021, it was not only comprehensive and catalogued, but appended artefacts (videos and recordings) of each one. And so a search began for a fish analogue.

This led a few days later to discovering the [Zebrafish behavior catalog (ZBC)](https://doi.org/10.1089/zeb.2012.0861)[^1]: a large fish behaviour glossary originally published in 2013.  References there to the NBO drew Ditch to attempt to use the NBO to label the behaviours in short underwater video clips in mid-2022. This increasingly revealed the sorry state of what had looked a promising resource.

No sign of the promised ZBC 2.0, let alone an ethogram, was forthcoming ten years on from the original ZBC 1.0. So a method for synthesising the NBO with a ZBC 2.0 was proposed and pre-printed in December 2022, but abandoned as it was clear that the Zebrafish research community had given up on the NBO.

From this point, a year-long attempt was made to ressurect the NBO, trying to tackle its multiple methodological and content shortcomings. Sadly, no significant progress was made to achieve consensus in the scientific community for its revamp, although a handful of edits were made, and new structural models described, to illustrate possible ways forward. Efforts ceased in February 2024 (see [Issue 127](https://github.com/obo-behavior/behavior-ontology/issues/127#issuecomment-1925736023)). (By 25th November 2025, nothing more had been done either to edit or end it.)

So yet another new chapter was opened in early 2024. Using open source data mapping and ontology software ([Gephi](https://gephi.org) and Protégé), a fresh start was made to create a comprehensive, open, participatory, citizen science-led ontology of animal behaviour. Just under a year later, working alone in his spare time, Ditch was ready to open up a collaborative improvement and implementation process, to build on a starting line-up of 361 behaviours and 374 non-behaviours.

Drawing some inspiration from Bill Eshmeyer [Eschmeyer's Catalog of Fishes](https://www.calacademy.org/scientists/projects/catalog-of-fishes), it is hoped that unless others can pick up and run with the ball in a timely and useful way, this ontology can gradually become a core resource for all kinds of scientist, 'citizen' or otherwise. Using only openly accessible sources, we hope one day to reference all animal behaviours, their label and synonym origins, definitions and earliest uses, and their hierarchical relations.

[^1]: If you can't access this article, try searching for its title in Google Scholar to see if there are alternative sources.
