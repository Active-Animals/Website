# Active Animals Ontology (AAO)

Welcome to the Active Animals Ontology.

## Introduction

[Ethology](https://doi.org/10.3389/fetho.2023.1270913) is the study of proximate causes of behaviour (mechanisms and development), and their ultimate roots (evolution and function). Behaviour classification is generally [a typological ordering system](https://doi.org/10.1046/j.1439-0469.2002.00211.x)[^1]. In this project, we are attempting to tease out some order from the, "almost chaotic diversity,"  of behaviour, by grouping its mechanisms: the more observable component of ethology.

Having undergone a closed, primordial development phase, the project is now open for Alpha testing and redesign. Those interested in animal behaviour, who are willing to contribute directly, are invited to collaborate.

Sister projects are also being developed to test the use of labelling developed here, for annotating searchable repositories of animal behaviour records, most notably at [iNaturalist](https://www.inaturalist.org). Collaborators are also being sought, who are able to test and extend these sister projects to their own records in various repositories, such as [xeno-canto](https://xeno-canto.org).

### Who is this for?

This ontology is designed by and for amateur animal behaviour watchers. It provides us with a system for classifying what could potentially be seen, heard, felt, or otherwise tangibly discerned by us. It can also help us to share knowledge with each other. For some of us, it could extend the scope of natural observation beyond taxonomy. For others, it may replace taxonomy as our root observational paradigm, with taxonomy having the supplementary role. In other words, 'collecting' behaviours.

A secondary use case is that of professional researchers into animal behaviour. Even if this ontology is not always consistent with the most current academic thinking, it can be used to build bridges between different interpretations or labels, as well as between 'citizens' and 'scientists'. If behaviour watchers use the labels to annotate publicly accessible instances of behaviour, it may assist professionals in searching for examples of unusual behaviour, or extensions of known behaviour to new animal taxa.

### Why is it needed?

What amateur behaviour watchers (and students beginning a life of ethology) crave, is an open access place to find labels and definitions for behaviours and categories of behaviour, with which to help them understand and record any behaviour they might encounter. For a price, paper glossaries might be bought such as the [Animal Behavior Desk Reference](https://doi.org/10.1201/b10864). But this and its ilk are an exhausting resource to bring to a five second video clip for a label, and have limited internal cross-references, let alone in a hierarchical set of categories.

Elephants currently probably have the most comprehensively categorised set of publicly accessible behaviour labels (see [Elephant Voices](https://www.elephantvoices.org/studies-a-projects/the-elephant-ethogram.html)). A handful of other taxon-specific glossaries and ethograms exist in scattered, patchy, often basic, and somewhat incompatible forms.

In 2011, a comprehensive, new ontology was launched. Called the [Neuro-Behavioural Ontology](https://www.ebi.ac.uk/ols4/ontologies/nbo) (NBO) and with a huge amount of goodwill, it scattered a vast range of behavioural shotgun pellets out into the behaviour-scape. Sadly, it rapidly ran aground on the shifting sands of its multiple use cases, and just couldn't be reconciled to the needs of all key stakeholders. It was for most purposes abandoned, never having come close to achieving its vision. Unfortunately, the way ontologies often crosslink to each other meant that a number of them had quickly become dependant on its continuing existence. And so it languished, effectively in limbo, with only minor attempts at what one correspondent called 'hacking'. A sage in the ontology world wrote of the NBO in January 2023:
> This ontology is functionally inactive, and I think it should be declared as such... to be fully transparent.

<p style="text-align: right">
  <a href="https://github.com/obo-behavior/behavior-ontology/issues/126#issuecomment-1397651952">Chris Mungall</a>
</p>

From this point, a year-long attempt was made to ressurect the NBO, trying to tackle its multiple methodological and content shortcomings. Sadly, no significant progress was made to achieve consensus in the scientific community for its revamp, although a handful of edits were made, and new structural models described, to illustrate possible ways forward. Efforts ceased in February 2024 (see [Issue 127](https://github.com/obo-behavior/behavior-ontology/issues/127#issuecomment-1925736023)). By 25th November 2025, nothing more had been done either to edit or end it.

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

NB: We are not describing specific individuals, except as instances for illustration and typing.

### How does it work?

You use the ontology's labels to annotate an instance of behaviour (e.g. one of your photos, sound recordings, or video clips). To find the right label, you need to look in the behavior branch hierarchy. You might be able to work your own way through a particular sub-branch to what you are looking for. Or you might want to try searching for a word you think is in the ontology somewhere. Bear in mind that some behaviours are listed with more than one parent class, or as part of another, so you might come at what you are looking for from different routes.

It might also be, that you want to add one or more non-behaviour classes to your annotation. The taxonomic characteristics (e.g. species) will be managed by your observation's host platform, if you are using a depository like iNaturalist to save your observations.

Only in exceptional cases do we label composite behaviours (usually if they have a unique term, or if they are synergistic and not merely additive). In other words, if you wish to label a co-occurent set of behaviours, label each one of them. The same goes for non-behaviours.

Remember that much is missing from the ontology and you may need to offer edits to existing entries, or new terms.

If you want to improve the ontology, make sure you understand the section, [Can I contribute?](#can-i-contribute) Then tuck into the page about [Editing](ontology/editing).

NB: You may offer edits to this Introduction or the Editing page too, although anything but typos in the Editing page may need some debate before being adopted by us all.

### Can I contribute?

[^1]: If you can't access this article, try searching for its title in Google Scholar to see if there are alternative sources.
