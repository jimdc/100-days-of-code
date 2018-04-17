# 100 Days Of Code - Log

### Day 0: March 26, 2018

**Today's Progress**: Scraped `textContent` with `document.querySelector()` for gender-reveal.

**Thoughts:** Not sure how much I should pay attention to Javascript's unique way of scoping, in light of browser optimizations. Still using JSLint but more skeptical of it. Finding out where the page "reloads" in React is tricky.

**Link to work:** [gender-reveal](https://github.com/jimdc/gender-reveal)

### Day 1: March 27, 2018

**Today's Progress**: Made gender-reveal more modular, added gendered pronouns (which work in theory).

**Thoughts:** No way this extension can work on every exercise, and on especially some languages like German, without some NLP processing of how words relate to each other in the context of a sentence.

**Link to work:** [gender-reveal](https://github.com/jimdc/gender-reveal)

### Day 2: March 28, 2018

**Today's Progress:** Gendered-pronouns work in practice, scaffolding for multiple-choice.

**Thoughts:** I wonder if I should have dummy HTML pages, serving dynamic content in similar classes to test this script? Because I couldn't *even* with this external service to serve me a certain type of question. 

**Link to work:** [gender-reveal](https://github.com/jimdc/gender-reveal)

### Day 3: March 29, 2018

**Today's Progress:** Walked through "[create a quiz with react](https://mitchgavan.com/react-quiz/)". 

**Thoughts:** The concept of props and state is still shaky to me, but I loved seeing how the modularity made it easy to refactor.

**Link to work:** [translate-jokes](https://github.com/jimdc/translate-jokes)

### Day 4: March 30, 2018

**Today's Progress:** Fixed bug in gender-reveal where source language prompts were colored according to target language pronouns.

**Thoughts:** I'm starting to miss static type checking. Starting to wonder about profiling this script's memory usage (is a 100ms recurring timeout expensive?)

**Link to work:** [gender-reveal issue #2](https://github.com/jimdc/gender-reveal/issues/2)

### Day 5: March 31, 2018

**Today's Progress:** Configured a toy React project without using `create-react-app`

**Thoughts:** I'm curious about how express.js is used here.

**Link to work:** [jimbo-scales](https://jimbo-scales.herokuapp.com/)

### Day 6: April 1, 2018

**Today's Progress:** Sort-of deployed personal-website to Heroku. 

**Thoughts:** More like 100-days-of-configuration-hell. Learning difference between `dependencies` and `devDependencies` in `npm`. I probably should know better how `webpack` works. Is using both `npm` and `yarn` bad? Which differences should I maintain between the development and production builds? Deployment is hard.

**Link to work:** [jimbo-scales](https://jimbo-scales.herokuapp.com/)

### Day 7: April 2, 2018

**Today's Progress:** Watched a JavaScript tutorial.

**Thoughts:** The most interesting topics to me were: anonymous functions, immediately invoked functional expressions, `let` and `const`, objects, closures

**Link to work:** It gave me an idea for [an enhancement](https://github.com/jimdc/gender-reveal/issues/3) to gender-reveal.

## Day 8: April 3, 2018

**Today's Progress:** Mocked up a Node CLI app for transcription into Chinese.

**Thoughts:** I'm eager to learn about unit testing in node. Also, is there a dobule-metaphone that makes working with IPA, or just in general, easier? If not, I see an opportunity for my first npm module.

**Link to work:** https://github.com/jimdc/transcribe-en-to-zh

## Day 9: April 4, 2018

**Today's Progress:** Updated some existing code to ES6 and TypeScript; fixed a timeout redundancy issue

**Thoughts:** 100-days-of-build-tool-bamboozle. I'm beginning to really enjoy npm's `package.json` system; next I would like to know how to `scripts` within it, and I still have trouble figuring out the deal with live monitoring for file changes. TypeScript is quite comfy.

**Link to work:** (diffs) [TypeScript](https://github.com/jimdc/transcribe-en-to-zh/commit/40660824e6292a584fbc490712746c66c7849086), [issue](https://github.com/jimdc/gender-reveal/commit/e4f76ec00a5a792111881af54564a4eb6b39e021)

## Day 10: April 5, 2018

**Today's Progress:** Added a mocha test to transcribe, start basic scraper rules

**Thoughts:** Doesn't seem to be a great ready-made solution to convert metaphone to IPA, or english to IPA for that matter. Working with JSON is so pleasant.

**Link to work:** (diff) [transcribe-en-to-zh](https://github.com/jimdc/transcribe-en-to-zh/commit/e50e2162a19861244603a9f4168a6e861257d2d2#diff-a091ca09d9fdc9eb5f89ae98eac72d05)

## Day 11: April 6, 2018

**Today's Progress:** Started integrating `transcribe.ts` and `scrape.ts` in `transcribe-en-to-zh`

**Thoughts:** With the rulebuilder it doesn't matter, but I wanted to use node 8's [util.promisify](https://hackernoon.com/node8s-util-promisify-is-so-freakin-awesome-1d90c184bf44) to read the json rules file asynchronously in `ChineseSound.ts`, with a view towards when this is a non-cli based webapp.

**Link to work:** [diff](https://github.com/jimdc/transcribe-en-to-zh/commit/f45b028b20c2ab96b9de86ee5450715cfe69c745)

## Day 12: April 7, 2018

**Today's Progress:** migrated personal website from [Jekyll](https://github.com/jekyll/jekyll) to [Gatsby](https://www.gatsbyjs.org/)

**Thoughts:** Looks like I'll have to add some text paragraphs with some outlinks, because if Javascript is disabled, font-awesome social icon placeholders are just asterisks. But redundancy is OK, since part of the idea of a progressive web app is to make your own navigation interface. Ended up learning some stuff about git, like how to revert to a previous branch, from when this migration went wrong.

**Link to work:** http://www.jamesdcarroll.me/

## Day 13: April 8, 2018

**Today's Progress:** Got pronoun color functionality up in gender-reveal

**Thoughts:** I also tried to [do class-based coloring](https://github.com/jimdc/gender-reveal/issues/4) based on a pure JavaScript solution, which failed because for some security reasons, Greasemonkey [has its own ways](https://stackoverflow.com/posts/19392142/revisions) of adding to the global CSS, which I will continue next time, along with the GM_setValue() stuff.

**Link to work:** (diffs to visible progress) [1](https://github.com/jimdc/gender-reveal/commit/7f48e29f2c0958a627bb02b2e1a7aae66d7da035) [2](https://github.com/jimdc/gender-reveal/commit/f8d00d30507b0c3e597277cf730cabfa90905f56)

## Day 14: April 9, 2018

**Today's Progress:** TDD approach to fixing colspan (soon: rowspan) in `transcribe-en-to-zh`

**Thoughts:** I really appreciated being able to run `npm test` after every refactor to make sure that previous functionality didn't break either. TDD is awesome, and the way I did things beforehand seems unbearably tedious now.

**Link to work:** (diffs) [failing test](https://github.com/jimdc/transcribe-en-to-zh/commit/69a5d10fd2e46b1d16b9890ab56c07473805ecdb) [code to pass test](https://github.com/jimdc/transcribe-en-to-zh/commit/563b26f7eabdbb2fe5616fc832ce4b7ea1ab8148)

## Day 15: April 10, 2018

**Today's Progress:** Fixed 1/2 of rowspan (the expanded entry but not its followers) using TDD

**Thoughts:** Keeping track of all these indices is becoming tedious; more like "real work" than a fun side project to learn new technology. I'm also running into certain conceptual problems that arise from the fact that I'm dealing with `each()` callbacks instead of loops, which I am more used to; so some of the scoping issues are mystifying. It's probably time to make `scrape.ts`'s table-building function more modular.

**Link to work:** [failing test](https://github.com/jimdc/transcribe-en-to-zh/commit/0515d0c1cadc05a3fc6bb1a249cded1f18db0d24), [partial success](https://github.com/jimdc/transcribe-en-to-zh/commit/136ba12f367063309903453a1f3f1b4a96c5edb7)

## Day 16: April 11, 2018

**Today's Progress:** Fell in love with Python again.

**Thoughts:** The only other thing to do for this program to be useful to me personally, would be to add support for (1) multiple file-in and file-out; (2) returning status code back to stdout to chain as part of shell script; and (3) giving rules and resume files as command-line arguments

**Link to work:** [resume-anonymizer](https://github.com/jimdc/resume-anonymizer)

## Day 17: April 12, 2018

**Today's Progress:** Converted HTML scrape to Retrofit/RXJava.Single (closed source, Kotlin) 

## Day 18: April 13, 2018

**Today's Progress:** Started my first Go program

**Thoughts:** It feels new and familiar at the same time. Amazing. Hope I can find some way to use goroutines here, or at least the reflection capability to automatically parse objects to JSON/XML/whatever. 

**Link to work:** [caffgraph/halflife.go](https://github.com/jimdc/caffgraph/blob/master/halflife.go)

## Day 19: April 14, 2018

**Today's Progress:** Started frontend for `caffgraph`, continuing with Go

**Thoughts:** I really like that Go gives me an error if I declare an import or a variable without using it. Reminds me about a feature I might have stopped implementing in the middle of wanting to implement another feature. Might have to make this into a package situation soon. `defer` is interesting. SVG is great: what's not to love about human-readable image format that lets you use existing CSS knowledge?

**Link to work:** [caffgraph diff](https://github.com/jimdc/caffgraph/commit/1b8cfd5360558dc6f5bdfe179bb4103a04289a30#diff-a8b6c9f79d0e30a8c9781f60764610ba)

# Day 20: April 15, 2018

**Today's Progress:** `caffgraph`'s `halflife.go` now writes to file

**Thoughts:** d3 might not mind if the csv entries are not in chronological order, so trying out *nonblocking* concurrency next might be cool. Reading existing input and integrating the new entries would be harder, which is why I wanted to automate feeding it info from `stdin`, but actually it might be much simpler to do with command line switches.

**Link to work:** [caffgraph diff](https://github.com/jimdc/caffgraph/commit/d83f59ec9ee612a7d08008c9f5407c633fec4d06#diff-a8b6c9f79d0e30a8c9781f60764610ba)

# Day 21: April 16, 2018

**Today's Progress:** `caffgraph` uses flags, starting csv-to-json transition

**Thoughts:** D3.js: hard to debug. I've been spoiled by Node. Go's error messages are really good too. Marshalling JSON manually is really cool because of reflection in Go and all, but I think it's too tedious when time is precious. Still don't know how to deal with two overlapping lines, when those lines represent remnants. Well, first I will focus on drawing the overlap, and maybe there can be a programmatic toggle whereby they are combined.

**Link to work:** [diff](https://github.com/jimdc/caffgraph/blob/1150d793a7ce534ec3f9e209461928a9831165f7/halflife.go#L1)

# Day 22: April 17, 2018

**Today's Progress:** Enabled standard json.Unmarshal, used `gofmt`

**Thoughts:** json.Unmarshal was silently failing at first because the struct members were not visible to `encoding/json` because, like, `remnant` wasn't named `Remnant` and so forth. It couldn't have returned some kind of error to indicate that an empty struct is probably not what you want? Next, I think it would be good to define a test case for the desired behavior in the event that it encounters an overlapping dose. Also, instead of overwriting it should append. 

**Link to work:** [new halflife.go](https://github.com/jimdc/caffgraph/blob/8990d4566b3c0753139cddfa9ae1aea334d573f7/halflife.go)
