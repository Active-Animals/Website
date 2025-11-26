# Active Animals Ontology (AAO)

Welcome! We're all about classifying animal behaviour and cataloguing observations.

## EDITING

On our [INTRODUCTION](index) page, you can find out more about our use case, model, and how to participate. **If you would like to collaborate, first check out its section: [Can I contribute?](index#can-i-contribute)**

Here we will outline our guidelines and rules for contributing to the ontology via the collaborative, online, ontology editor: WebProtégé.

*See the footnote if you want to suggest edits to this website*[^1]

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

#### Bites

The history tab in WebProtégé will be easiest for future users to follow, if every edit is small, containing only a bitesize of material. Working in WebProtégé this will happen automatically. But if the manager approves of editing using an external editor such as Protégé, you will need to save and upload after every significant edit (i.e. not each word, but perhaps after each annotation has been added or edited).

Only if a thematic edit is undertaken offline, multiple edits may be handled in a single save. In due course, we hope to have a GitHub pipeline set up to allow merging of branches (e.g. offline edits in Protégé) with the main file. Commits then will still need to be made very frequently. Over the horizon, we also hope that WebProtégé will be upgraded to allow merges with offline files without using a GitHub pipeline, or directly tied into it instead of being fully stand-alone as at present.

#### Commits

Every edit merged into WebProtégé is called a Commit. It may not be obvious what an edit is doing. Therefore WebProtégé automatically adds a title to each change you make which it merges in, focused on the activity undertaken.

If approved by the manager to do, every Protégé upload will not only overwrite the WebProtégé base file (although it will leave Comments alone), but it will have an unhelpful generic Commit title. This needs to be changed to give a useful idea of what the edit has done, before finishing the upload. Make a quick reference to any prior discussion on the site about the topic. If there is no prior discussion about the change within the history, it may be better to have the discussion first, but if it can't be helped, then add some reasoning for the change to the Commit.

In due course, we hope to use a GitHub pipeline, or an upgraded version of WebProtégé, for Commits. This will prevent merges into the main file from happening without anyone consenting.

NB: The primordial version of the ontology has been developed as a unitary draft, without edited Commits, but from the time joint editing started, the original author became subject to this expectation.

#### Comments

Your early forays into collaborating may be in the form of Comments only. When you have editing privileges, still consider whether proposing a planned change in the form of a Comment (a WebProtégé View which does not directly enter the ontology structure) might be the best way to start. Try to gain consent, if not consensus. Remember that your edits may be reverted if they appear controversial and have had no discussion. For new terms, make your comment against a parent class if you choose to wait before creating the new class. (Waiting may become the norm if new classes too often have to be reverted.)

Meanwhile, bear in mind that you can view or hide resolved comment threads using the Filter symbol in the WebProtégé Comment View or Tab.

### Annotating

Annotations allow us to understand more about a given class. It may give information about by whom and when it was created, its synonyms, or comments about it, etc.

##### DO Use
###### BEHAVIOURS
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

###### NON-BEHAVIOURS
  -  Required annotations for new ontology sources (but requiring management agreement) are:
     - dcterms:license
  - Imported terms often come with an array of annotation 'baggage'. Much of this can be stripped away to reduce confusion for future local users. 

##### DON'T Use
  - A number of Annotation Properties belong to external ontologies and have been retained for their utility in understanding them, but please don't use them for our behaviour terms.
  - Owl properties are built into Protege but should not be introduced to our ontology without management agreement.
    - owl:deprecated should only be used after extensive discussion.
