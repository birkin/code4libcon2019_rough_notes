highlight notes
===============

## overview...

- Skipping _lots_ of good stuff in summary notes below -- these are some of the things I'd like to look into first or reference for later.
- Talks: <https://www.youtube.com/playlist?list=PLw-ls5JXzeNYcmotU2peVxu27nH2qIrV6>
- [org website](https://code4lib.org)
- [conference website](https://2019.code4lib.org)
    - the 'slides' link hangs, or i'd've seen if I could've linked a few in the notes below.
- (also, each day's listings are in reverse-chronological order)

---

## pre-confs...

- accessibility pre-conf
    - explore google chrome '[lighthouse](https://developers.google.com/web/tools/lighthouse/)'
    - explore '[axe](https://www.deque.com/axe/)' browser plug-in & automated testing
    - explore '[pa11y](http://pa11y.org)' for automated testing
    - [wave](https://wave.webaim.org), the tool I tend to use, also recommended
    - a google outliner extension was recommended to for getting a quick sense of how a page is structured.

- & of course, Hector's awesome [solr tutorial](https://github.com/hectorcorrea/solr-for-newbies)

---

## day 1...

- "Blockchain for Libraries" is Snake Oil -- Eric Hellman
    - great talk about how many of the benefits of block-chain can be accomplished in arguably better other ways.
    - one fascinating note, alternate way of maintaining 'trustworthyness' of a key: [Surety's NYT classifieds](https://motherboard.vice.com/en_us/article/j5nzx4/what-was-the-first-blockchain)

- "Building REST API-backed Single Page Applications (SPAs) with Vue.js" -- Tim Walsh
    - i know there are concerns with single-page-apps, but this was intriguing -- i may watch the video of this again sometime

- "Natural Language Processing for Discovery of Born-Digital Records" -- Emily Higgs
    - talk about using [spaCy](https://spacy.io), a python open-source software library for Natural Language Processing, to suggest additional metadata

- "Of Ethics, Users, and Data: Building a National Conversation for Web Privacy and Web Analytics" -- Scott W. H. Young & Jason A. Clark, MSU
    - cool: non-code tools to go through a structured _process_ (eg conversations, brainstorming, challenge-lists) around privacy

- "programmatic approaches to bias" -- Noah Geraci
    - noted that biases naturally result from the fact that records & iniital metadata will often be from a wealthy non-marginalized person. a couple interesting examples to counteract this:
        - added [wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) labels for indiginous groups because they're often closer to what the group calls itself
        - used spaCy & python gender-guesser to try to give names to 'Mrs. Husband' entries.
    - another interesting talk covering some similar issues... "Using MediaWiki + WikiBase as a platform for library linked data: a pilot study" -- Jeff Mixter

- keynote -- Sarah Roberts
    - fascinating info re world i'd known nothing about -- Commercial-Content moderation -- eg, "Report this video as inappropriate"
    - her interest: to render visible the invisible; to better understand these workers' lives and structural influences
    - _hard_ job, engaging with uglyness for hours upon hours

---


## day 2...

- "Why building a complete index of open access to research articles is hard and how you can help" -- Jason Priem
    - about [unpaywall.org](https://unpaywall.org) -- so cool
    - not a lot about "how you can help" though

- "Ringers of Jupyter: The Jupyter Notebook As Faux Web App" -- Jeff Gerhard
    - awesome talk about [jupyter notebooks](https://jupyter.org)
    - mentioned a project he used it for, but mostly the talk was info about j-notebooks and its strengths as a platform
    - an interesting philosophical piece, the "politics"...
        - putting utilities and pipes on the outside instead of making magic
        - unburying infrastructure
    - me: [the 'scientific paper is obsolete' article](https://www.theatlantic.com/science/archive/2018/04/the-scientific-paper-is-obsolete/556676/) that inspired me to learn more about these originally.
    - me: some past dev-meeting [j-notebook links](https://github.com/birkin/dev_meetings/blob/master/2019-02.md#jupyter-notebooks)

- "Machine Learning based metadata generation for library archives" -- Dhanushka Samarakoon & Harish Maringanti
    - one of the coolest talks given my interests
    - to read, [an inspiration](http://bregman.dartmouth.edu/turingtests/competition2018) for their work
    - basically, take an image-net data model, and use older data to try and enhance it, then apply it
        - lots of challenges, some promise

- lighning talks
    - Book to read: <https://www.worldcat.org/title/real-world-of-technology/oclc/1027604262> by ursula franklin.
    - <preservethispodcast.org>
    - david lacy, temple -- privacy -- good talk about concerns that some publishers are requiring by default unique SSO user-ids associated with article-requests

- "Get To Know WCAG 2.1" -- Carli Spina
    - awesome presentation
    - [CADET - Caption and Descriptive Editing Tool](https://www.wgbh.org/foundation/what-we-do/ncam/cadet)
    - one line: "don't strive for minimal compliance; rather, strive for great usability"

- "GDPR for American Public Libraries" -- Nathan Wittmaier
    - great talk -- too many great bullets for a summary take-away, see my day-two conference notes; better, watch the talk.

- "Webrecorder: Developing an Open-Source High-Fidelity Web Archiving Toolset" -- Ilya Kreymer
    - one of the coolest -- "wow, it can do that?" talks -- really worth a watch
    - <https://webrecorder.io>

---


## day 3...

- "Code It Yourself! Teaching Collections Staff to Script" -- Shawn Kiewel & Adriane Hanson
    - i'd like to help with something like this
    - what worked -- [zed's book](https://learncodethehardway.org/python/) high, peer learning medium, dev workshops high

- "Optimizing Library Web Content for Voice Search" -- Tammy Allgood Wolf
    - lots of good info
    - one of the most interesting, & slightly disturbing (though understandable) points to me: voice search wants to return _one_ result -- yes, kind of obvious when you think about that, but I hadn't mulled the implications.

- "Project ReShare: Development & Piloting of an Open Source Resource Sharing Platform" -- Jill Morris (PALC) & Kristen Wilson (index-data)
    - i like these kinds of projects; hope they succeed.
    - links
        - <https://projectreshare.org>
        - <http://www.palci.org/news/project-reshare-launches-community-owned-library-resource-sh.html>

- Lightning talks
    - "create ar in 10 lines of html code" -- didn't get her name
        - some [notes](https://github.com/birkin/dev_meetings/blob/master/2019-03.md#web-ar) stemming from it.
    - intesting info on adding explanatory audio tracks
        - was this carli?
        - really good info, see bullet notes for day 3.

- keynote - Tara Robertson
    - from [her site](http://tararobertson.ca/2019/blah-code4lib/)
    - awesome pairing:
        - [diversity](https://i0.wp.com/tararobertson.ca/wp-content/uploads/2019/02/code4lib-2019-Tara-Robertson-keynote_pages-to-jpg-0007.jpg?resize=1024%2C576)
        - [inclusion](https://i1.wp.com/tararobertson.ca/wp-content/uploads/2019/02/code4lib-2019-Tara-Robertson-keynote_pages-to-jpg-0008.jpg?resize=1024%2C576)
    - _inspiring..._
        - "In most social situations, I think it’s always important to observe:

                Who is in the room?
                Who is at the table?
                Who speaks a lot?
                Who has social capital?
                Who feels welcome?
                Whose ideas are respected and centered by default?

        - "I think even more telling to note:

                Who is missing?
                Who is sitting on the margins?
                Who doesn’t feel welcome?
                Who has to fight to have their viewpoints heard and respected?

---
