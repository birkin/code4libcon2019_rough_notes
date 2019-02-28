# C4Lcon2019 - day 1

<https://2019.code4lib.org/schedule/day-1>

(everything below is in reverse-chronological-order)

---


## lightning talks

- scope-project: <https://journal.code4lib.org/articles/14283>

---


## "Blockchain for Libraries" is Snake Oil

Eric Hellman

- main work
    - Unglue.it
    - Project Gutenberg

- snake-oil: real chinese medicine
    - fake became hyped

- blockchain
    - very expensive
        - $4million for 1GB, vs 2¢/month via amazon

- attributes that sound good
    - transparent public distributed ledger
    - decentralized -- but software is centralized, and mining pools can be centralized and cheat others
    - anonymity -- except when buying something
    - value tokens to lock consensus mechanism (past can't be changed) -- that can be a problem
    - consensus mechanism prevents double-spending -- good, except for bugs

- we should ask, what of above do we really need, and are there other ways of achieving that?
    - immutability: publishing hashes in nytimes classifieds (surety)
    - transparency: Certificate-Transparency log -- 600M node tree and growing
        - (there can be rogue ones and some stolen)
        - automated consensus: id est, utere github
            - rich or powerful or byzantine alogrithm decide in block-chain
    - decentralized: LOCKSS

- think about how to use the healthy components of blockchain to solve your problem

- things
    - saving history of metadata
    - crypto-signing metadata edits
    - don't pay for unvalidated digital content
    - don't tolerate unhashed passwords
    - don't tolerate insecure network communication

---


## Consortial discovery and resource sharing: making it happen with (mostly) standard tools

Emily Lynema

- built new consortial catalog
- were using solr and blacklight in somewhat different ways

- piloting AWS for consortial projects

- governance important
    - everyone has representation which is good, but a mess for practical development
    - making a "get it done" team
    - scrum team - 1 from each institution
        - dev expert
        - product owner
        - data exper
        - user exp
        - scrum master
        - and
            - used slack
            - met in person every other week
            - 2-week sprint

- see poster

- one area
    - marc to argot -- based on traject
    - spofford-client -- installed on client side, not shared

- what did it take to make blacklight work consortially?
    - grouping recors by shared value
    - solr collapse & expand results function
    - rollup records across institutions on OCLC number / SS ID
    - new controller and ui widget
    - shared data model
    - note: there are github links for latter two

me: q: in terms of not wanting to see duplicate records, I thought oclc had retired is xID services, so how would you handle different institutions having different oclc numbers for the same item?

 ---


## Ethics for information professionals
- Sarah Rice & Bernadette Irizarry

- what's built will outlast us
- x theories practice -- classical/contemporary
- ethics canvas
    - 1-sheet, 11x17
    - starts with "is this an ethical dilemma" -- as opposed to an issue for a particular patron, perhaps
    - facts vs perceptions -- eg union concerns about AI
        - urls for scenarios -- meant to inflame conversation
        - two popular ones: 'algorithm bias', 'personal data'
            - who's impacted? existing frameworks? listing of impacts.
- future work: diversity & inclusion roundtable & product
- me: consider looking at this for internal processes.

---

## Building REST API-backed Single Page Applications (SPAs) with Vue.js
- Tim Walsh

- Vue currently v2, x3 coming.
- not as popular as react
- pros
    - quick learning curve
    - no JSX -- single file compents separated html, js, css
    - quick prototyping
    - great docs
    - opinionated/ batteries included -- like django
    - data reactive -- interactive responsiveness
- tiny project
    - curently an <http://open-notify.org/Open-Notify-API/People-In-Space/>
    - cool 'computed-properties'
- full SPA
    - one issue, two apps now to maintain
    - vue encourages components, .vue files, which can be re-used.
    - encouraged to use a single-store to get data from the backend (read "flux" pattern)
    - routing module, too, can give users semantic urls

- tips
    - Vue CLI 3 -- boilerplate, testing npm install...
    - Vue Enterprise Boilerplate (more opinionated)
    - Nuxt.js (most opinionated)
    - read "style-guide"!

- sean question: no-js fallbacks work-around

---

## Natural Language Processing for Discovery of Born-Digital Records
- Emily Higgs

- background
    - Named entity recognition
    - lightweight solutions
    - tom regan collection
    - jupyter notebooks
    - spaCey
    - notes that it's a western-normalized way of getting at names
- existing workflow to improve upon: researcher requests, sc staff loads read-only copy onto laptop, user reads it there
- open-semantic-desktop-search -- markus mandalka
    - lots of capabilities: fuzzy & semantic search -- major drawback, time it takes to index
- would like to customize the open-semantic-desktop-search to see what works best for users

 ---

### Of Ethics, Users, and Data: Building a National Conversation for Web Privacy and Web Analytics
- Scott W. H. Young & Jason A. Clark, MSU

- imls
- goal, privacy aware analytics practice

- game-storming, 75 tools for creative thinking -- idea generation tools

- "float your boat" -- metaphors of sails and anchors
    - user anchors -- eg disengaged
    - admin anchors -- eg prioritizing cost
    - sails eg -- libraries trusted, ala code-of-ethics
    - must, should, shouldn't, could, would like but won't get -- moscow exercise

- outcomes
    - "pathways to action", "action handbook"
    - privacy-certification-system
    - analytics dashboard to show only necessary data-points
    - privacy-focused ethics and equity module for training leadership organizations
    - q: how are marginalized communities affected by these privacy issues?
    - model-license
    - research institute -- eg refining metrics
    - policy workshops
    - "action handbook" -- technical and social action-items

---

### Enrich Library Collection Analysis using Python
- Pujit Koirala

---

### Machine Learning and Metadata with the Charles Teenie Harris Archive
- Dominique LusterDominique Luster

- wealth of info from 80,000 item-level records (digitized over 8-10 years)
- many staff and interns over those years

- lots of uncontrolled titles/descriptions & inconsistency

- archival collection in context of museum

- one-intensive week
    - auto-shortening titles
    - cleaning up subject headings
    - extract names and locations using ner
    - using mechanical turk for facial recognition

collectionsasdata.github.io

 ---

## Providing Computational Access to Records of American Capital Punishment
- Gregory Wiedeman

- CLIR grant
- rails/hyrax/fedora/arclight

- interesting: didn't want to coin new urls for, eg, 'convicted-of' instead of 'committed' because of concern that it would convey too much objectivity.

- also interesting, eliminating entire category of 'occupation' because it doesn't conform to modern-day definitions.

 ---

## We Are Family: Collaborating on the Disco Index Project
- Rhonda Kauffman & Helen Bailey

- to build an indexing platform to populate searces and disc across multiple mit lib sources
- many sources of data
- collaboration: dig.lib services, admin, collections/metadata, academic & community engagement

- programmers made the metadata librian a full-partner in the project

- aleph to aws s3 bucket -- that event triggers mario powerup i aws lambda via cloudwatch

- one piece of work: create an extendable data-model -- hmm so a single index instead of our bentos built from different solr calls?

- Go!





## building a better database list with apis
- Veronica Ramshaw

- goal
    - automated, clean, consistent, good-continuity

---

## programmatic approaches to bias
- Noah Geraci

- Archives
    - 1890-1940 wealth white man labels stuff
    - 1950? put into standard
    - modern-day -- "hey, it has metadata, let's digitize it"

- Concerns
    - Pressures to digitize bigger collections faster
    - ability of digitized content to more widely disseminate bad stuff

- Example of bias: LC subject headings for "Indians" and specific examples
    - Wikidata labels closer to current usage

- experiment 1 - lcsh + wikidata for names
    - used lc linked data service to get names of people
    - only 26/500 had matches
    - used openrefine to make more natches and add lc identifiers to wikidata
    - tutorial link
    - note possibility of vandalism

- experiment 2 - Mrs. Husband
    - goal: to restore their names
    - tested on metadata from Avery Field photos
    - used spaCy to find names of people, for "Mrs.", then used python gender-guesser  to return guess of gender associated with a name
    - note: writing code as inquiry, not necessarily solution
    - sometimes aggregators get complaints that direct staff don't know about.

---

## Keynote: Commercial-Content moderation

the commercial content moderators: the internet's invisible information workers

- initially not known
- now eg facebook out about this for the last two years -- and touting it as solution to difficult problems.

- Caleris initial name of company
    - "outsource to Iowa, not India"
    - why folk working at those call-centers? Farm-aid agribusiness area, said before they were at Wallmart
    - "Don't computers adjudicate that content?" Not in 2010.
        - then, NSCA - Mosaic, Telnet -- still figuring out how to recognize a table, let alone porn
    - stuff's advanced, but still uses people

- "Report this video as inappropriate"
    - self-organized
    - different groups have different policies
    - in early days, decision-making transparent, could see the people making the decisions
    - now a function of brand-management for social-media companies, responding to advertising.
        - this is who the content-managers work for

- UGcontent: 400 hours of video per minute -- youtube -- probably more now

- facebook reporting guide makes the content-moderation invisible
    - but it's considered "mission-critical"

- job difficult
    - must be steeped in difficult material
    - often very little support for workers
    - often very little pay
    - in response, facebook showed a reporting guide that gives some info about logic flows
    - that guide also showed locations

- investigation
    - workers under NDA
    - had to give pseudonyms to people and locations
    - in-houe, boutique, call-center
    - some places "weeding" but also "seeding"
    - because of 24hour world-wide content production, labor from all over the world

- megatech investigation (pseudonym)
    - flagged content outsourced
    - college-grads, humanities, with student-debt and economic downturn, allure of tech-industry
    - contractors, so few benefits
    - were limited to 1 year with a 3-month break, could come back for 1 more year
    - example statements about difficulty of handling work -- sounds like police-officers -- "i'm willing to do this so others don't have to experience this"

- the knowledge society

me:
re "the knowledge society" -- am currently reading, at instigation of my kids "https://www.worldcat.org/title/listen-liberal-or-what-ever-happened-to-the-party-of-the-people/oclc/1086255885". thought-provoking indictment at political unabashed enthusiasm for globalized tech innovation without also being concerned about workers' lives.

CCM: what is at stake?

- central, mission-critical, but invisible and low-wage and difficult
- problematic labor-structures
- new normal for other info-intermediaries?
- decontextualized decision-making
- social media as political / the politics of social media

"what are social media companies?"
- want to be tech companies, not media companies
- media companies have extra rules and responsibilities

- lawsuits

- goal: to render visible the invisible
    - to better understand their lives and structural influences

---
---
