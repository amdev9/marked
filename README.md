<a href="https://marked.js.org">
  <img width="60px" height="60px" src="https://marked.js.org/img/logo-black.svg" align="right" />
</a>

# Marked with custom links

[![npm](https://badgen.net/npm/v/marked4)](https://www.npmjs.com/package/marked4)
 
## Installation

**CLI:** `npm install -g marked4`

**In-browser:** `npm install marked4 --save`
 

New test cases:

```
[[Empty|/url/]]

[[Empty | /url/]]

[[Hello world | aphanum:hello-world]]

[[Hello world]]

[[One more  world]]

[[ Marked | https://github.com/markedjs/marked/blob/master/lib/marked.js]]

```

Results:

```
<p><a href="/url/">Empty</a></p>

<p><a href="/url/">Empty</a></p>

<p><a href="aphanum:hello-world">Hello world</a></p>

<p><a href="hello-world">Hello world</a></p>

<p><a href="one-more-world">One more  world</a></p>

<p><a href="https://github.com/markedjs/marked/blob/master/lib/marked.js">Marked</a></p>

```