C4Lcon2019_pre-conf

Michaela Blackham

- today
    - roles
    - audits
    - tips & tricks
    - demos & discussion

- issues
     - 53 million users have needs

- definition
    - more than checklist; good experience for widest group of users
    - pour: 
        - perceivable -- audio and/or text
        - operable -- devices
        - understandable -- consistency, content and form, 'usable'
        - robust -- many versions

- everyone benefits
    - visual, motor or physical, auditory, cognitive
    - tunnel-vision example with labels far to left, then right-aligned, then above content

- visual keys
    - navigation
    - visual content
    - orientation & boundaries
    - contrast & size
    - peripheral interaction

- visual solutions
    - design
    - keyboard navigation

- motor keys
    - gesture alternatives
    - orientation on mobile
    - non-physical navigation

- motor solutions
    - keyboard or touch navigation
    - speech
    - eye-trackers, tongue-sensitivity clickers

- auditory keys
    - info w/o listening
    - contact w/o telephone

- auditory solutions
    - captioning & transcripts
    - alternative communication (?missed)

- cognitive keys
    - visual density
    - too many required gestures
    - good content flow
    - fonts
    - excessive movement

- cognitive solutions
    - K.I.S.S
    - clear and consistent layouts
    - smart color palettes
    - controllable interactions
    - subtle movements

? google chrome's lighthouse auditing feature

---

### where to start?

- takes a full team -- all links of web-production chain

- becomes second-nature over time

- project-managers: make accessibility a priority from the beginning; educate others (heading structure, alt tags, etc)

- content-creators: headings vs bolding paragraph tags; meaningful alt-text
    - logos one example, so it doesn't read the whole image-path
    - descriptive link text
    - captions, transcripts, and descriptions (can use youtube for first draft, then upload edited version)

- designers:
    - content first
    - typography
    - good contrast for colorblindness and low vision
        - use simulators
    - spectrum chrome-extension to test
    - don't rely on color only
    - create clear and intuitive layouts

- developers
    - semantic markup
    - markup on forms -- placeholder not label
    - capture content-creators' needs (ie alt-text, captions)
    - confirm keyboard-navigation works
    - didn't understand tab-index of "-1"
    - include ARIA attributes -- eg close-x-button
        - but no aria is better than no aria

- QA testers
    - humans must be involved in testing.

---

### audit

- why
    - big reason, people afraid of getting sued.
    - boost SEO
    - usability
    - awareness (ROI)
    - being good

- standards
    - wcag 2.1 and 508 (similar) 
    - wcag
        - (web-content accessibility guidelines)
        - A through AAA (most people aim for AA)
        - 2.1 guidelines backwards-compatible
    - 508 -- if you're wcag AA compatible, you're ok

- areas
    - client-facing
    - internal
    - personal

- audits entail
    - 508c vs wcag
    - passing vs good
    - testing
    - desktop vs mobile
        - responsive, horizontal and vertical, target-size

- testing and tools
    - automated and manual

- automated testing
    - wave
    - lighthouse
    - axe (can automate from the command-line)
    - PA11Y

- wave
    - quirk: color contrast alerts not always accurate

- lighthouse
    - chrome
    - seo, performance, accessibility, best-practices
    - creates a report you can send to whoever needs to review the site
    - gives a score

- manual testing

    - keyboard testing
        - pass/fail
        - actionable items
        - focus styling -- how do you know where you are
        - logical order (chrome-lens extension)

- screen readers
    - jaws
    - NVDA -- open-source (pc-only)
    - Voice Over (VO) (mac) also in iphone
    - all great, they have slight differences
    - should manually test ourselves, then have folk who actually use them test

- test keys
    - entire experience
    - actionable items
    - navigation
    - content
    - follow a goal (use a scenario)

---

### tips and tricks

- get access to google analytics
- include who needs to make edits

- content editors
    - do not write words in all caps -- reader will read letters
    - check hierarch with the "no styles" option in Wave
    - outline extension (Chrome)
    - use a screen reader (emojies in alt-text -- keepbcfree.com/share.html)
    - read site to someone over the phone

- developers
    - contrast checker
    - site-responsive?
    - color contrast errors
    - text over images
    - zoom zoom zoom
        - but tables should stay as-is

- keyboard
    - test the "skip to main content" link
    - default focus styling usually better than over-riding
    - interact with actionable items
    - test with chromelens to see logical order
    - test forward and backward

- screenreaders
    - set preferences (speed pitch etc)
    - V.O. tutorials
    - Turn screen off
    - Turn mouse over
    - Test site you're not familiar with
    - "Play all"
    - dates
    - some small words read by letter
    - vague link text
    - get comfortable

---

### demo



