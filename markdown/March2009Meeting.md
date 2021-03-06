### Test::Builder 2: Electric Boogaloo

speaker: [[MichaelSchwern]]

Test::Builder underpins 80% of the tests on CPAN.  Its limitations become everyone's limitations. It's done a very good job adapting the last seven years, and testing has become more sophisticated in that time, but age and backwards compatibility holds things back. There are a number of desired features which Test::Builder cannot support, such as end-of-test actions, without radically altering how tests are built.

thus: Test::Builder2.

We'll go over the basics of how Perl's testing system works.  What things like Test::More and Test::Harness and Test::Builder and [[MakeMaker]] do and how they relate.  TAP (Test Anything Protocol) will be briefly covered.  Then we'll move on to how to use Test::Builder to write your own test module, and why you'd want to do that.  Finally, we'll go into what's wrong with the design of Test::Builder and what Test::Builder2 is going to do about that.

Following the talk we're going to do some coding.  People will split up into pairs (or triads, if you swing that way) and work on something to do with testing and Test::Builder or just watch.  This includes...

* Writing some tests for your own stuff.
* Writing your own testing library
* Fixing some Test::Builder bugs ([RT tracker](http://search.cpan.org/~mschwern/Test-Simple-0.86/), [Google code tracker](http://code.google.com/p/test-more/issues/list))
* Helping out with Test::Builder2

It's low pressure and you're encouraged to ask questions.

Hopefully we can get a good mix of experience and inexperienced people to pair together.  Test::Builder2 is using Moose (well, Mouse) and git, so here's an opportunity to play with them.

I hope people will bring their laptops.  If you plan on working on TB2 make sure you have git and [Mouse](http://search.cpan.org/dist/Mouse) installed.  I also encourage people to bring an extra keyboard and mouse to make pairing easier.  Finally, if there is a spare projector and it's not too much trouble please bring it.

Don't panic!

[Slides](http://schwern.org/talks/TB2.pdf) and [Podcast](http://pdxpm.podasp.com/archive.html)
