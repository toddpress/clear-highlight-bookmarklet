# clear-highlight-bookmarklet


<header>

# Clear Highlight Selection Bookmarklet

</header>

<main>

<section>

## What is it?
### TL;DR
A bookmarklet to help me combat a bad habit of highlighting words as I read them (sometimes as few as 3 words per high-lit chunk)

### TL
For those who don't remember the glory days of bookmarklets, they are basically browswser plugins implemented before there were extension marketplaces. This one in particular removes `background-color` from selections.

_See this contrived use-case for a semantic blockquote:_

> I don't expect it'll help many others, but it will help speed up my productivity, especially with learning from online articles.
> 
> You see, I've noticed a compulsion of mine worsening over time. When reading informational content, such as news or turorials, I'm developing an extremely limiting habit of **highlighting every "chunk" of information** sequentially.
> 
> <footer>-- Todd Pressley <cite>"Stream of Consciousness"</cite></footer>

It depends on the density of the subject matter, as to how often I find myself highlighting and at what "chunk" size. For example, in javascript tutorials, I don't highlight much at all; however, I highlight very frequently (sometimes as much as 3 words per chunk) when reading a technical article from nasa, say one confirming the presense of water on sunlit surfaces of the moon ([link to youtube video release](https://www.youtube.com/watch?v=pXbuElvuY7Q)), or learning functional reactive programming techniques in Haskell.

</section>

<section>

## Installation

To install the highlight clearer bookmarklet, drag the following link into your bookmarks bar.
[Clear Highlight Bookmarklet][1]
[1]:javascript:var sheet = (function() {var style = document.createElement('style'); style.appendChild(document.createTextNode('')); document.head.appendChild(style); return style.sheet;})();sheet.insertRule('*::selection { background-color: transparent !important; }', 0);
Here's the formatted code: 

```js
javascript: var sheet = (function () {
  var style = document.createElement("style");
  style.appendChild(document.createTextNode(""));
  document.head.appendChild(style);
  return style.sheet;
})();
sheet.insertRule("*::selection { background-color: transparent !important; }", 0);
```
</section>

</main>
