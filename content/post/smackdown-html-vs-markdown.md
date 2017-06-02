+++
Description = "Smackdown: HTML vs Markdown"
menu = "main"
Categories = ["technology"]
date = "2017-02-28T10:56:07+02:00"
title = "smackdown: html vs markdown"
Tags = ["technology", "smackdown"]
aliases = ["/post/smackdown-html-vs-markdown"]
ogimage = "https://leantesting.com/wp-content/uploads/2016/04/Markdown-mark.svg_.png"
metadescription = "Which is better for web writing? Here is a smackdown between HTML and Markdown."
+++

<img src="https://leantesting.com/wp-content/uploads/2016/04/Markdown-mark.svg_.png" width="45%">
<img src="https://www.w3.org/html/logo/downloads/HTML5_Badge_512.png" width="45%">

### smackdown - html vs markdown

Welcome to the first Raen Smackdown.

The question today is:

Which is better for web writing, HTML or Markdown?

This is a controversial topic. I use both, and I like both. HTML is more versatile. For layouts and very rich pages, HTML is clearly the way to go.

This topic, however, is about web writing. Content only, not layout. Let's dive in.

### what is html?

Hypertext Markup Language was invented in 1990 by Tim Berners-Lee. Browsers understand this language and use it to determine how a page should be displayed.

### what is markdown?

Markdown is a lightweight markup language that gets converted to HTML. It's simpler than HTML but does not have as many features.

### Samples of both

[Here is an awesome cheat sheet on GitHub - thanks Adam P!](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

I used some examples from it in this smackdown.

#### Title tags:

```
<h1>This is an H1 tag in HTML</h1>
```

```
# This is an H1 tag in Markdown
```
```
<h2>This is an H2 tag in HTML</h1>
```

```
## This is an H2 tag in Markdown
```

For title tags, Markdown clearly smacks down HTML - it's far simpler. **Running total: Markdown 1, HTML 0**

#### Lists:

```
<ul>
<li>List item 1</li>
<li>List item 2</li>
<li>List item 3</li>
</ul>
```

```
* List item 1
* List item 2
* List item 3
```

For lists, Markdown clearly smacks down HTML - there's less typing involved. **Running total: Markdown 2, HTML 0**

#### strong and italic:

```
<strong>strong in HTML</strong>
<em>emphasized in HTML</em>
```

```
**strong in Markdown**
*emphasized in Markdown*
```

For strong and emphasized, HTML wins - although there's more typing, it's clearer. **Running total: Markdown 2, HTML 1**

#### links

```
[link description](http://example-markdown-link/)
```

```
<a href="http://exmaple-html-link">link description</a>
```

This is somewhat close, but Markdown wins due to simpler syntax. **Running total: Markdown 3, HTML 1**

#### images

```
![image alt text](http://example-markdown-image.png)
```

```
<img src="http://example-html-image.png" alt="image alt text">
```

Again, Markdown wins due to simpler syntax. **Running total: Markdown 4, HTML 1**

#### tables

(From the cheat sheet page)

```
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
```
```
<table>
<tr>
  <th>Tables</th>
  <th>Are</th>
  <th>Cool</th>  
</tr>

<tr>
  <td>col 3 is</td>
  <td>right-aligned</td>
  <td align="right">$1600</td>  
</tr>

<tr>
  <td>col 2 is</td>
  <td>centered-aligned</td>
  <td align="center">$12</td>  
</tr>

<tr>
  <td>zebra stripes</td>
  <td>are neat</td>
  <td>$1</td>  
</tr>
</table>
```
This isn't even close. It's a complete smackdown for Markdown. **Running total: Markdown 5, HTML 1**

#### line breaks

```
page break in markdown:

single line break (line 1)
single line break (line 2)

double line break (line 1)

double line break (line 2)

```

```
line break in html:

single line break (line 1)<br />single line break (line 2)
double line break (line 1)<br /><br />double line break (line 2)
```

This one goes to Markdown - putting a space between the lines as desired is less likely to cause mistakes than using tags. **Running total: Markdown 6, HTML 1**


#### page breaks

```
page break in markdown:
---
```

```
page break in html:
<hr>
```

This one goes to HTML - it's more intuitive. **Running total: Markdown 6, HTML 2**

### conclusion

There's more to it than what was covered in this smackdown, but for web writing, it's clear from the above smackdown that for web copy, Markdown is simpler.

HTML still has its place, but for web copy, it's overkill.

Markdown is a good compromise between web-based WYSIWYG editors, like WordPress (easy UI but a lot of drawbacks), and writing raw HTML (great to a certain extent, but too complex for some authors, and perhaps overkill for most web copy use-cases even if you are seasoned web designer or developer.)

Final score: **Markdown 6, HTML 2**

Stay tuned for the next Smackdown.
