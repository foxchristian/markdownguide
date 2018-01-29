# Markdown Guide
### Christian Fox (From Wes Bos - Mastering Markdown)

This is a test paragraph. To create paragraphs, a blank line must be left after each sentence.

Paragraph 2. Here I will test bold text. There are 2 ways to create bold and italic text, either with single and double asterisks(*) or with single or double underscores (_). It is common practice to use double ** for bold, and single _ for italic.

**Bolded Text** _italic text_

Strikethrough is achieved wrapping text in double tilde(~~). 

~~Strikethrough text~~

Headings are achieved with # marks. h1 is single #, h2 is double #

# H1 Heading

## H2 heading

### H3 Heading

#### H4 Heading

##### H5 Heading

###### H6 Heading

(Side Note) - Headings can also be written with a solid line of = (3 of more) underlining the heading for h1, or line of - (3 or more) underling for h2.

## Links in Markdown

If full URL needs to be written, text can be wrapped in <> and it will become clickable.

<http://www.google.com>

To add a link to plain text - wrap in square brackets, then follow immediately with brackets containing the URL. If a second attribute is added within "", it refers to the title hover attribute of the link.

[Google](http://www.google.com "This is a link to google")

To neatly embed a link within a long sentence or paragraph, you can use a square bracket reference system. Wrap the text in square brackets, followed by a second set of square brackets, typically enclosing a number. At the bottom of the document, refer to the number in square brackets, followed by a colon, then the link.

[Google][1]

[1]: http://www.google.com

## Images

Displaying images in Markdown is similar to links. It follows a three part protocol. 

! (bang) signifies an image. 

[] Signifies the alt text. 

() Signifies the URL. A title attribute can also be added with the () in ""

![A Cool image](http://unsplash.it/500/500?image=900 "My cool image")

Images can also be used with a referencing system in the same way at links. (square brackets)

It is also possible to use nested image linking within links. This could be useful for linking from a small version of an image to a larger version.

(Side Note): Full HTML tags can be used at any time within markdown, such as IMG, FIGURE, STYLE etc.

## Unordered Lists

Unordered lists can be written with a *, - or + before each item. It is common to change between these in nested lists to diferenciate levels.

* Item 1
* Item 2
    - Item 3
        + Item 4

## Ordered Lists

Ordered lists are writting with a number and dot before each item. It is good practice to use the same number before each item, and markdown will do the rest. This makes re-ordering lists very easy.

1. Wake Up
2. Drink Coffee
3. Go for a walk
4. Learn about Markdown

## Line Breaks

Use a BR tag.

## Horizontal Rule

Use 3 or more either - or = 

## Block Quotes

Use a > before the quote.

> This is my quote - Christian Fox


## Code Blocks

The most basic way to display a code block is to indent the text. Most browswers will automatically interprit the language.

    var hello = "hello";
    var num = 123;

Another way would be to start a code block with 3 backticks followed by the name of the language, then close the block with 3 more backticks.

```javascript
var hello = "hello";
var num = 123;
```
You can also show inline code with the use of single backticks around a code block.

Hey, did you try `var let = 100;`?


Typing ```diff followed by code that contains lines starting with + or - can show code edits.

```diff
var x = 100;
- var y = 10;
+ var y = 20;
```

## Tables

Tables are creating by using the pipe | symbol between cells.

In order to create table headings, a row containing a | followed by - creates headings. The | must be followed by :, left aligned (left) double (center) right aligned (right)

| Table Heading 1 | Table Heading 2 |
|:---------------:|----------------:|
| Cell 1          | Cell 2          |
| Cell 3          | Cell 4          |


## Checkboxes

Checkboxes can be created using a set of square brackets with a space between. If an x is placed between, the box will be checked.

* [ ] Make Coffee
* [x] Eat Pancakes
* [ ] Go to Work


## Github References

To reference github issues & pull-requests in-line, use #3 and a link will be created.

Users can also be referenced using the @ symbol.