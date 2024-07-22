# markdown tutorial
## Text
### Heading 
There are six different types of headings, from heading 1 to heading 6. 

Heading 1 has the biggest text among these headings. 

While heading 6 has the smallest text among these headings.

| Markdown	| HTML | Rendered Output |
| --------- | ---- | --------------- |
| # Heading level 1 | `<h1>Heading level 1</h1>` |	<h1>Heading level 1</h1> | 
| ## Heading level 2	| `<h2>Heading level 2</h2>` | <h2>Heading level 2</h2>	| 
| ### Heading level 3	| `<h3>Heading level 3</h3>` | <h3>Heading level 3</h3>	| 
| #### Heading level 4	| `<h4>Heading level 4</h4>` | <h4>Heading level 4</h4> |
| ##### Heading level 5	| `<h5>Heading level 5</h5>` | <h5>Heading level 5</h5> |
| ###### Heading level 6 | `<h6>Heading level 6</h6>`	| <h6>Heading level 6</h6> |

#### Alternative Syntax

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| Heading level 1 <br> ===============	| `<h1>Heading level 1</h1>` | <h1>Heading level 1</h1> |
| Heading level 2 <br> ---------------	| `<h2>Heading level 2</h2>` | <h2>Heading level 2</h2> |

#### **NOTES**
+ Don't forget to put one space between `#` and the first word.
+ `#` must be consecutive. For example, `## Heading 2` and `# # Heading 2` are **NOT** equivalent.

### Paragraphs
To create paragraphs, use a blank line to separate one or more lines of text.

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| I really like using Markdown. <br> <br> I think I'll use it to format all of my documents from now on.	| `<p>I really like using Markdown.</p> <p>I think I'll use it to format all of my documents from now on.</p>` | <p>I really like using Markdown.</p> <p>I think I'll use it to format all of my documents from now on.</p>
  
#### **NOTES**
Unless the paragraph is in a list, don’t indent paragraphs with spaces or tabs.

### Line Breaks
To create a line break or new line (in html `<br>`), end a line with two or more spaces, and then type return.

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| This is the first line.  <br> And this is the second line. |	`<p>This is the first line.<br> And this is the second line.</p>`	 | <p>This is the first line.<br> And this is the second line.</p> |

#### **NOTES**
Unlike C, one can ***NOT*** `\` to break a new line.

See the example on [Line Break Best Practices](https://www.markdownguide.org/basic-syntax/#line-break-best-practices)

## Emphasis of text
### Bold

| Markdown | HTML | Rendered Output |
| -------- | ----- | -------------- |
| `I just love **bold text**`. |	`I just love <strong>bold text</strong>`.	| I just love <strong>bold text</strong> |
| `I just love __bold text__.` | `I just love <strong>bold text</strong>.` | I just love <strong>bold text</strong>. |
| `Love**is**bold`	| `Love<strong>is</strong>` | Love**is**bold |

#### **NOTES**
There don't exist this syntax. Such as `Love__is__bold`.

### Italic

| Markdown | HTML | Rendered Output |
| -------- | ---- | --------------- |
| `Italicized text is the *cat's meow*.` | `Italicized text is the <em>cat's meow</em>.`	| Italicized text is the <em>cat's meow</em>. |
| `Italicized text is the _cat's meow_.`	| `Italicized text is the <em>cat's meow</em>.`	| Italicized text is the <em>cat's meow</em>. | 
| `A*cat*meow` | `A<em>cat</em>meow` | A*cat*meow

#### **NOTES**
There don't exist this syntax. Such as `A_cat_meow`.

### Bold and Italic

| Markdown | HTML |	Rendered Output |
| -------- | ---- | --------------- |
| `This text is ***really important***.` | `This text is <em><strong>really important</strong></em>.` | This text is <em><strong>really important</strong></em>.|
| `This text is ___really important___.` | `This text is <em><strong>really important</strong></em>.` |	This text is <em><strong>really important</strong></em> |
| `This text is __*really important*__.`	| `This text is <em><strong>really important</strong></em>.`	| This text is <em><strong>really important</strong></em> |
| `This text is **_really important_**.` | `This text is <em><strong>really important</strong></em>.` | This text is <em><strong>really important</strong></em> |
| `This is really***very***important text.`	| `This is really<em><strong>very</strong></em>important text.`	| This text is <em><strong>really important</strong></em> |

#### **NOTES**
There don't exist this syntax. Such as `This is really___very__important text.`.

#### **NOTES** 
The order of the em and strong tags might be reversed depending on the Markdown processor you're using.

## Blockquotes
To create a blockquote, add a > in front of a paragraph.

    > Dorothy followed her through many of the beautiful rooms in her castle.

The rendered output looks like this:

> Dorothy followed her through many of the beautiful rooms in her castle.
