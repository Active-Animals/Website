# Active Animals Ontology (AAO)

Welcome! We're all about classifying animal behaviour and cataloguing observations.

## EDITING

On our [INTRODUCTION](index) page, you can find out more about our use case, model, and how to participate. **If you would like to collaborate, first check out its section: [Can I contribute?](index#can-i-contribute)**

Here we will outline our guidelines and rules for contributing to the ontology via the collaborative, online, ontology editor: WebProtégé.

*See the footnote if you want to suggest edits to this website.*[^1]

[^1]: Feel free to click the 'View on GitHub' button, then click 'Issues' in the top bar, and create a new one by clicking 'New issue'. Explain your suggestion and we will look into it. Of course, if you are familiar with GitHub, you can create a branch, make and commit your edits, and create a pull request. If it is more than a simple edit though, we suggest you tie it to an issue so some discussion can be had in advance of the pull request.

### Using WebProtégé

#### Login
1. You need your own account to use WebProtégé. You can Sign Up or Sign In [here](https://webprotege.stanford.edu/#login).
2. Contact the AAO manager with your new username, to receive an invite to the project in WebProtégé. (In the Alpha phase, there may be restrictions even on the number of viewers or commenters, let alone editors. You may be asked to explain how you can contribute before being given an invitation. You may want to get this agreement before creating a WebProtégé account.)
3. On your Projects list page, ensure that the 'Shared with Me' box is ticked. If you have been invited to the project, it should appear there as 'Active Animals ALPHA', although you may need to refresh the page, or even log back in if the page has expired.
4. Open the project by clicking the project's name, or find more opening options in the hamburger button.
  - You can download your own legacy copies as often as you like: the project has a CC0 license and the file can be read by any owl/rdf/xml viewer.
  - Unless you have the manager's permission, please don't download to work offline with another editor such as Protégé and then upload, as you will overwrite the whole project, losing other peoples' changes since your last download.

#### Guides
There is a basic [user guide](https://protegewiki.stanford.edu/wiki/WebProtegeUsersGuide) available at WebProtégé. Only one of its screencast links works (the first link below).

Only two useful videos seem to be available to help. One is an early version [demo](http://www.youtube.com/watch?v=QvURiHVXnQQ), but it gives a feel for things, although the layout is outdated.

The [other](https://www.youtube.com/watch?v=fkBjRfQGoXQ) is much more modern and gives some ideas about layout and use, in the form of 10 Tips. Tip 9 shows the mechanics of laying out WebProtégé to suit you.

You do not actually need to know how to do much that these guides talk about, as you will be editing a previously set up ontology. Not only will you probably be set up initially to just Comment (see Tip 9 above), but you will be offered support, probably in the form of a one-to-one online screen-sharing tutorial, if you are invited to collaborate during the Alpha phase.

If you really want to delve into ontology engineering (including desktop Protégé), you can steer yourself through anything that takes your fancy at the [OBO Semantic Engineering Training](https://oboacademy.github.io/obook) site.

### Always...

#### Small bites
The history tab in WebProtégé will be easiest for future users to follow, if every edit is small, containing only a bitesize of material. Working in WebProtégé this will happen automatically. But if the manager approves of editing using an external editor such as Protégé, you will need to save and upload after every significant edit (i.e. not each word, but perhaps after each annotation has been added or edited).

Only if a thematic edit is undertaken offline, multiple edits may be handled in a single save. In due course, we hope to have a GitHub pipeline set up to allow merging of branches (e.g. offline edits in Protégé) with the main file. Commits then will still need to be made very frequently. Over the horizon, we also hope that WebProtégé will be upgraded to allow merges with offline files without using a GitHub pipeline, or directly tied into it instead of being fully stand-alone as at present.

#### Frequent Commits
Every edit merged into WebProtégé is called a Commit. It may not be obvious what an edit is doing. Therefore WebProtégé automatically adds a title to each change you make which it merges in, focused on the activity undertaken.

If approved by the manager to do, every Protégé upload will not only overwrite the WebProtégé base file (although it will leave Comments alone), but it will have an unhelpful generic Commit title. This needs to be changed to give a useful idea of what the edit has done, before finishing the upload. Make a quick reference to any prior discussion on the site about the topic. If there is no prior discussion about the change within the history, it may be better to have the discussion first, but if it can't be helped, then add some reasoning for the change to the Commit.

In due course, we hope to use a GitHub pipeline, or an upgraded version of WebProtégé, for Commits. This will prevent merges into the main file from happening without anyone consenting.

NB: The primordial version of the ontology has been developed as a unitary draft, without edited Commits, but from the time joint editing started, the original author became subject to this expectation.

#### Inclusive Comments
Your early forays into collaborating may be in the form of Comments only. When you have editing privileges, still consider whether proposing a planned change in the form of a Comment (a WebProtégé View which does not directly enter the ontology structure) might be the best way to start. Try to gain consent, if not consensus. Remember that your edits may be reverted if they appear controversial and have had no discussion. For new terms, make your comment against a parent class if you choose to wait before creating the new class. (Waiting may become the norm if new classes too often have to be reverted.)

Meanwhile, bear in mind that you can view or hide resolved comment threads using the Filter symbol in the WebProtégé Comment View or Tab.

### Annotations

Annotations allow us to understand more about a given class. It may give information about by whom and when it was created, its synonyms, or comments about it, etc.

#### DO Use
##### For Behaviours
  - Automatically introduced annotations for new terms are:
    - created_by
    - creation_date
  - Required annotations for all terms are:
    - rdfs:label
    - dc:source
    - hasDefinition (this can be waived short-term)
  - As required annotations are:
    - hasBroadSynonym
    - hasExactSynonym
    - hasNarrowSynonym
    - hasRelatedSynonym
    - rdfs:comment (for additional, useful information)
    - rdfs:isDefinedBy (where a definition is substantially quoted even if not originally intended as such)
    - rdfs:seeAlso (where another source gives an illuminating perspective but is not necessarily synonymous)
    - skos:example (for valuable illustrations)
    - skos:scopeNote (for an idea about the content or limits of a concept, usually where the definition is not yet finally composed)

##### For Non-Behaviours
  -  Required annotations for new ontology sources (but requiring management agreement) are:
     - dcterms:license
  - Imported terms often come with an array of annotation 'baggage'. Much of this can be stripped away to reduce confusion for future local users. 

#### DON'T Use
  - A number of Annotation Properties belong to external ontologies and have been retained for their utility in understanding them, but please don't use them for our behaviour terms.
  - Owl properties are built into Protege but should not be introduced to our ontology without management agreement.
    - owl:deprecated should only be used after extensive discussion.

### Definitions

Sooner or later, every class should have a useful definition. The primordial structure contains many without definitions and these are a priority for completing. New terms from the Alpha stage onwards should generally be proposed alongside a well researched definition.

For more detailed guidelines, many of which have informed ours below, see the paper on[Guidelines for writing definitions in ontologies](https://revista.ibict.br/ciinf/article/view/4015)

#### Meaning
Before starting, consider whether your new definition will change the meaning of the class's ground concept (note that the two are not always identical). This can be broadly assessed by considering the existing label, examples, comments, scope notes, properties, and any sources referred to already.

Be more wary if there is already a textual definition and you wish to change it: consider whether your new definition will be inclusive of it (i.e. is your new definition more general, NOT more specific).

Lastly, consider whether your definition will directly aid (or improve) the identification of the behaviour in question. If all these issues are answered positively, go ahead.

NB: A very strict form of ontological reasoning will argue that there is no intrinsic difference between a concept and an accurate axiomatic definition. Therefore changing the concept will necessarily require changing a logical definition, which must necessarily require creation of a new term. However, humanly useable ontologies like ours do not fully axiomatise their 'ground concepts' in the form of logical definitions, and unless written strictly for machine learning, what we are doing is generally accepted.

#### Constructing
Ignoring the parts in (rounded brackets), use the construction:
(X is a) Y [that / when / in which / wherein] Z. 

Use the immediate binomial or trinomial for Y if it will aid understanding, e.g. (gathered-suspended is) an unsupported placement that...

  - X is linguistically referred to as a definiendum. 
  - Y is linguistically referred to as the genus.
  - Z is linguistically referred to as the differentia(e); there may be more than one).

#### Quoting
Where a source is essentially being quoted for the definition, annotate with rdfs:isDefinedBy and hasDefinition. Sub-annotate hasDefinition with dc:source and skos:scopeNote (quoting the whole sentence or sentences from which the definition is drawn). There is no need to add dc:contributor as a sub-annotation to the definition, but by all means add it as a term annotation.

Use [square brackets] to add the label for Y (the genus) if it is not in the quoted section of the source, but no quote marks.

Limited edits may be needed, such as modifying word endings, or cutting and splicing very close elements contained within a single sentence (or possibly adjoining sentences), and preferably without reversing word order.

A quoted definition may be made more parsimonious by dropping a superfluous component, but not if it simply generalises the definition (i.e. not if the dropped component would effectively create a sub-division). Word changes should also be avoided, particularly if the definition would be made more generic (e.g. by changing 'fish' to 'animal').

Otherwise, even if the bulk of the definition comprises quotes, use hasDefinition, with dc:source and dc:contributor as sub-annotations (and avoid rdfs:isDefinedBy); see [Creating](#creating).

#### Creating
Annotate with hasDefinition, and sub-annotate that with dc:source and dc:contributor (even if you are the creator of the term). Every definition must be sourced, even if not quoted.

#### Multi-sourcing
Where more than one source is used to create a definition, give each as a sub-annotated dc:source. Also quote from each as a skos:scopeNote, but add the source in brackets to link it back, because sub-sub-annotating is not possible in WebProtégé.

#### Expanding
To expand the definition beyond its essential core, either use additional text following a full-stop (rather than a comma, colon, or semicolon), or offer a skos:scopeNote annotation.

#### Tautology
Do not use the term label or its root within its own definition, unless in a clarifiying sentence after the first full-stop. An exception may occur where the label is apparently partly composed from its actual or potential ontological parents, parts, participants, or attributes (e.g. terrestrial-lateral-undulating). Another is where the label is one of a set of invariant and exclusive subdivisions (e.g. spawning may only involve eggs or sperm). In any case, remain open to adopting alternative terminology.

NB: Some judgement may be needed about how far back roots should be sought (e.g. are feign and feint from separate French words or the same Latin word), but try to avoid a debate if possible.

#### Multi-parenting
All parents must be referred to in the definition. It may be most appropriate to select one as genus and use the others as differentia to form a composite definition. In this case, do not offer a dc:source, but use hasDefinition with dc:contributor embedded, and rdfs:comment embedded noting that the definition is a composite.

The ontology is currently moving towards the goal of single parenthood, with subsidiary parthood. Older terms are most likely to remain unamended for some time, but new terms will need to strongly justify multi-parenting.

#### Para-synonymy
Using a synonym in a simplistic definition is tempting and perhaps unavoidable at times. But it is too close to being tautology for the long term, and should be avoided in the first place if possible. (The definition is ideally some kind of expanded explanation.)

If needed, change the synonym type to hasRelatedSynonym as a workaround which will also highlight its deliberate use, but don't just delete the synonym in order to reintroduce it to the definition.

### Synonyms

Synonyms should be sourced and dated by year. They can have modified suffixes to match the class label in question.

Choose the annotation property which is most suitable, when labelling synonyms. Remember that any one may in future be challenged, so consider a justifying comment or quote:
  - **hasExactSynonym** may be asserted by a source, or linguistically
  - **hasBroadSynonym** is inclusive of, but not limited to, the main label (consider if it should be a superclass instead)
  - **hasNarrowSynonym** excludes aspects of the main label, but is fully enclosed by it (consider if it should be a subclass instead)
  - **hasRelatedSynonym** should be used with great care, to ensure it is not in fact one of the other forms. It may be worth using if you have used much licence to infer a synonym from within a source in a way that you expect other collaborators could question (consider too whether you have actually stumbled on a new term needing creating); see also [para-synonymy](#para-synonymy)

If you wish to promote a synonym to the main label, justify this and try to engage in discussion before implementing any change; remember also to relegate the label to a synonym.

The same word may have different meanings in different sources. The following method should enable a string search to pull out each alternate meaning:
  1. Where it is used as a synonym with a different meaning to its use elsewhere, add the current term's ID to the synonym string as a suffix after a hyphen, and repeat for each different synonym meaning (e.g. if Label A applies to a primary term, synonym A-AAO000000x applies to one alternative meaning, synonym A-AAO000000y applies to another alternative meaning, etc).
  2. Do not add the ID suffix to the label bearing the primary meaning of the string, unless it is demoted later to a synonym (and remove the suffix from any synonym promoted to primary label use).
  3. It is possible that a synonym string is used in multiple ways (each with its own ID suffix) without being used as a primary label anywhere.
  4. It is possible that a synonym string is used in multiple terms but only one way (without the need for an ID suffix), without being used as a primary label anywhere.
  5. Where two synonymised occurrences of a label have the same meaning but different to a primary label usage, select one ID suffix to use for both. This could be one of the two occurrences, or in the case of a shared parent (most likely to happen with a Broad synonym) it could be the ID of the shared parent.

### Obsoletions

It is not our role to judge the validity of an assertion. Before considering incompatibility, be sure you are not better served with a [Synonym](#synonyms).

However, scientific ideas evolve and new ideas emerge which may be incompatible with former ones, and we need to be able to differentiate these assertions from one another. With sufficient consensus, an rdfs:Comment can be added to the effect that it is an INACTIVE TERM simply meaning that it should not be used for ongoing annotation.  Where a concept is directly criticised in a source as obsolete, defunct, or a similar appelation, consider using the annotation property 'skos:scopeNote' to quote or summarise the criticism, along with 'dc:source'.

If incompatibility is clear, then create a new term. Annotate both with rdfs:seeAlso. In OWL syntax, we can also annotate a term as OWL:deprecated, which means it will appear crossed-out, yet will not disappear from the ontology, and remains visible to the reasoner. It also means the ID will not be reused, so there will be no confusion over its edit history.

Don't simply hijack a label, since the term history could become incomprehensible. Instead consider alternatives which preserve the old and the new. For example, give a clarifying word after a hyphen in the label, although try to relate it to the clarifying author (e.g. 'migrating-Smith' and 'migrating-Jones) or concept, rather than simply '-old' and '-new'. Some new concepts will come with their own new labels. If you must reuse a label for the new concept, ensure the deprecated term has some label in addition to its old ID number.

This whole topic may be revisited in due course.

### Instances

An Instance is a unique example of a class being used. In our case, it will be a particular behavioural label as applied to a specific Observation (a photo, recording, video, or other artefact). This will have been archived in a permanent (if possible), specific, sign-posted (e.g. a URL), publicly accessible location outside our ontology (online if not a physical artefact, and not embedded in our ontology). While the item may be reused (e.g. for several different behaviours), the Instance is unique (being the only use of the particular behavioural label to the particular item).

#### Preparation
iNaturalist is designed to host hundreds of millions of observations. The [Active Animals (AA)](https://www.inaturalist.org/projects/active-animals-aa) project there can leverage its capabilities to catalogue large numbers of examples. Our ontology is not designed to duplicate that cataloguing function. The Instances we hope for in this ontology are of two kinds:

###### ILLUSTRATION
Links to scientifically robust external resources which illustrate a behaviour, to aid in understanding it, and to aid in identifying the behaviour in one of our field observations. These links should be provided judiciously, and only multiplied in a specific class where they extend understanding beyond previous Instances; they should not simply be added on a taxonomic basis, although taxonomy may be an underlying reason to multiply illustrations.

###### TYPE
Type examples should come from within the iNaturalist catalogue, or other hobbyist repositories (i.e. not scientific sources). They should be offered or agreed to by their originator. Once added, they should not be changed without a discussion.

#### Leaf (terminal) classes
Where a class has no subclasses (i.e. it is a leaf or terminal class), a new Instance can be considered. Where a class has subclasses, Instances should only exist to illustrate key elements missing from the subclasses. Otherwise, it is redundant and should be deleted unless justified in an rdfs:comment.

#### Individuals
Use the Individual tab in WebProtégé, or the Individuals by Class view in any tab in WebProtégé, to add details of the Instance to the relevant class.

### New Terms

#### Preparing
Your new class should represent a unique concept, not merely a unique label. Indeed, the label could be changed later, but the 'thing' that is the class should never change. (If it is superceded later, it may be [deprecated](#obsoletions), and a new class should be created, even if it has the same label, and a link can be made to the deprecated class to show it has been replaced.) 

Search the ontology thoroughly for classes which may duplicate your concept, even if using different wording, and if they need modifying without changing the meaning, an edit there may be the best way forward. As long as there is still no exclusive definition, it may be possible to modify the class's concept (e.g. inclusive definitions might be changed, or subdivisions added).

Except in justifiable cases (e.g. 'instinct' which has a long pedigree and is widely known), try not to create new classes just to suggest they are inactive. Our initiative is not trying to track every discredited idea that has ever been dreamt up about behaviour, but ideas which help explain where we are now, and how we got here.

#### Compounding
An almost infinite array of compound terms is possible. We need to limit this:

  1. A behavioural episode observed may be broken up into multiple sub-behaviours, any of which can be created individually if they don't already exist (i.e. in the case of five sub-behaviours, there will be a maximum of five new terms added, rather than five factorial = 120 new terms).
  2. A commonly used compound term may be used along with links to its multiple parents, but there should be an rdfs:comment giving justification for using it.
  3. A conjoint term may be created where it is not simply additive, but synergistic, i.e. there is more to the compound behaviour than a simple addition of its components.
  4. Unless a single word captures the compound concept, place dashes-between-words in its label, to avoid confusion with the [binomial behavioural description](#constructing) and the 'inverted commas' used by WebProtégé to capture labels given more than one word by other ontologies.
  5. Unless the words are used in tandem in the source, they should be very close together in its text and there should be no doubt about them modifying the meaning of each other.

#### Starting
If you want to create new terms, ask the manager to allocate you a batch of ID codes (these are then applied automatically).

Select a parent class (you can change it later), click the Create button, and write a label which is unique to the behaviour branch of the ontology. (WebProtégé will auto-insert the ID and IRI, and the created_by and creation-date annotations.) 

If the label must duplicate a non-behaviour branch label, here is a trick learned the hard way:
  1. first create it with a mis-spelling;
  2. when the class has been created and saved, correct the spelling, but not immediately;
  3. there may be some delay as WebProtégé catches up with itself internally;
     - too soon, and it may list both as labels alongside each other;
       - in this case, go back and delete the superfluous one;
     - otherwise autofill will simply insert the other class with the same name;
       - if this happens by mistake, do not compound the error by deleting the pre-existing class;
       - instead delete its mistaken parent in its own parent's list;
  4. and then refresh your view

#### Word form
Try to select a word form for the new term, such that it can form a meaningful binomial as both parent and child, when spoken in the word order subclass > superclass, with the option to complete the phrase with a high level term such as 'behaviour' (e.g. singing vocal behaviour, vocal acoustic behaviour, acoustic signaling).

#### Sourcing
The term itself should be sourced if possible (although a slightly different word form is okay). A sub-annotation should be added with a dc:source. If the term can only (but easily) be inferred from a source, add an rdfs:comment as a sub-annotation.

### Precedence

This section explains which sources or contributors should have priority in our ontology.

#### Principles
1. Any source must be legally, publicly accessible, even if the DOI or ISBN or catalogue number does not link directly to such a source. (Digital media should be available free and online via links from within a Google Scholar, or Internet Archive Scholar, or JSTOR free personal account search.)
2. The oldest such source to use the term should be referenced.
3. The oldest source need not incorporate every facet of the topic, so long as it does not lie outside, or contradict, a class's definition.

#### Label & Synonyms
Ideally, given our Principles, we want to list the earliest source which references any label or synonym:

1. It should if possible contain the stem and not just the root (e.g. symmetric, symmetrical, and asymmetric share a root - symmetry - but have two different stems - symmetric and asymmetric), although some variance may be acceptable.
2. Compound labels should apply the same rule to each word individually, but compound synonyms should apply the rule to the whole.
3. No concept may be changed by changing a label, although a completely different word or word form may be more appropriate to an existing one. (A new concept and possible deprecation of the old one may be needed instead.)

#### Definition
The key for a definition is not so much its precedence, as its accuracy, inclusivity, and utility.

#### Creation
Editors who create new terms using the WebProtégé portal will automatically have the date and the creator added, and also an ID number which will remain exclusive to that class despite future edits.

#### Contribution
All contributors are encouraged to flag their own inputs with annotation property dc:contributor, preferably using an [ORCID](https://orcid.org) ID or something similar, although your name is acceptable (but not just initials or username).

#### Examples
The number of examples should be very constricted, preferably to one overall, but up to one each of the following criteria if necessary. Please don't delete examples or add a fourth (or more) without a discussion in the relevant page's WebProtégé comment tab. It should balance:

1. Primordial publication
2. Evocative description
3. Generalisability

#### Instances
##### ILLUSTRATIONS
Most important are production values (clarity, aesthetics, story, etc) and utility (accessibility, comprehensiveness), with age-related features only being key if they have some historical weight (e.g. a classic photo).

##### TYPES
This should be the earliest AAO-user example that clearly shows the behaviour in question. This is both an incentive and a credit to those of us for whom this is our hobby.

#### Top classes
Several key principles apply to successful ontologies. They should be:

>open, orthogonal, instantiated in a well-specified syntax and designed to share a common space of identifiers
>
<p style="text-align: right">
  <a href="https://doi.org/10.1038/nbt1346">OBO Foundry (Smith et al)</a>
</p>

Accordingly, we have reused classes defined in other ontologies for our top level classes:

  - GO:0007610 behavior, comes from a primordial ontology called the Gene Ontology (GO), and is widely reused amongst other ontologies. Its core is borrowed directly from a 2009 paper, doi:10.1016/j.anbehav.2009.03.018

    NB: behavior in GO is defined as a process, and as such it is a branch of an almost fundamental ontological category: 'occurrent'. This group is defined as, "An entity that has temporal parts and that happens, unfolds or develops through time." For now we have avoided using the category in the ontology, being loathe to allow 'behavior' to disappear from first line view of users.

  - BFO:0000002 continuant, is contradistinct to 'occurrent'. It lies at the heart of several sub-branches, not least a key ontology called the Phenotype And Trait Ontology (PATO) with its branch PATO:0000001 quality. Continuants should all be imported in this ontology.

  - Several other imported process branches line up alongside behavior because they too are occurrents, but they are less critical to understanding our ontology terms: 'environmental system process', 'life cycle stage', and 'mental process'.

Many of our terms could have been reused from the [Neuro-Behavioural Ontology](https://www.ebi.ac.uk/ols4/ontologies/nbo) (NBO). However most terms there don't match our criteria for proper definition, or come without an appropriate external reference. Furthermore, the ontology has not been owned and maintained effectively for many years. Indeed, some efforts have been made to obsolete its terms in favour of near equivalents in other ontologies, or to transfer ownerships to other ontologies, not least from its phenotype branch. Hypothetically, the same could apply to many of the terms on its behavior branch in favour of our ontology. Hence, in due course, we hope to annotate many terms with rdfs:seeAlso or hasDbXref [NBO_???????], but do not plan to import any NBO term.

### Relationships

Every parent-child relationship is automatically accorded the inclusion 'is_a' (which is invisible to us). Be careful not to introduce circularity by making something a subclass of itself somewhere else in the map.

Also be cautious about the direction of other kinds of relationship (called object properties) you add to a term, as it can affect reasoning if it is wrong (e.g. 'part_of' instead of 'has_part' can introduce the enigma in which, "all cats are animals and all animals are cats"). Our aim is to keep the number and kinds of relationship simple and limited. Feel free to introduce your argument in a WebProtégé comment if you feel the need for a new one. Only a manager should introduce new kinds of relationship.

Delving under the surface of ontology engineering will reveal two basic types of data: occurrents (in the case of behaviour, these are all processes which may be on or off at any given time), and continuants (in our case, these are generally tangible objects like morphological qualities, which do not behave ephemerally). Some object properties should only be used when relating two terms of the same type. Some only when terms are of different types.

-----
