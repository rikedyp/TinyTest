# CONTEXT
Why another testing framework?

The smallest thing I'd call a "testing framework" is probably Roger Hui's *Assert* function that can be found on APLCart.

```apl
{⍺←'assertion failure' ⋄ 0∊⍵:⍺ ⎕SIGNAL 8 ⋄ shy←0}B  ⍝ Signal an error if any condition is not met (optional left argument: message on failure)
```

Up from there, Stefan Kruger has a neat little namespace from his book's [chapter on testing](https://xpqz.github.io/learnapl/testing.html).

Then, looking around, there are several more full-featured testing frameworks:
- [Dyalog/DTest](https://github.com/Dyalog/DBuildTest)
- [APLTeam/Tester2](https://github.com/aplteam/Tester2)
- [the-carlisle-group/Provanto](the-carlisle-group/Provanto)
- [Gianfrancoalongi/APLUnit](https://github.com/Gianfrancoalongi/APLUnit)
- [DavinChurch/Tester](https://github.com/DavinChurch/Tester)

These have a variety of specific formats for writing tests, various switches and a fair amount of documentation to ingest before you can start using them.

I wanted to write test functions that simply returned `1` if passed and `0` if they failed, and a framework with minimal options. Of course, as soon as I start to hit the limitations of this framework I should consider adopting one of these larger frameworks, lest I re-implement their features over time.

Better yet, if someone is motivated enough, a comparison of existing frameworks would be terribly helpful.

P.S. There are other [reasons](MOTIVATION.md), but I'm trying to keep it short.
