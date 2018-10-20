# Introduction

A typical website is usually divides up into different sections. A header, a navbar, footer and main area. It is possible to use <div> to section up the site, but this has a few drawback. A <div> is a grouping tag. It is used to group stuff together, and it doesn't explicitily tell the user, or browser, what type of content this is.

These following two examples shows how semantic tags explicitly tells us what kind of content is inside the tags. 

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

The second example clearly shows us which section is which without even looking at the content. This is great for screen readers, search engine robots, developers and everyone.

---

# Header

The `<header>` element represents a container for introductory content or a set of navigational links.

A `<header>` element typically contains:

* one or more heading elements (`<h1>` - `<h6>`)
* logo or icon
* authorship information
* You can have several `<header>` elements in one document.

Note: A `<header>` tag cannot be placed within a `<footer>`, `<address>` or another `<header>` element.

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

The `<footer>` tag defines a footer for a document or section.

A `<footer>` element should contain information about its containing element.

A `<footer>` element typically contains:

* authorship information
* copyright information
* contact information
* sitemap
* back to top links
* related documents

You can have several `<footer>` elements in one document.

```
<footer>
  <p>Copyright 2018, Lazerman</p>
</footer>
```

___

# Nav

The `<nav>` tag defines a set of navigation links.

Notice that NOT all links of a document should be inside a `<nav>` element. The `<nav>` element is intended only for major block of navigation links.

Browsers, such as screen readers for disabled users, can use this element to determine whether to omit the initial rendering of this content.

```
<nav>
  <a href="index.html">Home</a> |
  <a href="about.html">About</a> |
  <a href="contact.html">Contact</a>
</nav>
```

___

# Aside

The `<aside>` tag defines some content aside from the content it is placed in. The aside content should be related to the surrounding content.

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

```
<section>
  <h1>Why Lazerman?</h1>
  <p>Lazerman is a lorem ipsum dolor sit amet.</p>
</section>
```

___

# Article

The `<article>` tag specifies independent, self-contained content.

An article should make sense on its own and it should be possible to distribute it independently from the rest of the site.

Potential sources for the `<article>` element:

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
