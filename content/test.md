---
views:
    byline:
        region: after-main
        template: default/content
        sort: 1
        data:
            meta:
                type: content
                route: block/byline
...
INTRODUCTION TO MARKDOWN
=======

## HEADERS

Markdown offers two styles of headers: Setext and atx. Setext-style headers for `<h1>` and `<h2>` are created by “underlining” with equal signs (=) and hyphens (-), respectively. To create an atx-style header, you put 1-6 hash marks (#) at the beginning of the line — the number of hashes equals the resulting HTML header level.
>
> H1 with *setext*
> ================
> #H1 with atx
> H2 with *setext*
> -----------------
> ##H2 with atx
> ###H3 with atx


## EMPHASIS

Markdown uses asterisks and underscores to indicate spans of emphasis.

You can either use * or _ around a word to emphasis it, like *this* or _this_. 

If you want to make a strong emphasis you use ** or __, like **this** or __this__.
Some of these words _are emphasized also_.

## LISTS 

Unordered lists are creating by putting one of these characters at the start of each line, *, - or +. 

*   List item
+   List item
-   List item

    With multiple paragraphs.

    
*   Another item in the list.
For ordered lists you type numbers in front. 
 
 1. List item
 2. List item
 3. List item

## LINKS {#url}

Markdown supports two styles for creating links: inline and reference. With both styles, you use square brackets to delimit the text you want to turn into a link.

Inline-style links use parentheses immediately after the link text. For example:

This is an [example link](http://example.com/).

Reference-style links allow you to refer to your links by names, which you define elsewhere in your document:

I get 10 times more traffic from [Google][1] than from
[Yahoo][2] or [MSN][3].

[1]: http://google.com/        "Google"
[2]: http://search.yahoo.com/  "Yahoo Search"
[3]: http://search.msn.com/    "MSN Search"

Linking to other pages {#url}
---------------------------------

I can link to another document. In the same directory like the file [license.md](license). Or in another directory like [report/kmom01](report/kmom01).

It does not matter in what subdirectory we are. All urls that are relative, will be prepended with the site base url. The base url will be the url to the [`htdocs`]() directory.

You can find a copy of this file in a subdirectory [`example/markdown.md`](example/markdown). Try it out to verify that all urls work in both this document and in the document in the subdirectory.



Linking to image sources {#img}
---------------------------------

Linking to image sources works in the same manner as linking to other pages. Anax will prepend the base url to all relative image sources.

Here are some samples on how you can link to a image using Markdown or HTML.

```text
![alt text](img/dbwebbisar.jpg)
<img src="img/dbwebbisar.jpg" alt="alt text">
```

This is the outcome of the two images.

![alt text](img/dbwebbisar.jpg)

<img src="img/dbwebbisar.jpg" alt="alt text">



Creating a mailto: link {#mailto}
---------------------------------

You can create a mailto link using Markdown or HTML. It looks like this.

```text
<mailto:user@example.com>
<user@example.com>
<a href="mailto:user@example.com">user@example.com</a>
```

The resulting links looks like this.

* <mailto:user@example.com>
* <user@example.com>
* <a href="mailto:user@example.com">user@example.com</a>
