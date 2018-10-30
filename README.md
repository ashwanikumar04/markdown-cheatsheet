
```Markdown
# Markdown Basics
## Headlines, Paragraphs, and Basic Formatting
### Headlines
#### Heading Level 4
##### Heading Level 5
###### Heading Level 6
```
# Markdown Basics
## Headlines, Paragraphs, and Basic Formatting
### Headlines
#### Heading Level 4
##### Heading Level 5
###### Heading Level 6

### Paragraphs and Line Breaks

```Markdown
We create paragraphs by typing the way we would in any other program. Just hit return twice to start another paragraph.

Where we see empty space between blocks of text in our Markdown document, we will see empty space separating those blocks of text in our formatted HTML document.
```

We create paragraphs by typing the way we would in any other program. Just hit return twice to start another paragraph.

Where we see empty space between blocks of text in our Markdown document, we will see empty space separating those blocks of text in our formatted HTML document.

#### Line Breaks

We don’t always want that space that appears between one line of text and another: for example, lines of poetry or song lyrics don't have spaces between them. To add just a line break without a space, type **two spaces** at the end of a line, then press return once.

```Markdown
Line 1 testing  
Line 2  
Line 3  
```
Line 1 testing  
Line 2  
Line 3  

### Emphasis and Bolding

#### Italics

Emphasis can be added with either the asterisk or the underscore characters.
```Markdown

This *works*, and this _works_ too

```
This *works*, and this _works_ too

#### Bolding

Bolding is easy too. Just add an extra asterisk or underscore.

```Markdown

This **works**, and this __works__ too

```
This **works**, and this __works__ too


#### Bolding and Emphasis Together

```Markdown

We can even bold and italicize text like ***this*** or ___this___

```

We can even bold and italicize text like ***this*** or ___this___

### Block quotes

A blockquote sets text apart from the rest of the document. It indicates that the text is quoted from another source.

We format a blockquote using the greater than symbol. If we want a blockquote to span multiple paragraphs, add the greater than symbol to the line between paragraphs too.

```Markdown

> Markdown is intended to be as easy-to-read and easy-to-write as is feasible.
>
> Readability, however, is emphasized above all else. A Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions. — [John Gruber](https://daringfireball.net/projects/markdown/ "The Creator of Markdown")

```
> Markdown is intended to be as easy-to-read and easy-to-write as is feasible.
>
> Readability, however, is emphasized above all else. A Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions. — [John Gruber](https://daringfireball.net/projects/markdown/ "The Creator of Markdown")

### Horizontal Rule

We can separate this from our next section with a horizontal rule, which is just a line used to separate sections of a document.

We can use three or more underscores, asterisks, or hyphens.
```Markdown

___

***
---
```
___

***

---

## Lists

We can write both numbered and bulleted lists with Markdown.

### Numbered Lists

We create numbered lists like we do in other writing programs. Type the number, a period, a space, and the item label.
```Markdown

1. Item One
2. Item Two
```

1. Item One
2. Item Two

To nest an item, indent it with a tab or at least two spaces beneath the item above it.

```Markdown

1. Item One
    1. Nested Level Two
    2. Nested Level Two
        1. Nested Level Three
        2. Nested Level Three
```

1. Item One
    1. Nested Level Two
    2. Nested Level Two
        1. Nested Level Three
        2. Nested Level Three

#### Bulleted Lists

Bulleted lists work like numbered lists, but we use the asterisk character, a space, and no period.
```Markdown

* Item One
* Item Two
```

* Item One
* Item Two

We can nest bulleted items too. We just indent our item below another item like we did with our numbered list.
```Markdown

* Item One
    * Nested Item One
    * Nested Item Two
```
* Item One
    * Nested Item One
    * Nested Item Two

```Markdown

* ***Bold Italicized Bulleted Item***
```
* ***Bold Italicized Bulleted Item***

#### Mixed Lists

We can mix the two list styles too. Just use the numbers or asterisks where we want them.
```Markdown

1. Item One
    * Nested Item
    * Nested Item
2. Item Two
    * Nested Item
    * Nested Item
        1. Deep Nested Item One
        2. Deep Nested Item Two
            * Super Deep Nested Item
            * Super Deep Nested Item
```

1. Item One
    * Nested Item
    * Nested Item
2. Item Two
    * Nested Item
    * Nested Item
        1. Deep Nested Item One
        2. Deep Nested Item Two
            * Super Deep Nested Item
            * Super Deep Nested Item

---

## Code

We format code using the backtick character. 
We can use a single backtick to create inline code. For example, we may type something like this:

```Markdown
To install the latest version of NPM, we can type,  `npm install npm@latest -g`
```

To install the latest version of NPM, we can type,  `npm install npm@latest -g`

For multiple lines of code, we'll usually create a code block. Instead of one backtick, use three back ticks above and below the code block. Some sites and editors also support syntax highlighting by language. Add it by typing the name of the coding language immediately after the top three back ticks.
```Markdown
```Javascript
let exampleFunction = () => {
  let foo = 'foo';
  let bar = 'bar';

  return foo + bar;
}
```

```Javascript
let exampleFunction = () => {
  let foo = 'foo';
  let bar = 'bar';

  return foo + bar;
}
```

---

## Links

Markdown provides a syntax for links that’s easy to remember. First, type the text we want to appear on the page in square brackets, then add the link in parenthesis. If I want to link to Github, I would type

```Markdown

[Github](https://github.com/)

```

[Github](https://github.com/)


We also have the option to provide a title, which appears when we hover the mouse cursor over the link. Just type a space after the url and close the label in quotes. Both the url and the title should be inside the parenthesis.

```Markdown

[Github](https://github.com/ "Github link with a title")

```

[Github](https://github.com/ "Github link with a title")

What if we want to link to a reference at the bottom of a section or page like a footnote? Start with the text in square brackets, but don’t add the parenthesis. Instead, add a number to reference in another set of square brackets.

```Markdown

[Github][1]

```

[Github][1]

Now at another place in the document, add the reference number in square brackets and follow it with a colon, a space, and the link url. we can add an optional title with a space and quotes to this type of link too. Reference links don’t require parenthesis.

```Markdown

[1]: https://github.com "Github Reference Link"

```

[1]: https://github.com "Github Reference Link"

---

## Images

Type a label for the image in square brackets. On the Web we call this alt text, because it will be displayed as an alternate if the image cannot be shown for any reason. I have an image of kittens, so I’ll write, “Kittens” in square brackets and follow that with the url for the image in parenthesis.

That creates a link for the kitten image, but I want to display the image. All I have to do is add an exclamation mark in front of the square brackets.

```Markdown

![Kittens](https://placekitten.com/250/400)

```

![Kittens](https://placekitten.com/250/400)


What if I want the image to link to something too? Just add square brackets around our whole image code. At the end of the new square brackets, put the link url in parenthesis.

```Markdown

[![Kittens](https://placekitten.com/300/400 "Fluffy Kitten")](https://placekitten.com)

```

[![Kittens](https://placekitten.com/300/400 "Fluffy Kitten")](https://placekitten.com)

Images can have titles like links too. We add them the same way. After the image url, add a space and put the title in quotes.

```Markdown

[![Kittens](https://placekitten.com/350/400 "Curious Kitten")](https://placekitten.com)

```

[![Kittens](https://placekitten.com/350/400 "Curious Kitten")](https://placekitten.com)

---
