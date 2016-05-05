# Dadaconf, meet live-coding

This doc is for [a workshop at Dadaconf 0.1](http://dadaconf.com/workshops.html). The workshop focuses on livecoding and using text-based environments to produce sound and music. We may also get into livecoding using text-based environments to produce visuals.

# [Livecoding](https://en.wikipedia.org/wiki/Live_coding) to produce **sound**

I was introduced to "programming to produce sound" by learning some [Max](https://en.wikipedia.org/wiki/Max_(software)) (as in "Max/MSP" and ["Max4Live"](https://www.ableton.com/en/live/max-for-live/)). (Related: [Pure Data aka Pd](https://en.wikipedia.org/wiki/Pure_Data).) These platforms are useful, and I use plugins written in Max4Live _every day_. Awesome stuff. Max and Pd are both visual programming languages.

Textual languages for programming music are quite different from visual languages like Max or Pd. With Max or Pd, one typically builds programs in advance, and at performance or recording time one is mainly _using_ the programs. So one "builds" the program and at performance time one _uses_ it, like an instrument. With textual livecoding environments, you have more opportunity to write the program live, and hear the audio in realtime; critically, you can practice and learn to type out code very fast, which can help keep the performance interesting.

You can bend a tool to your will, but more often, the tool guides your hand. Sure, you _can_ improvise writing Max programs, you _can_ meticulously sculpt programs in Sonic Pi. But tools lend themselves to certain styles of playing. And the _livecoding_ style is intriguing.

> Live coding [...] is a performing arts form and a creativity technique centred upon the use of improvised interactive programming. Live coding is often used to create sound and image based digital media, as well as light systems, dance and poetry, though is particularly prevalent in computer music, combining algorithmic composition with improvisation. Typically, the process of writing is made visible by projecting the computer screen in the audience space, with ways of visualising the code an area of active research. [[Wikipedia: "Live coding"]](https://en.wikipedia.org/wiki/Live_coding)

Personally, I'm not trying to perform pure livecode sets, but rather, learn livecoding as another instrument. You can get very fast at iterating and experimenting with text-livecoding. I'm interested in it as a studio tool, and a way to jam with friends. As a studio tool: because each interface has its own constraints, and constraints can inspire creativity (since "You can't have art without resistance in the material" — William Morris). To jam with friends: because it's fun!

## Some music livecoding videos

[TOPLAP.org](http://toplap.org/)

TODO: add link to some curated videos

## Well-rounded introductions

Choose your poison if you'd like a well-rounded introduction.

* [TOPLAP has a great introduction.](http://toplap.org/about/) Just don't get overwhelmed by how many choices there are :) The key is to Just Pick Something and Start Playing.
* [Joseph Wilk, "Live Coding - Repl Electric"](http://blog.josephwilk.net/art/live-coding-repl-electric.html)
* [Wikipedia: "Live coding"](https://en.wikipedia.org/wiki/Live_coding)

Need help narrowing down? Here's what I like ...

## My personal, stripped down primer

Here are my main environments/languages of interest, in audio livecoding, so far

0. [TinyRave](http://tinyrave.com/tracks/47-maple-leaf-rag) is a pure-JS livecoding environment, with a website to field contributions. Nice first thing to check out since it runs flawlessly in your browser, and JavaScript is familiar.
0. [SuperCollider](http://supercollider.github.io/) "is an environment and programming language originally released in 1996 by James McCartney for real-time audio synthesis and algorithmic composition" ([Wikipedia: "SuperCollider"](https://en.wikipedia.org/wiki/SuperCollider)). SuperCollider comprises a realtime audio engine (server) and a C-like client language (client). Sonic Pi and Overtone are two popular clients these days. I didn't like the SuperCollider client language so much, so I moved onto Sonic Pi ...
1. **[Sonic Pi](http://sonic-pi.net/).** It's a different client language for the SuperCollider engine (plus some stuff, like some useful synth presets). The language is inspired by Ruby and Python. [You can put Sonic Pi on a Raspberry Pi](https://www.raspberrypi.org/documentation/usage/sonic-pi/), making it a great project for classrooms etc. It's easy to pick up, but [it's not just a toy.](https://github.com/josephwilk/sonic-pi-examples) Created and mainly maintained by [Sam Aaron, who you can see presenting on it](https://www.youtube.com/watch?v=ENfyOndcvP0).
2. If/when you want to try something else ...
  1. [Overtone](http://overtone.github.io/). Clojure client. Also uses SuperCollider. Quite popular. I haven't tried it yet.
  2. [Tidal](http://tidalcycles.org/). Haskell DSL. Less popular, yet very compelling. It's weird. It focuses on patterns and rhythms.
      1. According to the official [homepage](http://tidal.lurk.org): "Tidal is a language for live coding pattern(s). It provides a way to express music with very flexible timing, providing a little language for describing patterns as discrete sequences (which can be polyphonic and polymetric), some generators of continuous patterns (e.g. sinewaves, sawtooths) and a wide range of pattern transformations."
      2. [The paper about it, by creator Alex McLean (yaxu)](https://raw.githubusercontent.com/yaxu/Tidal/master/doc/farm/farm.pdf)
      3. Tidal can be hard to install, so at first, you may want to use [this Docker image](https://github.com/DoubleDensity/tidebox) (or [this fork, which is set up for MIDI rather than audio](https://github.com/lvm/tida1vm))

So far my taste is for Sonic Pi for a more malleable thing (it was easier for me to pick up), and Tidal for GETTIN WEIRD and making cool drum patterns

## More resources

* General/alltools
  * [Join TOPLAP on Slack](http://toplap.org/toplap-on-slack/)
  * [Various more environments shouted out in this HN thread](https://news.ycombinator.com/item?id=11054319).
* Max/MSP and Pure Data ... _not textual_ like many of these other things, though
  * [The difference](https://puredata.info/docs/faq/pdmaxjmax)
  * I prefer Max/MSP because of integration with Ableton Live via Max4Live
  * PureData is open-source and truly free
* Browser-based (mainly these are just novelties ... not fully capable)
  * [musiclab.chromeexperiments.com](https://musiclab.chromeexperiments.com/Experiments)
  * [TinyRave](http://tinyrave.com/tracks/47-maple-leaf-rag)
  * [studio.substack.net](http://studio.substack.net/-/recent) (TURN YOUR SPEAKERS DOWN)
* [Raspberry Pi with other stuff (not just Sonic Pi)](https://www.raspberrypi.org/blog/pi-synthesisers/)
* Supercollider, Sonic Pi, Overtone
  * ["Aerodynamic" by Daft Punk: tutorial to recreate it in Sonic Pi](https://aimxhaisse.com/aerodynamic-en.html)
  * [sc140](http://supercollider.github.io/community/sc140), basically "Supercollider Golf," a series of compositions in <= 140 chars of Supercollider code
* Tidal
  * [kindohm's tidal-pattern-every-day tumblr](http://365tidalpatterns.tumblr.com/) has gone past 365 now!
  * [yaxu's "patternlib" of Tidal patterns, that he released along with a recent release](http://slab.org/tmp/patternlib/)

----

# [Livecoding](https://en.wikipedia.org/wiki/Live_coding) to produce **visuals**

TODO
