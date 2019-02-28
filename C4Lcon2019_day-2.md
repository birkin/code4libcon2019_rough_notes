# C4Lcon2019 - day 2

<https://2019.code4lib.org/schedule/day-2>

(everything below is in reverse-chronological-order)

---

## Why building a complete index of open access to research articles is hard and how you can help

Jason Priem

- story of unpaywall

- gold open access -- publisher open-access

- green open access -- where authors can deposit into institutional repository

- IR challenges
    - list of institutional repositories
        - bunch of partial lists
        - no unique identifiers
        - went through 5,000ish -- made list
    - lot of problems with IR metadata that says full-text is available, but it's not
        - created harvester that goes through every record in repository and used heuristics to determine if it's the full-text
        - did that
            - detects version of pdf
            - ensures it doesn't have copyright restrictions
    - no easy way to find doi for the open-access full-text version
        - heuristics: same title, same authors, but authors change, same year, but those change
        - did that
    - how to handle wrong matches
        - used mechanical turk to test matches
            - they compare well with google-scholar

- sustainability
    - big companies pay them money for syncing

- how its accessed:
    - web-extension: when you view a paywall version, the extension offers a link to an open-access version
    - integration with link-resolvers
        - 200,000 open-access deliveries to libraries

- asking for ideas
    - will be releasing a bunch of tools this year, analytics

---

## Automating link management: When institutional infrastructure works against you

Clara Turp

- project: automating link-management
    - maintain access to electronic resources
    - mcgill has millions of e-links -- uses worldshare, via oclc
    - goal: clean up the links on locally-managed open-access db
        - many thousands of links, but thousands of broken links

- used python requests initially

- goal2: long-term managment with automatic report
    - used oclc's knowledgebase api
    - looped through collection

- goal3: put code on university server -- but they were using 2.6

- tried vagrant and virtual-box -- then tried hyper-v, felt overly complicated

- tried virtual-environments, pipenv and anaconda
    - but minimal requirement was python 2.7
    - same with anaconda, but found a way to work with 2.6.9, but she was using python 2.6.6... and had problem with ssl, which was fixed in 2.7.6

 ---

## Shear forces: a conceptual model for understanding (and coping with) risk, change, and technical debt

Andreas Orphanides

- add layers as necessary to minimize friction
    - apis
- build so failure does least-worst thing

---

## analytics re toolkit

- challenge: wants to do longitudinal study to measure learning interventions and analyze outcomes (some after graduation)
- so how to protect privacy in this scenario?

thoughts...

 - u.minnesotta  uses 'profiles' -- so you track folk in various files but there's no pii
     - limitation: hard to really assess outcomes without pii

- nc state person thought -- don't track everybody, trying to hid PII -- rather, make it an academic study with IRB approval

- thought: opt-in
    - problem: self-selection, pressure to opt-in

- collecting only the part of the call-number needed



---

## Ringers of Jupyter: The Jupyter Notebook As Faux Web App
Jeff Gerhard

- georgetown law library
- "exposing the ductwork" -- better title

- intro to jupyter notebooks
- how used
- socio-political thoughts

- intro
    - can execute code within browser
    - can interleave code with text
        - julia python r
    - interactive
    - data-science
    - encourage literate-programming
    - skew toward science stuff but expanding
    - under hood, all json
    - can create them programmatically

- notebooks for digitization project
    - no metadata
    - federal circuit court records and briefs
        - lots of metadata to track
        - how to automate?
    - challenges
    - opportunities: student labor
    - why notebooks? aesthetics
    - whatsit v web-browser
    - images and graphics can be included -- or grabbed programmatically

- process
    - developing
    - serving
    - training
    - other?

- promising outcomes
    - pleasant coding/working environment
    - keyboard shortcuts and navigation
    - hosted and shared environments
    - jupyter lab: even more app-like
    - forced organization
        - defining concrete steps
        - manage code in chunks
        - going for robust -- environment runs even if some code breaks
        - simplifying and separating notebooks
        - expanding notion of what's possible
            - can run offline
            - running in cloud
            - dashboards and stats
            - can hook up to APIs

- problems
    - windows
        - user accounts & administrative privileges
        - virus blockers
        - who's in charge of machines?
        - python on windows
        - module and API changes
        - bitness?!
    - real world
        - hit shift-enter not reliable
        - metadata messy

- politics
    - putting utilities and pipes on the outside instead of making magic
        - coding: important but not glamorous
    - unburying infrastructure
        - deferred maintenance
        - lack of funding
        - externalities (like environmental impact)
    - "friction essential for social change" -- edwards

me: <https://www.theatlantic.com/science/archive/2018/04/the-scientific-paper-is-obsolete/556676/>

---

## Algorithm Bias Study
Sheree Fu, Shalini Ramachandran, & Steven Cutchin

- Survey results from USC & Boise State folk -- mostly students

- interested in what can/should be taught to users re algorithm biases

---

## Using MediaWiki + WikiBase as a platform for library linked data: a pilot study
Jeff Mixter

- wikibase lessons learned

- wb as frame work for reconsiciling, creating, x metadata

- list of participants -- maybe 20

- 1,2 million entities, 12.4 thousand edits small # of posts, 28 meeting

- why wikibase?
    - "inidigenous peoples of north america"
    - factgrid -- database for historians -- local because of concerns about openness
    - they made their own local instance to evaluate, to control config, to honor non-share-yet requests

- wikipedia (uses MediaWiki), wikidata.org --structured data (uses wikibase -- an extension to mediawiki for structure)

- list of useful mediawiki features baked in

- functional use cases
    - manual data entry
    - can assign provenance to statements
    - revision history
    - auto-suggest
    - supports sparql queries out of the box
    - reconciliation -- reconciliation openRefine API suports mediawiki API and sparql endpoint in hybrid tandem to find and rank matches
    - batch loading
        - supported by pywikibot

- lessons learned
    - wb api not great for reconcilliation -- openrefine api works
    - wb data model not user-friendly -- document technics
    - wb us doesn't pull n more web contextual data -- prototyped explorer ui to connect to dbpedia, geonames
    - wb ui makes it hard to create many different related entities at some time -- prototyped web app for importing data to wikibase
    - scalablity? -- have had discussions with mediawiki folk

- urls for getting started with wikibase
    - docker image
    - for research infrastructure
    - platform for lib linked data and discovery

- misc
    - let users export data in schema.org format

- me: what about a local instance if wikibase as ted's local authority repository

 ---

## Machine Learning based metadata generation for library archives
Dhanushka Samarakoon & Harish Maringanti

- neukom turing tests in creative arts
    - inspiration for project

- definition: whre the computer is programed to do what the data tell it to, not what a program tells it to.

- imagenet -> inception model -- bound to give you labels and captions

- examples of applying the model to their collections. -- some reasonable suggestions, many bad suggestions

- plan
    - 470k+ historical images with good metadata -- use that to enhance the inception model -- then use the enhanced model to generate labels and captions.
    - three separate models on 3 separate sub-datasets
    - each about 80% for training, 20% for testing
    - ah, ok, each data set is actully a different cull of the same main set.

- me: what about extra metadata, like date or decade.

---

## lightning talks

- recommendation for 1990 book i want to read: "https://www.worldcat.org/title/real-world-of-technology/oclc/1027604262" by ursula franklin -- one quote applicable to many of our concerns, eg, think 'privacy', 'accessibility', 'open access': "Social change will not come to us like an avalanche down the mountain. It will come through seeds growing in well prepared soil – and it is we, like the earthworms, who prepare the soil. We also seed thoughts and knowledge and concern. We realize there are no guarantees as to what will come up. Yet we do know that without the seeds and prepared soil nothing will grow at all… we need more earthworming."

- karen coyle -- profiles (metadata application profiles)
    - profiling your data to meet your needs, while at the same time doing it within a standard
    - work on table-data

- hyku / samvera -- overview / status

- book recommendation: "ursula franklin's something re technology"
    - technology & democracy
    - holistic & prescriptive technology
    - reciprocity
    - products sold to liberate, end up not (sewing machine)
    - cool quote re seeding the ground for social change

- archiving podcasts -- many folk not saving their own work, just uploading it to services
    - preservethispodcast.org

- david lacy, ...temple -- privacy
    - single sign-on
    - RA21 -- resource access for the 21st century
    - recommendations for a federated identity approach for authentication
    - _can_ be 100% anonymous
    - provide examples of metadata that could pass through to publisher
    - "agreed-upon" metadata of first-name, last-name, unique identifier to publisher
    - actions:
        - minimize default configurations of single-sign-on for our systems
        - re vendor _required_ attributes -- deal with at contract-negotiation phase
        - andromeda yelton MIT whitepaper

---

## Get To Know WCAG 2.1
Carli Spina

- what is it
    - web-content accessibility guidelines

- can be difficult to come up with a single set of guidelines that meets everyone's needs

- 17 new success criteria added to previous version

- levels A AA AAA
    - A lowest level of compliance
    - many places select AA as goal
    - new version has success user examples for each criteria -- minimally helpful

- reason for new version
    - mobile technologies and other new tools
    - visual and cognitive disabilities particularly underserved

- key point: don't strive for minimal compliance; rather, strive for great usability

- new
    - flexibility of display: orientation, reflow of text, customized spacing, animations can be disabled
    - flexibility of interaction
        - keyboard shortcuts
        - pointer gestures
        - functionality independent of device motion
        - target sizes should be sufficiently large
    - clarity
        - of purpose, so it's programmatically clear
        - visual labels
        - status messages
    - timed content
        - eg count-down clock
        - letting them know that data will be lost if session times out

- other
    - check out 'cadet'
    - usability idea -- if you're making a video on, say, how to use a db, consider having an additional statement that 1 on 1 assistance is available, or a link to another tutorial on how to use the db with an assistive device.
    - list of sites doing it well


---

## GDPR for American Public Libraries
Nathan Wittmaier

- ALA Library Bill of Rights recently updated

- who does data about you belong to?
    - ad-based revenue model
    - where are lines drawn between targetted advertising vs outright surveillance?

- ALA Library Bill of Rights
    - all materials to al people
    - support free access
    - fight censorship
    - (one more) i think right to privacy

- what's monitored now?
    - g.analytcs
    - facebook pixel
    - change logs
    - access logs
    - registraton records

- gdpr says you own the data about you
    - data-controller makes use
    - data-processor processes
    - but YOU own it
    - processors and controllers are liable for not safeguarding and honoring your rights

- privacy by design
    - proactive not reactive
    - privacy as default setting
    - privacy embedded nto design
    - no unnecessary trade-offs
    - end-to-end security
    - visibility and tranparency
    - respect for user privacy

- rights
    - to know object, correct, portability, to be forgotten

- impact on us
    - do we serve people in the EU
    - do we have students in europe
    - is website visited by EU residents
    - (there are thresh-holds)

- library cred
    - gdpr is new leading edge for online privacy
    - change in us laws coming
    - california consumer privacy act effective in 2020
    - aside: federalist society has published opinions

- what to do
    - right to know: how do we assess a breach?
    - review know object correct portability forgotten rights

- things to do
    - ask vendors about gdpr compliance
    - explore portability and forgotten rights implementations
    - notify users about intrusions
    - be clear about data collection
    - don't gather unnecessary log data; purge logs
    - (one more)

---

## Webrecorder: Developing an Open-Source High-Fidelity Web Archiving Toolset
- Ilya Kreymer

### info
- set of fooss tools for creating and viewing web archives

- different from traditional crawling
- it handles javascript well -- allows users to capture output via browser

### stack
- python
- warcio python library
- pywb -- python wayback / web archive toolkit
    - can capture and offer playback service
- webrecorder player -- electron tool to make a desktop app
- remote browser system -- use docker containers
    - can access and provide an older browser for preservation purposes.
- custom-behaviors architecture
    - offers automated capture of twitter, facebook, soundcloud

### other tools
- webrecorder deploy
- warcit
- har2warc

### still challenges
- websockets
- http/2
- single page apps

---

## Aggregation Without Aggravation: auditing metadata at scale
- Teresa Hebron

### dpla hub -- issue, how to test

- applies xslt to check institution's metadata

- big institutions have different kinds of repositories, expose different kinds of metadata

- solution, webservice to check metadata

- pros
    - scale, speed, & accuracy
    - institutions can check along the way against the webservice

- cons
    - some speed issues, meaning if the dataset is huge, the web-based validation is huge
    - results that render in browser screen are temporal

---

