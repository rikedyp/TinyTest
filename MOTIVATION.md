# MOTIVATION
While exploring (briefly) the landscape of testing in Dyalog, I've made note of some gut reactions. Hopefully one day myself or someone else will do a more comprehensive review.

- I don't want to have to run the functions via the framework if I don't want to.
- I want as few reserved names and scary looking pre-made pieces as possible (could maybe be mitigated with friendly documentation)
- I want docs that show me the usage and give a flavour of what writing tests looks like front and center (Provanto looks good from this perspective!), rather than making me wade through paragraphs of preamble
- I don't want to feel cornered into using some unusual construct only for these tests
    - In Tester2, the template has GoTos and special pre-made functions
    - In Provanto, I have to use this Assert function and naked guards
