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

**Today's Progress:**

**Thoughts:**

**Link to work:** 
