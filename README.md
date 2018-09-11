# EPUB Reader Comparison

## Summary 
A critical evaluation of two EPUB Readers: [ReadiumJS Viewer](https://github.com/readium/readium-js-viewer) and [Epub.js Reader](https://github.com/futurepress/epubjs-reader/)

## How to Choose? 
NPM's ["How to Choose Between Similar Packages"](https://docs.npmjs.com/getting-started/searching-for-packages#how-to-choose-between-similar-packages) is a helpful start:
<pre>
<b>Popularity</b> indicates how many times the package has been downloaded. This is a
good indicator of packages that others have found to be especially useful, but
not foolproof.

<b>Quality</b> includes considerations such as the presence of a readme file,
stability, tests, up-to-date dependencies, custom website, and code complexity.

<b>Maintenance</b> ranks packages according to the attention given by developers.
Packages that are maintained more frequently are more likely to work well with
the current or upcoming versions of npm, for example.
</pre>

### Other Questions to Ask
* Does the license suit your needs?
* How easy is it to integrate this library into my current workflow?
  * How easy would it be to migrate _to_ this library?
  * How easy would it be to migrate _from_ this library?
* When was this project started?
* How many active contributors?
* When was the most recent activity?
* Have there been major releases recently? Just minor? Just bugfixes?
* What is the version number?
	* The presence of a prerelease tag (-alpha, -beta) indicates substantial risk, as does a major number of zero (0.y.z), which may contain any level of potentially breaking changes.
* Is the README well-written? Does the formatting show care?
	* Attention paid to small details is usually a good sign for the big picture, too

## Conclusion
**Both** libraries are free to use commercially, and both have similarly recent commits. It's hard to say which reader will best integrate with an unknown workflow, and without knowing the full scope of the project.

I do appreciate the attention to detail in **Epub.js**, and the code seems well-written: succinct without being confusing. It's written in a consistent style, which is nice for readability. However, this consistency is due to there being only [one contributor](https://github.com/futurepress/epubjs-reader/graphs/contributors). Such a high [bus factor](https://en.wikipedia.org/wiki/Bus_factor) is a tough pill to swallow when considering a library's use in production. 

**Readium JS** may not have the polished style of the Epub.js examples, but it's got functionality where it counts. It has tests (Epub does not), it has 417 closed issues (Epub: 5), 1720 commits (Epub: 12), and 22 active contributors (Epub: 1). The project does seem to sprawl a bit, but that comes naturally in a feature-rich project. Support does not seem like an issue, especially considering it is a sub-library of a larger, well-maintained project.

Ultimately, **Epub.js** would be a nice choice for a small project, due to its compact size and readability. Good for getting something relatively polished off the ground quickly.

Conversely, **Readium JS** seems like the go-to for a large project with complex requirements. Its testing suite and comparably robust dev community engender confidence for the customer-facing project with a long life cycle.
