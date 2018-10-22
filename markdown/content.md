# Introduction

A typical website is usually divides up into different sections. A header, a navbar, footer and main area. 

It is possible to use <div> to section up the site, but this has a few drawback. A <div> is a grouping tag. It is used to group stuff together, and it doesn't implicitly tell us what kind of content is between these tags.

Semantic tags on the other hand has implied meaning. The `<nav>` tag tells us implicitly that the content inside is for site navigation. This is great for screen readers, web crawlers etc.

These following two examples shows how semantic tags implicitly tells us what kind of content is inside the tags. 

```
<body>
    <div>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
    </div>
    <div>
        <h1>Lazerman</h1>
        <p>Lazerman is the greatest hero of all time.</p>
    </div>
    <div>
        Copyright 2018 Lazerman
    </div>
</body>
```

```
<body>
    <header>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
    </header>
    <main>
        <h1>Lazerman</h1>
        <p>Lazerman is the greatest hero of all time.</p>
    </main>
    <footer>
        Copyright 2018 Lazerman
    </footer>
</body>
```

The second example clearly shows us which section is which without even looking at the content.

---

# Header

The `<header>` element represents a container for introductory content or a set of navigational links. Also elements like a search form, author name or a logo can fit here.

A `<header>` element typically contains:

* heading elements (`<h1>` - `<h6>`)
* logo or icon
* authorship information

Note: There can be several `<header>` elements in one document. But a `<header>` tag cannot be placed within a `<footer>`, `<address>` or another `<header>` element.

```
<header>
    <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="about.html">About</a></li>
    </ul>
</header>
```

---

# Footer

The `<footer>` tag defines a footer for a document or section. Typically, it contains information about the author of a section, links to related documents or perhaps information about the author.

A `<footer>` element typically contains:

* authorship information
* copyright information
* contact information
* sitemap
* back to top links
* related documents

There can be multiple `<footer>` elements in one document.

```
<footer>
  <p>Copyright 2018, Lazerman</p>
</footer>
```

___

# Nav

The `<nav>` tag defines a section of a page that provides site navigation links.

Notice that NOT all links of a document should be inside a `<nav>` element. The `<nav>` element is intended only for major block of navigation links.

You shouldn't put all links inside a `<nav>` element. `<nav>` is only intended for blocks of navigation links, like a menu, or table of content.

Accessibility tools, such as screen readers, can use this element to determine whether to omit the initial rendering of this content.

```
<nav>
  <a href="index.html">Home</a> |
  <a href="about.html">About</a> |
  <a href="contact.html">Contact</a>
</nav>
```

___

# Aside

The `<aside>` tag defines a block of content that is only indirectly related to the main content. It could for example be a sidebar containing further information about something which is mentioned in the main content.

```
<p>Today I finished yet another project on freecodecamp :).</p>
<aside>
  <h4>Freecodecamp</h4>
  <p>Freecodecamp is an open source community that helps people learn how to code.</p>
</aside>
```

----

# Section

The `<section>` tag defines sections in a document, such as chapters, headers, footers, or any other sections of the document.

The `<section>` tag defines a standalone section, without a more specific semantic element to represent it. Often a section will have a heading.

```
<section>
  <h1>Why Lazerman?</h1>
  <p>Lazerman is a lorem ipsum dolor sit amet.</p>
</section>
```

___

# Article

The `<article>` tag specifies independent, self-contained content on the page.

An article should make sense on its own and it should be possible to distribute it independently from the rest of the site.

Examples include:

* Forum post
* Blog post
* Story
* Comment

```
<article>
  <h1>Freecodecamp</h1>
  <p>Freecodecamp is an open source community that helps people learn how to code.</p>
</article>
```
