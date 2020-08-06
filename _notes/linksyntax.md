---
title: Link Syntax
---

To link to another note, I use regular [Markdown syntax](https://www.markdownguide.org/getting-started/) for links, with a relative link to the other note, like this: [this is a link to a note about cats](/cats){: .internal-link}. To make sure the link is styled as an internal link, I use the `.internal-link` class 

Since the Web is all about HTML, I can always use plain HTML like this: <a class="internal-link" href="/cats">This is the same note about cats as above</a>.

To link to external websites, like this: [this is a link to Wikipedia](https://wikipedia.org/). Again, I can also use plain HTML.

Additionally, to use Roam/wiki-style link syntax by wrapping a note's title in double brackets, like this: [[A note about cats]]. If the Roam-style link does not point to a valid note's title, the double brackets will still be shown, like this: [[There is no note with this title]].

### Automatic bi-directional links

Notice in the "Notes mentioning this note" section that there is another note linking to this note. This is a bi-directional link, and those are automatically created when you create links to other notes.

### Link previews

If you're on a device with mouse support, try hovering your mouse on internal links to preview the notes: [[A note about cats]]

### Images

Finally, you can display images using Markdown syntax, like this:

![]({{page.image}})


