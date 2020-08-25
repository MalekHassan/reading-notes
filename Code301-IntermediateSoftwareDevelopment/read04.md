
### Grid

SS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system. You work with Grid Layout by applying CSS rules both to a parent element (which becomes the Grid Container) and to that element’s children (which become Grid Items).

*display*

Defines the element as a grid container and establishes a new grid formatting context for its contents.

*Values:*

* grid – generates a block-level grid
* inline-grid – generates an inline-level grid

**grid-template-columns**

**grid-template-rows**

Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.

*Values:*

*track-size* – can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit)

*line-name* – an arbitrary name of your choosing

**grid-template-areas**

Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. Repeating the name of a grid area causes the content to span those cells. A period signifies an empty cell. The syntax itself provides a visualization of the structure of the grid.

*Values:*

*grid-area-name* – the name of a grid area specified with grid-area

. – a period signifies an empty grid cell
none – no grid areas are defined

**grid-template**

A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.

*Values:*

none – sets all three properties to their initial values
*grid-template-rows* / *grid-template-columns* – sets grid-template-columns and grid-template-rows to the specified values, respectively, and sets grid-template-areas to none

**gap**

**grid-gap**

A shorthand for row-gap and column-gap

*Values:*

*grid-row-gap* *grid-column-gap* – length values

**justify-items**

Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). This value applies to all grid items inside the container.

*Values:*

start – aligns items to be flush with the start edge of their cell
end – aligns items to be flush with the end edge of their cell
center – aligns items in the center of their cell
stretch – fills the whole width of the cell (this is the default)

**align-items**

Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis). This value applies to all grid items inside the container.

*Values:*

* start – aligns items to be flush with the start edge of their cell

* end – aligns items to be flush with the end edge of their cell

* center – aligns items in the center of their cell

* stretch – fills the whole height of the cell (this is the default)

**place-items**

place-items sets both the align-items and justify-items properties in a single declaration.

*Values:*

* *align-items* / *justify-items* – The first value sets align-items, the second value justify-items. If the second value is omitted, the first value is assigned to both properties.

* All major browsers except Edge support the place-items shorthand property.


### Responsive design with CSS Grid

* CSS Grid Layout is growing in browser support every day and we can ship CSS Grid to production. The quick adoption of CSS Grid has been truly remarkable.

* Before we get to making a responsive portfolio site layout with CSS Grid, let’s clear a couple of things up: CSS Grid is not a replacement for Flexbox. It’s not even a replacement for floats. In fact, you might realise that we’ve been using Flexbox to do things that CSS Grid does much better. But instead of thinking in terms of replacement, we can think in terms of combination.


Do you often find yourself banging your head against the wall when trying to make your page responsive? I sure did for a long time, that was before I became familiar with the grid system. I had already seen and used grid a few times but I was a little intimidated by the huge amount of properties that it has to offer, but today I’m pretty comfortable creating layouts with just CSS Grid, so in this article, I want to show you what I think are the most important properties that you can use in CSS grid to make your web page fully responsive.

* The way I see it there are two main ways to use this amazing tool in your page, those are:

* Grid template columns & rows or grid areas combined with media queries.

* Grid template columns & rows combined with the repeat and minmax functions.

**Combining grid with media queries**

* This is the easier way, in my opinion, to adapt your page to multiple screen sizes. The trick is to create your initial layout using the grid template columns (and grid template rows if you need explicit rows) or grid template areas and utilize media queries to change the display of your container depending on the screen size, simple right? Let’s see this in action.

* Utilizing grid template columns and rows to their full potential If you choose this method, you’ll have a more compact set of rules and you won’t even have to write a single media query, isn’t that amazing?! To make this work you’ll need to be familiar with the repeat, auto-fill & auto-fit, and the minmax functions.

**Conclusion**

To wrap this up I would like to point the biggest drawback of using the second method, which is that if you want to remove content from your grid as your page gets smaller, you won’t be able to make that happen. Instead, it would be better to resort to mixing media queries in your stylesheet, that way at the same time that you change the grid template columns at each breakpoint, you can also set the display of the elements that should be hidden to display: none.

### Regex

* Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).

* Fields of application range from validation to parsing/replacing strings, passing through translating data to other formats and web scraping.

* One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).

**Summary**

As you’ve seen, the application fields of regex can be multiple and I’m sure that you’ve recognized at least one of these tasks among those seen in your developer career, here a quick list:

* data validation (for example check if a time string i well-formed)

* data scraping (especially web scraping, find all pages that contain a certain set of words eventually in a specific order)

* data wrangling (transform data from “raw” to another format)

* string parsing (for example catch all URL GET parameters, capture text inside a set of parenthesis)

* string replacement (for example, even during a code session using a common IDE to translate a Java or C# class in the respective JSON object — replace “;” with “,” make it lowercase, avoid type declaration, etc.)

* syntax highlightning, file renaming, packet sniffing and many other applications involving strings (where data need not be textual)

